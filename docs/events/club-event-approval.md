---
title: Approving Club Events
hide:
  - toc
---
# **Approving Club Events**

This guide covers **system requirements** for event approval – the technical things that need to be right for events to display correctly on the website.

---



## **Policy vs System**



**Important distinction:**


| Type | Who Decides | Examples |
| ---------- | ----------------------- | ----------------------------------------------------------------------------- |
| **Policy** | TUSA internal direction | What makes an event approvable, risk thresholds, approval criteria |
| **System** | Technical requirements | Categories for filtering, required fields, how the automated publishing works |


This documentation covers **system requirements only**. How events and risk assessments are approved is largely up to internal direction from TUSA. When in doubt about approval decisions or processes, **ask your manager for clarification**.

---



## **Overview**



Events submitted through the risk assessment and event application process need to be reviewed before publication.

**Important:** Club events are **never published directly**. They are always created as **drafts** first. The event only becomes published automatically when the application is approved through the workflow.

Before approving, staff should verify the event is properly configured in the system – especially categories.

---



## **The Approval Process**



&nbsp;

### **Workflow**



&nbsp;

```
Club submits the risk assessment and event application
    ↓
TUSA staff reviews application
    ↓
Staff checks draft event (link in form submission)
    ↓
If issues found → Return for amendment
    ↓
If ready → Approve in the workflow
    ↓
Step 90: Event is automatically published
    ↓
Event status changes: draft → publish

```



&nbsp;

### **Accessing Draft Events**



The event application includes a link to the draft event:

- A link to the draft event listing
- Click this to open the event and review details

---



## **Seeing ALL Events (Important)**



There are two different “Events” screens in the admin, and they show **different things**. This catches people out constantly, so it’s worth knowing which is which.


| Screen | How you get there | What it shows |
| -------------------------------------------- | ---------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Eventin dashboard** (the fancy one) | Clicking **Events / Eventin** in the left admin menu | A limited, paginated view in Eventin’s own interface. It only shows a handful at a time and is awkward to search — **this is NOT the full list.** |
| **WordPress events list** (the complete one) | The address below | **Every** event — drafts and published — with proper search, status tabs (All / Published / Draft), and bulk actions. |


**To see and manage every event, use this address:**



```
/wp-admin/edit.php?post_type=etn

```



(Full link on the dev site: `https://tusa-dev.its.utas.edu.au/wp-admin/edit.php?post_type=etn`)

**Bookmark it.** The left-hand menu’s “Events” link sends you to the Eventin dashboard, not this list, and there’s no obvious button to get here — so the address bar (or a bookmark) is the reliable way.

**Use this screen when you need to:**

- See the true total number of events (top of the list shows e.g. “All (43)”)
- Find a specific event that isn’t showing in the Eventin dashboard
- Bulk-select events to trash (e.g. clearing out old test events)
- Filter by Draft vs Published using the status tabs

> **Tip:** Use **Screen Options** (top-right of the list) to increase how many events show per page if you have a lot of them.

> **Frontend Store Manager (clubs and entities):** Presidents and entity managers who work in the frontend Store Manager rather than the site admin find their drafts a different way. In **Store Manager → Events**, click **Filter** and set **Status** to **Draft**, and their own draft events appear. (The default Events list shows published events only, which is why a newly saved draft can look like it has vanished.)

---



## **Pre-Approval Checklist**



&nbsp;

### **1. Event Categories – CRITICAL**



**Why this matters:** Categories control where events appear on the website. If categories are wrong or missing:

- Event won’t show up in filtered views
- Event won’t appear on special pages (UTE, Online, Shut Up & Write, etc.)
- Campus filters won’t work correctly

**Check the** `etn_category` **taxonomy is set correctly:**


| If the event is… | Must have category… | What happens if missing |
| ------------------------- | ----------------------------- | ------------------------------------ |
| On a specific campus | Campus name (Sandy Bay, etc.) | Won’t show when filtering by campus |
| A UTE event | UTE | Won’t appear on UTE events page |
| An online event | Online | Won’t appear in online events filter |
| A Shut Up & Write session | Shut Up & Write | Won’t appear on SUW page |
| A Food Hub event | Food Hub | Won’t appear on Food Hub events |


**How to fix:**

- Edit the draft event
- Find the Categories section
- Select appropriate categories
- Save/Update



### **2. Event Details**



Verify basic information is complete:


| Check | What to Look For |
| --------------- | ------------------------------------- |
| **Title** | Clear, descriptive event name |
| **Date/Time** | Correct start and end dates/times |
| **Location** | Venue specified (or marked as online) |
| **Description** | Adequate event description |
| **Image** | Featured image uploaded |


### **3. Tickets (if ticketed event)**




| Check | What to Look For |
| -------------------- | ------------------------------------------------ |
| **Ticket types** | Appropriate variations (member/non-member, etc.) |
| **Pricing** | Prices look reasonable |
| **Capacity** | Global capacity set if venue has limits |
| **Tag restrictions** | Correct membership tags if members-only |


### **4. Organiser Information**




| Check | What to Look For |
| ------------- | ---------------------------- |
| **Organiser** | Correct club/entity selected |
| **Contact** | Contact details included |


### **5. Stall Applications – Indoor vs Outdoor**



**Temporary stall applications are for outdoor stalls only.**


| Location | Process |
| ------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Outdoor** (courtyards, lawns, outdoor walkways) | TUSA approves via the event application |
| **Indoor** (foyers, atriums, indoor common areas) | UTAS Campus Services books via [venue hire form](https://www.utas.edu.au/__data/assets/pdf_file/0005/1661270/Contract-for-hire-of-University-venues-and-events.pdf) |


If a club submits a stall application for an indoor location:

- Return for amendment
- Direct them to contact UTAS Campus Services for indoor booking
- They may still need a TUSA event application for food/activities, but indoor space is booked separately

---



## **Common Issues**



&nbsp;

### **“Template selector is missing” when creating an event or ticket**



**Symptom:** In the event creation page (Advanced section), there’s no longer an option to select an **event template** or a **ticket template**.

**This is not a problem — ignore it.** Both the **event display template and the ticket template are pre-set and locked at the site level**, not chosen per-event in Eventin. The site templates are used for every event and ticket regardless of whether Eventin shows a selector — and if a selector appears empty, that’s expected. There is nothing to fix, choose, or change here. Staff and club admins do not need to do anything with templates.



### **Missing Campus Category**



**Symptom:** Event doesn’t appear when users filter by campus location.

**Cause:** Event has location set but no campus category assigned.

**Fix:** Add the relevant campus category (Sandy Bay, Newnham, Cradle Coast, etc.).



### **Missing Program Category**



**Symptom:** Event doesn’t appear on program-specific pages.

**Cause:** UTE/SUW/Food Hub events without appropriate category.

**Fix:** Add the program category in addition to any campus categories.



### **Online Event Without Category**



**Symptom:** Online event doesn’t appear in online events filter.

**Cause:** Event marked as online but missing Online category.

**Fix:** Add “Online” category.



### **Multiple Categories**



Events can (and often should) have multiple categories:

- A UTE event at Sandy Bay should have both “UTE” AND “Sandy Bay”
- An online SUW session should have both “Online” AND “Shut Up & Write”

---



## **Fixing Issues Before Approval**



If system issues need fixing (missing categories, incorrect details), you have two options:

**Option 1: Fix it yourself**

- Open the draft event (link on the application)
- Make the necessary changes (add categories, fix dates, etc.)
- Save the event
- Then approve the application

**Option 2: Return for amendment**

- Use the workflow’s Return for Amendment option
- Club receives notification to fix their submission
- They edit and resubmit

**When to use which:** Minor system fixes (adding a missing category) are often quicker to do yourself. Larger issues or things the club needs to clarify should go back to them.

**Note:** Whether to approve, return, or reject an application based on risk assessment or policy grounds is an internal decision – refer to your manager or internal guidelines.

---



## **Equipment Hire Orders**



Clubs place equipment hire orders directly through the Hire Store before submitting their event application — the order number is recorded on their event application in the hire order number field. A 100% discount coupon auto-applies at checkout for eligible users (club presidents, club admins, TUSA staff), so club orders complete at $0 with stock reserved.

When you review an event application, you also decide what happens to the linked hire order — leave it at $0, adjust the price and invoice the club, or cancel it if the event isn’t approved.

**Full walkthrough of the staff workflow:** [Handling Club Hire Orders](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/events/approving-club-events/handling-hire-orders.md).

---



## **Manual Orders for External Parties**



Sometimes external organisations (NFPs, general public) need to hire equipment outside of the normal club event flow. These require manual order creation with custom discounts.



### **Who Gets Discounts?**




| Customer Type | Discount | Notes |
| -------------------------------- | ------------------ | ----------------------------------------------------------- |
| **Affiliated clubs** | 100% auto-discount | Handled automatically via club ordering |
| **External NFPs at TUSA events** | Case-by-case | e.g., NFP with stall at Student Life Expo – discount varies |
| **General public** | Usually none | Rare exceptions by prior arrangement |


**Policy note:** NFP discounts for externals are offered on a case-by-case basis, typically when they’re attending a TUSA event and paying a stall fee. Bron handles invoicing for external hire related to her events. Discount rates vary depending on the organisation.



### **Creating a Manual Order**



Since guest checkout is not enabled, you must first create a customer account (if they’re new), then create an order for them.



#### **Step 1: Create Customer Account (New Customers Only)**



**If the customer has never ordered before**, a TUSA admin must create their account:

- Go to **Users → Add New** in the site admin
- Enter the customer’s details:

– **Username:** Their email address (or something memorable)  
– **Email:** Their email address (required for invoice)  
– **First Name / Last Name:** Customer’s name  
– **Role:** Customer

- Click **Add New User**
- **Note:** You can skip the password – they’ll use the password reset link if needed

**Important:** Club vendors cannot create new user accounts — that requires site admin access. Once the customer exists, vendors can create orders for them.



#### **Step 2: Create the Order**



**Option A: TUSA Admin (site backend)**

- Go to **Orders → Add New** in the site admin
- Click **Add Order**
- **Customer:** Search for and select the customer
- **Add items:**

– Click “Add item(s)”  
– Click “Add product(s)”  
– Search for the hire products needed  
– Select quantities  
– Click “Add”

- **Set dates:** Ensure hire dates are set correctly on each item
- **Billing/Shipping:** Fill in or update billing details from customer info

**Option B: Vendor (frontend dashboard)**

Vendors can create manual orders from **Vendor Dashboard → Orders → New Orders**.

Vendors can:

- Select from their existing customers (customers who’ve previously ordered from their store)
- Add their own products to the order
- Update billing and shipping details
- Add order notes

**Note:** It’s unclear whether vendors can search all site users or only customers who’ve previously ordered from their store. If a vendor can’t find a newly-created user, admin should create the order via the site backend instead.



#### **Step 3: Apply Discount**



**Option A: Percentage discount**

- Click “Apply Coupon” (if you have a coupon code set up)
- Or manually adjust line item prices

**Option B: Manual price adjustment**

- Click the pencil icon next to each line item
- Change the price to the discounted amount
- Click “Save”

**Option C: Add a fee (negative)**

- Click “Add fee”
- Enter a negative amount (e.g., -$20.00)
- Name it “NFP Discount” or similar
- Click “Save”



#### **Step 4: Send Invoice**



- Make sure the order status is **Pending Payment**
- In the **Order Actions** dropdown (right side), select:

– **“Email invoice / order details to customer”**

- Click the **arrow button** (or Update) to send

The customer receives an email with a link to pay online. Payment updates the order status automatically.



### **What the Customer Sees**



- Email with invoice details and “Pay Now” link
- Links to their account where they can view and pay the order
- If they don’t have a password, they can use “Lost password” to set one



### **Tracking External Hire Orders**



External hire orders can be identified by:

- No club association
- Customer is general “Customer” role (not Club Admin)
- May have manual discount notes

Consider adding an order note documenting why the discount was applied (e.g., “NFP discount – SLE 2026 stallholder”).

---



## **After Approval**



Once you approve the event application:

- Webhook fires automatically
- Event status changes to Published
- Event appears on website (with correct categories → correct pages)
- Club receives notification of approval



### **If Event Doesn’t Appear**



Check:

- Was the event actually published? (View in the site admin)
- Are the categories correct? (See filtering issues above)
- Is the event date in the future? (Past events may not show)
- If the event is published with correct categories but still missing from filtered pages, see [Reporting an Issue](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/events/approving-club-events/#reporting-issues) — there may be a category index that needs rebuilding

---



## **Category Reference**



**Categories determine which facets (filters) an event appears under.** Getting these right is critical for discoverability.



### **Campus Categories (Event Campus)**



These control the campus location filter:


| Category | Use For |
| ------------------- | ------------------------------- |
| Sandy Bay Campus | Events at Sandy Bay |
| Hobart City Campus | Events in Hobart city |
| Inveresk Campus | Events at Inveresk (Launceston) |
| Cradle Coast Campus | Events at Cradle Coast |
| Rozelle Campus | Events at Rozelle (Sydney) |
| Online | Online/virtual events |


**Multiple campuses:** Hybrid events should have BOTH the physical campus AND “Online” selected.



### **Event Type Categories (Event Category)**



These determine the event type and where it appears:


| Category | Use For | Appears On |
| ------------------------------- | ------------------------ | ---------------- |
| Club Events | Standard club activities | Main events grid |
| TUSA Events | TUSA-organised events | Main events grid |
| Food Hub | Food Hub activities | Food Hub page |
| UTE (Unique Tassie Experiences) | UTE program | UTE page |
| Training and Workshops | Educational sessions | Main events grid |


### **Special Categories**




| Category | Use For | Appears On |
| ---------------------- | ---------------------- | ----------------- |
| Shut Up and Write | Writing/study sessions | SUW page |
| Orientation | O-Week events | Orientation pages |
| Post Graduate Students | Postgrad-specific | Postgrad pages |


**Critical:** Without the correct category, the event won’t appear on that program’s dedicated page, even if all other details are correct.



### **Checking Categories in Bulk**



To audit event categories: **Events → All Events** in the site admin. You can filter by category and see which events are missing categories.

---



## **Related Guides**



- [Approving Club Applications](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/events/approving-club-events/#approving-clubs) — Affiliation and reaffiliation
- [Reporting an Issue](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/events/approving-club-events/#reporting-issues) — When something on the site isn’t working

