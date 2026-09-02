---
title: Setting Up Store Products for Non-Club Entities
hide:
  - toc
---
# **etting Up Stores for Non-Club Entities**

Most stores on the site belong to **clubs**, and those are built automatically when a club is affiliated. But some stores belong to things that **aren’t clubs** and never go through affiliation — the Food Hub, Student Council, and other TUSA-run entities that come and go over time. Anything outside the club affiliation process is set up the way this page describes.

There is **no “create a store” button**. In this system a store is created by making a **new user** the **store owner** — once that user exists with the right role, the store exists too. Put simply: **the store-owner user *is* the store.**

This page walks through creating that user correctly. It’s the same process every time; only the names and email change for each entity.

> **Heads up before you start:** the **username** you choose becomes part of the store’s web address, and it’s awkward to change afterwards. Take a moment over it — the rest is straightforward.



## **The pattern**



In the WordPress dashboard, go to **Users → Add New** and fill in the new user using the values below. Set the password (or let WordPress generate one) as you would for any user, then click **Add New User**.


| Field | What to enter |
| -------------- | ---------------------------------------------------------------------------- |
| **Username** | The entity’s name (this drives the store’s web address — see the note below) |
| **First Name** | The entity name (first word) |
| **Last Name** | The entity name (remaining word/s) |
| **Email** | The entity’s **central, shared** address (not a personal one) |
| **Role** | **Vendor** |


That’s it — creating this Vendor user **creates the store**. But the store is created **without a name** — setting the store name is a separate manual step, and an essential one. Don’t skip the next part.

> **About the username and the store address:** the store’s web address is built from the username, so the store lives at an address based on whatever you enter there (WordPress tidies spacing and capitals when it makes the address). This is why the username matters and is worth getting right the first time — changing it later changes the store’s address too.

> **Always use a central, shared email — not a personal one.** Putting a shared address on the user means the store-owner login **and** that entity’s Stripe account both sit on one inbox the team can all reach, rather than being tied to one person who might move on. These entities drift in and out, so a shared address keeps the store usable regardless of who’s currently running it.



## **Worked example — the Food Hub**




| Field | What to enter |
| -------------- | --------------------------- |
| **Username** | `Food Hub` |
| **First Name** | `Food` |
| **Last Name** | `Hub` |
| **Email** | `food.hub@tusa.utas.edu.au` |
| **Role** | **Vendor** |


Other entities (Student Council, etc.) follow the same shape — their own name and their own shared address.



## **What happens next**



**Set the store name yourself — it is NOT created automatically, and it’s required.** Creating the Vendor user makes the store exist and builds the store’s web address from the username, but the store itself has **no name** until you add one by hand. An unnamed store can’t be recognised or matched to its group or Stripe account, so this step is essential. Go to **Dokan → Vendors**, find the vendor you just created, and set the **Store Name** to match the entity exactly (for the Food Hub, the store name is `Food Hub`). While you’re there, add the store **logo** and **banner** too. Leaving the store name blank is the single most common reason an entity store and its payments won’t link up. After that you can start adding items — see [Adding Products to Your Club Store](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/store-product-management/club-guide/adding-products.md), which works the same way for these stores.

**Why entities need all this by hand (and clubs don’t).** When a club is affiliated, the system wires the whole chain up automatically — store, name, Stripe account, connection. Entities never go through affiliation, so **every one of those steps is done manually for them**, and they have to line up exactly: the store name matches the entity, the email matches across the store and Stripe, and the Stripe account is connected to the store owner. Miss one and the store looks set up but won’t take payments.

**Connecting payments.** The entity’s **Stripe account** is set up and connected through the site (not through the Stripe dashboard — these are a special account type that can only be managed from our end). The full step-by-step, including connecting the account once the store exists, is in [Setting Up Club Stripe Accounts](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/store-product-management/setting-up-stores-for-non-club-entities/#stripe-account-setup) — see “Creating an account when there’s no store yet” and the **two-step** connection that follows it. If you’d rather we handle the Stripe side, create the store (named correctly) and **give us a yell**.



## **If something looks off**



If you don’t see a **Vendor** option in the Role dropdown, stop and flag it — don’t pick a different role to get past it.

If you’re unsure about the username before creating the user, ask first rather than guessing — it’s the one part that’s a hassle to undo.

Anything unexpected, drop a note on the task or [send it through](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/store-product-management/club-guide/reporting-issues.md) and we’ll sort it.