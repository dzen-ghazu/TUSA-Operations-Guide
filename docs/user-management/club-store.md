---
title: Connecting Users to a Club Store
hide:
  - toc
---
# **Connecting Users to a Club Store**

> **The golden rule:** You **cannot** connect a user to a store by editing their role on the **Users → Edit User** screen. Changing a role to `vendor staff` there does **not** link them to the club’s store — it leaves them half-connected and Dokan attaches them to the **TUSA Store** instead. Store membership is handled by automation, on purpose. This page explains why, the two correct ways to do it, and how to recover a user who got attached to the wrong store.

---



## **Why you can’t do it on the Edit User screen**

A user’s **role** and their **store membership** are two separate things:


|  | What it is | How it’s set |
| --------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------------- |
| `vendor_staff` **role** | A permission flag — “this person is allowed to work in *a* store” | Added by the automation (or by you, but that alone does nothing useful) |
| **Store link (**`_vendor_id`**)** | *Which* store they belong to | **Only** set by the automation — never by editing the role |


Adding the `vendor_staff` role by hand sets the permission flag but **not** the store link. The account ends up as staff with no proper store, and Dokan resolves that to the **TUSA Store** — which is why the store URL slug changes to `…/club-store/tusa`.



### **A store link is a whole transaction, not one field**

This is the heart of it: **linking a user to a store is much more than assigning a vendor ID.** A working link is a set of changes the automation makes *together, in one go*:

- the `vendor_staff` **role**
- the **Dokan permissions** that actually let them open and work in the store dashboard
- the **“selling enabled”** flag Dokan checks before it lets them in
- the **store identity** — which store (by vendor ID), plus the store-switcher record that keeps it consistent
- a **cache clear** so the change takes effect, plus internal notifications other parts of the system rely on

Setting the vendor ID by hand in the back end does **one** of those and skips the rest. That’s why backend fiddling only ever gets you **halfway**: the account *looks* linked, but the permissions, the selling flag and the store identity are out of step — so it lands on the wrong store, or can’t open the dashboard, and breaks in ways that are hard to spot.

**This is exactly why the workflows are built the way they are.** Promoting an Organizer, or using the Team page, runs *all* of those steps as one safe operation — enforcing the one-store rule and keeping everything in sync. There is deliberately **no single back-end switch** for it, because a half-applied link is worse than no link at all.

**This is also why roles are additive, not exclusive.** A club exec who shows as **Hire Store Customer** or **Club Admin** can *also* hold `vendor_staff` — that’s normal and correct. Don’t try to “fix” their profile type or swap their role to connect them to a store. The profile type and the store link are unrelated.

---



## **One store per person — the rule behind everything on this page**

Every store has a single **vendor ID**, and **a user can be linked to only ONE vendor ID — one store — at a time.** There is no “second store”: trying to add someone to a new store does nothing until they have been removed from the store they’re currently on.

This single rule explains everything else here:

- It’s why editing a role to `vendor_staff` is so disruptive — the account grabs a store link (the TUSA Store) and uses up its one and only slot.
- It’s why a user on the wrong store **must be removed from it first** before they can be linked to the right one.
- It’s why the automation (Organizer promotion, or the Team page) is the only safe way in — it manages that single slot for you.

If a person genuinely needs to work across two stores, that is **not possible with one account** — contact the dev team rather than reassigning them back and forth.

---



## **The two correct ways to connect someone to a club store**

Both of these run the automation that sets the store link (`_vendor_id`) to the **club president’s** store. Use either:



### **1. Promote them to Organizer in the club’s group (recommended for committee)**

- Go to the club’s **BuddyBoss group → Members**
- Promote the person to **Organizer**

That automatically:

- Gives them group organizer powers, **and**
- Adds them as store staff, linked to the **president’s** store

Demoting them from Organizer later removes that store access automatically.



### **2. Add them from inside the Store Manager → Team page (for non-committee helpers)**

Done by the club president or an existing staff member, from **their own account**:

- Log in to an account with access to **that club’s** store (president, club admin, or existing store staff)
- Go to **Profile → Store Management → Team**
- Use **Add Existing User** (or **Create New Staff**)

See the club-facing walkthrough: [Managing Store Staff](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/user-management/club-guide/managing-store-staff.md).

> Either path runs the webhook/automation that sets the store link correctly. The Edit User screen does not — there is no way to do this from wp-admin user editing.

---



## **Recovering a user who got attached to the wrong store**

If someone ended up on the wrong store — e.g. edited into `vendor_staff` on the Edit User screen and now stuck on the **TUSA Store** (`…/club-store/tusa`):

- **Remove them from the store they’re wrongly attached to.** Log in as a club admin / owner of **that** store (for the TUSA Store, a TUSA Store admin account), go to **Profile → Store Management → Team → Current Staff**, find them, and click **Remove from Store**. This clears their store link (`_vendor_id`) — it does **not** delete their account.
- **Demote them from Organizer** in the correct club’s group (**BuddyBoss group → Members**).
- **Re-promote them to Organizer.** This re-runs the automation and links them to the correct store (the club president’s).

> **Why demote *and* re-promote?** If they’re already an Organizer, promoting again does nothing — there’s no change for the automation to react to. And demoting alone won’t clear a store link that points at a *different* store. So you remove them from the wrong store first (step 1), then the demote → re-promote cycle (steps 2–3) cleanly re-fires the automation against the right store.

> A user can only hold **one** store link at a time, so the removal in step 1 must happen before they can be linked to their club’s store.

---



## **Quick reference**


| Situation | Do this |
| ----------------------------------------------------------- | --------------------------------------------------------------------------------------- |
| Add a committee member to the club store | Promote to **Organizer** in the club’s group |
| Add a one-off event helper (not committee) | President/staff add them via **Store Management → Team** |
| Exec shows as “Hire Store Customer” / “Club Admin” | Leave it — profile type is separate from store membership |
| You want to set `vendor_staff` on the Edit User screen | **Don’t** — it doesn’t link the store and attaches them to TUSA Store |
| User got stuck on the wrong store (e.g. `/club-store/tusa`) | Remove via **that store’s → Team**, then **demote + re-promote** them in the club group |


