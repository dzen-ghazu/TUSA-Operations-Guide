---
title: Setting Up Food Hub People
hide:
  - toc
---
# **Setting Up Food Hub People**

This guide is for TUSA staff who set people up on the Food Hub. There are two jobs it covers:

- **Setting up a new Food Hub admin** — someone who will run the rosters (put up shifts, add and remove volunteers).
- **Adding a volunteer** — someone who works shifts but doesn’t run the hub.

> **The one thing to remember:** you add someone to the Food Hub by adding them to the **Food Hub group**. That’s what sets them up in the shift system behind the scenes. You don’t set anything up in the shift system by hand — adding them to the group does it for you.

---



## **Who can do this**



Setting up a **new Food Hub admin** is a back-end job — it needs a **site admin, a clubs super, or a content admin**. If that’s not you, ask one of them.

Adding a **volunteer** to the hub is done by a **Food Hub group organiser**, from the Food Hub group. You don’t need back-end access for that part.

---



## **Part 1 — Setting up a new Food Hub admin**



**This is a back-end job — you do it in wp-admin, not from the front-end group page.** It needs a site admin, a clubs super, or a content admin. A Food Hub admin needs two things: the right **role**, and to be an **organiser of the Food Hub group**. Do both, in wp-admin.



### **Step 1: Give them the Food Hub Admin role**



- In wp-admin, go to **Users** and find the person.
- Edit them, and give them the **Food Hub Admin** role.
- If they already have other roles, leave those as they are — just add this one.

That role is what grants the ShiftController permissions to run the shift calendar and manage the hub — being in the group alone won’t do it. That’s why you do both this and the group step below.



### **Step 2: Add them to the Food Hub group as an organiser — in wp-admin**



Do this from the back end, **not** the group’s front-end “Manage → Members” tab:

- In wp-admin, go to **BuddyBoss → Groups**.
- Find the **Food Hub** group, click the **three dots (⋮)** beside it, and choose **Edit**.
- Open the **Members** section.
- In the **Add New Members** field, search for the person and click **Add**. That adds them as a regular member.
- Click the person’s **member box**, change the role to **Organizer**, and click the orange **Save** button.

> **Why the back end, and not the group’s own “Manage → Members” tab?** That front-end tab only works if you are **already** an organiser inside the group — so it can’t be used to add someone who isn’t in the group yet, including re-adding yourself if your membership was ever removed. The wp-admin route above works either way, which is why setting up (or re-adding) an organiser is always a back-end job. Once someone *is* an organiser, they can use the front-end tab to add volunteers (Part 2).

That’s it — role plus organiser of the group. Nothing else needs setting up. Once that’s done, point them at the [Food Hub Rosters](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/food-hub/setting-up-food-hub-people/#managing-food-hub-rosters) guide so they know how to run shifts and volunteers.

---



## **Part 2 — Adding a volunteer to the hub**



Once someone is ready to volunteer, you add them to the Food Hub so they can be rostered. A **Food Hub group organiser** does this from the Food Hub group.

Before you start:

- The person must already have an account on the website. If they don’t, they make one at the login page first.
- Their induction and onboarding happen in **Employment Hero**, not on the website. The website just gets them ready to be rostered.

To add them:

- Go to the **Food Hub group** and open the **Add a member** tab.
- Start typing their name or email, and pick them from the list.
- Click **Add**.

That sets them up in the shift system behind the scenes. Afterwards you’ll get a message telling you they still need to be put on a calendar, with a link. Follow that link, find the person, and in the **Calendar** column click **Edit** next to their name to add them to the right Food Hub calendar. Once they’re on a calendar, they can pick up shifts there.

So the order is always: they’re onboarded in Employment Hero first, then you add them to the group, then you put them on their calendar.

---



## **If something looks wrong**



- **You can’t find the person to add.** They need an account on the website first. Ask them to make one at the login page, then add them.
- **A new Food Hub admin can’t see the shift calendar.** Their setup probably isn’t complete — check they have the **Food Hub Admin** role (Part 1, Step 1). If it still doesn’t work after that, contact the dev team.
- **You don’t have the access to set up a new admin.** That part needs a **site admin, a clubs super, or a content admin**. Ask one of them to do Part 1 for you.

---



## **Related Guides**



- [Food Hub Rosters](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/food-hub/setting-up-food-hub-people/#managing-food-hub-rosters) — the day-to-day: putting up shifts, adding and removing volunteers, seeing who’s coming.

