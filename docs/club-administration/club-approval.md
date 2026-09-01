---
title: Approving Club Applications
hide:
  - toc
---
# **Approving Club Applications**

This guide covers how to process club affiliation and reaffiliation applications.  
  
this is for testing

---

## **Policy vs Process**

**Important distinction:**


| Type | Who Decides | Examples |
| ----------- | ----------------------- | ------------------------------------------------------------- |
| **Policy** | TUSA internal direction | Whether a club meets affiliation criteria, required documents |
| **Process** | What this guide covers | Where to find applications, what gets created automatically |


This guide covers **the process only**. Whether to approve or reject a club application is an internal decision — refer to your manager or the club affiliation policy documents.

---

## **Before an Application: EOI and Club Officer Meeting**

**Important:** Clubs cannot submit an affiliation application directly. There is a required step first:

- **Expression of Interest (EOI)** — The club submits an EOI form
- **Meeting with Club Officer** — TUSA Club Officer contacts them to arrange a meeting
- **Application invited** — After the meeting, the club is invited to submit their full application

This means by the time you see an application in the system, the club has already met with a Club Officer and been given the go-ahead to apply.

---

## **Types of Applications**


| Type | What It Is | Key Difference |
| ------------------- | ------------------------------------------ | --------------------------------------------------- |
| **New Affiliation** | Brand new club applying for the first time | Creates everything fresh — group, store, accounts |
| **Reaffiliation** | Existing club renewing for a new year | Updates existing records, doesn’t create duplicates |


Both come through the same workflow, but the system handles them differently behind the scenes.

---

## **Finding Applications**

### **Your Workflow Inbox**

**Where:** Profile avatar → Profile → Workflow Inbox tab  
**Direct URL:** `/my/workflow-inbox/`

This shows applications **assigned to you** for action. If you’re in the clubs admin team, new applications will appear here.

### **TUSA Internal Group**

**Where:** `/clubs/clubs-index/tusa-internal/` → **Functions** tab


| Sub-tab | What’s Here |
| -------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Club Affiliations** (`/functions/affiliation/`) | Every affiliation and reaffiliation application, with its status. **This is where you find an application by club name** and see whether it’s pending or approved. |
| **Re/Affiliation Processing** (`/functions/processing/`) | The **live setup that runs after you approve** an application: it shows each step (store, group, tags, and so on) and whether it succeeded. It is not a queue of applications waiting for review. See *Watching Setup Progress*, below. |
| **Club Admin Rolodex** | Contact details for all club admins |


---

## **Processing a New Club Application**

### **Step 1: Review the Application**

Open the application from your workflow inbox or the Functions tab.

**Check the basics:**


| Item | What to Look For |
| ----------------------- | --------------------------------------------- |
| **Club name** | Appropriate, not duplicating an existing club |
| **Acronym** | Sensible abbreviation (used for usernames) |
| **Description** | Clear explanation of club purpose |
| **Constitution** | Document uploaded |
| **Meeting minutes** | Document uploaded |
| **Member list** | Document uploaded |
| **Executive committee** | President and other officers listed |
| **Contact details** | Phone, email, student IDs provided |


### **Step 2: Check Documents**

The application includes uploaded documents. Verify:

- Documents are readable (not corrupted/blank)
- Constitution meets requirements (per policy)
- Member list has the required number of members

**Where to see documents:** Click document links in the application, or check TUSA Internal → **Documents** tab.

### **Step 3: Approve or Return**

**If everything looks good:**

- Assign yourself as the reviewing admin (if required)
- Click Approve in the workflow

**If issues need fixing:**

- Use “Return for Amendment” to send back to the applicant
- They’ll receive a notification to fix and resubmit

### **What Happens After Approval**

When you approve a new club, the system automatically creates:


| Item | What Gets Created |
| ---------------------- | --------------------------------------------------------------------------------------------------------------------------- |
| **Club group** | The private club group |
| **President account** | Login for the club president |
| **Committee accounts** | Logins for other executive members |
| **Club store** | The public store, created disabled. A Clubs Super Admin switches it on to sell once the club’s set up and ready (see below) |
| **Startup grant** | Automatic grant application for new club funding |
| **Membership tags** | The tags that grant club access (this year plus the next two years) |


**You don’t need to create any of this manually** — it all happens automatically.

### **Watching Setup Progress**

After you click Approve, you’ll see a confirmation message with a link to the **[Club Setup Status](https://tusa-dev.its.utas.edu.au/clubs/clubs-index/tusa-internal/functions/processing/)** dashboard. Click it to watch the setup happen in real time.

The dashboard shows a card for each setup with a step-by-step checklist:

- **President Setup** — Create or update the president’s account
- **Dokan Store** — Create the club’s store
- **BuddyBoss Group** — Create the club group
- **Group Media** — Set group avatar and cover image
- **Committee** — Add executive committee members
- **Membership Tags** — Create the club’s membership tags (this year and the next two years)
- **Stripe Account** — Create the club’s Stripe connected account (new affiliations only)

Each step shows a checkmark when complete, a cross if it failed, or “skipped” if it wasn’t needed. You’ll also receive an email at clubs@ when the setup finishes (or if it fails).

**Dashboard actions:**

- **Retry** — re-runs the full setup if it failed or stalled (safe to run multiple times)
- **Delete** — removes the record from the dashboard (does not undo any setup that already happened)

**If you want to verify manually** in the site admin:


| Check | Where to Look |
| -------------------- | --------------------------------------- |
| Group exists | Site admin → Groups → search club name |
| President can log in | They should receive a login email |
| Store created | Site admin → Vendors → search club name |
| Startup grant | TUSA Internal → Grants tab |
| Documents in library | TUSA Internal → Documents tab |


---

## **Switching a club’s store on to sell**

When you approve a club, its store is created automatically but starts **disabled**. It won’t appear in the stores list or take any payments until it’s switched on to sell.

That switch is done by a **Clubs Super Admin**, because it needs back-end access, and it’s manual on purpose: before a store goes live, a person confirms everything’s in place and that the club is genuinely ready to launch its store and group. It’s the final readiness check, not a rubber-stamp. Until it’s flipped, the store is fully built but not yet live, which is why an approved club may not be showing in the stores list yet.

### **How to switch a store on**

- Go to **Dokan → Vendors** (`/wp-admin/admin.php?page=dokan-dashboard#/vendors`).
- Find the club’s store (its status shows as **Disabled**).
- Click the **three-dots menu** (⋮) and choose **Approve vendors**.

The store is now **Enabled**: it appears in the stores list and can take sales.

### **Taking a store back down**

Click the same **three-dots menu** and choose **Disable selling**.

> **Important:** disabling doesn’t just hide the store; it removes its ability to sell entirely. Only disable one you genuinely want taken offline, not one you want tidied out of a list.

---

## **Processing a Reaffiliation**

Reaffiliations are for **existing clubs** renewing for a new year.

### **Key Difference from New Clubs**

The system **updates existing records** rather than creating new ones:


| New Club | Reaffiliation |
| ----------------------------- | --------------------------------------- |
| Creates new group | Uses existing group |
| Creates new president account | Updates existing president’s details |
| Creates new store | Updates existing store |
| Creates everything fresh | Preserves history, updates for new year |


### **Step 1: Review the Application**

The reaffiliation form pre-populates with existing information. Check that:


| Item | What to Verify |
| --------------------- | -------------------------------------------------- |
| **Club name** | Still correct (or updated appropriately) |
| **Affiliation year** | Correct new year selected |
| **President details** | Current president’s information |
| **Committee members** | List of current executive (pulled from the system) |
| **Updated documents** | New constitution / minutes if required |


### **Step 2: Committee Member Changes**

The form shows the current committee. The club may have:

- Kept the same people
- Added new members
- Removed departed members

**After approval:**

- New members get added as group admins
- Departed members get demoted (not deleted — they keep their account)
- The president account stays the same (only their profile details update)

### **Step 3: Approve or Return**

Same as new clubs:

- **Approve** if everything is in order
- **Return for Amendment** if changes are needed

### **What Happens After Approval**


| Item | What Happens |
| --------------------- | -------------------------------------------- |
| **Group** | Stays the same (no duplicate created) |
| **President account** | Profile details updated to the new president |
| **Committee** | Members added or removed as specified |
| **Store** | Details updated if changed |
| **Membership tags** | New year tags created |
| **Documents** | New uploads added to the library |


### **Watching Reaffiliation Progress**

After you click Approve, you’ll see a confirmation message with a link to the **[Club Setup Status](https://tusa-dev.its.utas.edu.au/clubs/clubs-index/tusa-internal/functions/processing/)** dashboard. Click it to watch the reaffiliation happen in real time.

The reaffiliation checklist includes:

- **Membership Tags** — Create the club’s membership tags for the new year
- **Find Group & President** — Locate the existing club group
- **Process Logo** — Update logo if changed
- **Process Banner** — Update banner if changed
- **President Profile** — Update the president’s profile details
- **Club Store** — Update store details
- **Group Media** — Update group avatar and cover
- **Committee** — Add or remove committee members
- **User Avatars** — Update profile photos
- **President Member Type** — Set the correct member type

Steps that aren’t needed (e.g., logo unchanged) show as “skipped”.

---

## **Common Issues**

### **“I can’t find the application”**

**Check:**

- Is it assigned to you? Check your workflow inbox (it lists items by form, date and id, not by club name, so match by the date)
- Are you in the right role? You need clubs admin permission
- Look in TUSA Internal → Functions → **Club Affiliations**, which lists every application by club name and status

### **“The setup seems stuck” or “Something didn’t get created”**

The **[Club Setup Status](https://tusa-dev.its.utas.edu.au/clubs/clubs-index/tusa-internal/functions/processing/)** dashboard will tell you exactly what happened.

**What you’ll see:**


| Status | Meaning | What to Do |
| -------------------- | ---------------------------------- | ----------------------------------- |
| **Complete** (green) | Everything worked | Nothing — you’re done |
| **Failed** (red) | A specific step broke | Click **Retry** to re-run the setup |
| **Stalled** (red) | Process timed out before finishing | Click **Retry** to re-run |


The dashboard shows which step failed and an error message. Retrying is safe — the system won’t create duplicates.

You’ll also receive an email at clubs@ if something fails, so you don’t need to check the dashboard after every approval.

**If the dashboard doesn’t help:**

- The club can be manually created via Functions → Add a Club
- See [Reporting an Issue](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/club-administration/approving-club-applications/#reporting-issues) — send the error details from the dashboard

### **“Documents aren’t showing in the library”**

**Check:**

- TUSA Internal → Documents tab — search for club name
- If missing, documents may need to be re-uploaded
- Check the original application still has the files attached

### **“President can’t log in”**

**Common cases:**

- Email went to spam
- They’re using the wrong email address
- Password reset needed

**Fix:**

- Site admin → Users — find the president account
- Trigger a password reset email
- Verify their email address is correct

### **“Duplicate club group appeared”**

This shouldn’t happen with reaffiliation, but if it does:

- Don’t delete either group without checking first
- See [Reporting an Issue](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/club-administration/approving-club-applications/#reporting-issues) — send details so the duplicate can be merged or fixed

---

## **Quick Reference: Where Things Live**


| Need to Find | Where to Go |
| --------------------------- | --------------------------------------------------------------------------------------------------------------------- |
| Applications to process | Your workflow inbox |
| Setup progress and errors | [Club Setup Status dashboard](https://tusa-dev.its.utas.edu.au/clubs/clubs-index/tusa-internal/functions/processing/) |
| All club affiliations | TUSA Internal → Functions → Club Affiliations |
| Club contact details | TUSA Internal → Functions → Club Admin Rolodex |
| Club documents | TUSA Internal → Documents tab |
| Club grants | TUSA Internal → Grants tab |
| Individual club’s dashboard | `/clubs/clubs-index/{club-name}/` |


