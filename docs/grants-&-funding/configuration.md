---
title: Configuring Grants
hide:
  - toc
---
# **Configuring Grants**

This guide explains how to set up and maintain grant programs – the configuration that determines what applicants see and what evidence they need to provide.

---



## **How the Grants System Works**



&nbsp;

### **The Three Forms**



The grants system uses three interconnected pieces:



```
┌─────────────────────────────────────────────────────────────────────┐
│                    SETUP FIRST (Master Lists)                       │
├─────────────────────────────┬───────────────────────────────────────┤
│  GRANT REQUIREMENTS         │  GRANT CAPS                           │
│                             │                                       │
│  Master list of ALL         │  Spending limit templates             │
│  possible requirements      │  that can be attached to grants       │
│                             │                                       │
│  • Requirement name         │  • Cap name (e.g., "Venue Hire")      │
│  • Documentation needed?    │  • Dollar maximum                     │
│  • Evidence collection      │  • Percentage cap                     │
│    method                   │  • Per person limit                   │
│                             │  • Conditions                         │
└──────────────┬──────────────┴───────────────────┬───────────────────┘
               │                                  │
               │      THEN CONFIGURE GRANTS       │
               ▼                                  ▼
┌─────────────────────────────────────────────────────────────────────┐
│                          GRANT DETAILS                              │
│                                                                     │
│  Each grant program picks from the master lists:                    │
│                                                                     │
│  • Grant name, description, dates                                   │
│  • Which REQUIREMENTS apply (from the requirements list)            │
│  • Which CAPS apply (from the caps list)                            │
│  • Overall cap settings                                             │
└─────────────────────────────────────────────────────────────────────┘

```



&nbsp;

### **The Order of Operations**



**Important:** You must create requirements and caps BEFORE you can select them on a grant.


| Step | What to Do | Where |
| ---- | ------------------------------ | ----------------------- |
| 1 | Create any needed requirements | Grant Requirements list |
| 2 | Create any needed sub-caps | Grant Caps list |
| 3 | Create/configure the grant | Grant Details |
| 4 | Tick which requirements apply | Inside the grant entry |
| 5 | Link which caps apply | Inside the grant entry |


If you try to configure a grant and the requirement or cap you need doesn’t exist in the dropdown/checkboxes, you need to create it in the master list first.



### **The Big Picture**



&nbsp;

```
GRANT DETAILS                    GRANT REQUIREMENTS
┌─────────────────────────┐      ┌──────────────────────────────┐
│ • Grant name            │      │ Master list of ALL possible  │
│ • Description           │      │ requirements across all      │
│ • Opens/closes dates    │      │ grants                       │
│ • Caps and limits       │      │                              │
│ • Which requirements    │◄────►│ Each requirement defines:    │
│   apply to THIS grant   │      │ • What evidence is needed    │
│   (checkboxes)          │      │ • How to provide it          │
└─────────────────────────┘      └──────────────────────────────┘

```



**Key concept:** Requirements and caps exist in master lists. Each grant “picks” which ones apply by ticking checkboxes or linking entries.



### **Why It’s Built This Way**



Many requirements apply to multiple grants. Instead of entering “Two quotes required for items over $500” nine times (once per grant), you enter it once in the requirements list, then tick it on each grant that needs it.

This also means:

- If you update a requirement’s wording, it updates everywhere
- If a requirement isn’t ticked on ANY grant, it won’t appear anywhere
- You can add new requirements without editing every grant



### **What Applicants See**



When a club submits an application:

- They select a grant from the dropdown (only shows currently open grants)
- The grant description displays so they can confirm they chose correctly
- **Requirements automatically appear** based on what’s ticked for that grant
- **Caps and limits automatically appear** based on that grant’s configuration
- They complete the form with all required evidence

---



## **Where to Find Everything**



&nbsp;

### **Grant Details (Configure Each Grant)**



**Location:** TUSA Internal → Grants tab → Current Grants

Each entry here is one grant program. Click into a grant to configure it.



### **Grant Requirements (Master List)**



**Location:** TUSA Internal → Grants tab → Grant Requirements

This is the master list of all possible requirements. Create entries here FIRST, then tick them on grants.



### **Grant Caps (Master List)**



**Location:** TUSA Internal → Grants tab → Grant Caps

This is the master list of spending limit categories. Create sub-cap entries here FIRST, then link them to grants.

**Note:** Overall caps (the total grant limit) are set directly on the grant. Sub-caps (limits on specific expense categories like “Venue Hire” or “Catering”) come from this list.

---



## **Configuring a Grant**



&nbsp;

### **Step 1: Open the Grant**



- Go to TUSA Internal → Grants → Current Grants
- Click on the grant you want to configure
- You’ll see the Grant Details form



### **Step 2: Review Basic Information**




| Field | What It Does | Tips |
| --------------------- | ----------------------------------------------------- | ------------------------------------------------------------------------------------------------------- |
| **Grant Name** | Appears in the dropdown and on the public grants page | Keep it clear; include the year if time-limited (e.g., “Balls & Annual Dinners Grant 2026”) |
| **Grant Description** | Explains what the grant is for | Write in plain English that students understand. Explain who it’s for, what it covers, and key criteria |
| **Opens** | When applications open | Grant won’t appear in dropdown before this date |
| **Closes** | When applications close | Grant won’t appear in dropdown after this date |


**Note:** Entry ID 1345 is “Always Open” and doesn’t need dates.



### **Step 3: Configure Caps and Limits**



Caps control the maximum funding applicants can request.



#### **Cap Type Options**




| Option | When to Use |
| -------------------------------------- | ------------------------------------------------------ |
| **None** | No spending limits for this grant |
| **Overall limit (% or dollar)** | One cap for the entire grant |
| **Overall limit with sub-item limits** | Overall cap PLUS specific limits on expense categories |


#### **If Using Overall Limit**




| Field | What to Enter |
| ----------------------- | ------------------------------------------------------- |
| **Cap Type** | Choose “Dollar Amount” or “Percentage of claim” |
| **Grant Overall Cap $** | If dollar: enter the maximum (e.g., 1500.00 for $1,500) |
| **Grant Overall Cap %** | If percentage: enter the number (e.g., 50 for 50%) |


#### **If Using Sub-Item Limits**



Sub-caps let you set limits on specific expense categories. Each sub-cap entry includes:


| Field | Example |
| --------------------- | ------------------------------------------ |
| **Cap Name** | “Venue Hire”, “Catering”, “Transport” |
| **Cap Dollar Amount** | Maximum dollars for this category |
| **Cap %** | OR percentage of this expense type covered |
| **Cap Per Person** | Per-attendee limits if applicable |
| **Cap Conditions** | Any special notes or conditions |


### **Step 4: Select Requirements (Critical!)**



This is the most important configuration step. The **Prerequisites/Requirements** field is a list of checkboxes.

**Tick each requirement that applicants for THIS grant must meet.**

Ask yourself: “When I’m assessing a Balls & Annual Dinners application, what information do I need to make a decision?”

Whatever you need to see should be ticked.



#### **How Requirements Work**



When you tick a requirement:

- It appears in a yellow “Evidence Required” box on the application form
- The box shows HOW to provide evidence (upload, text input, acknowledgement, etc.)
- Applicants complete the relevant fields

When you DON’T tick a requirement:

- It won’t appear for this grant
- Applicants won’t be asked for it



#### **Example**



If “Balls & Annual Dinners Grant 2026” has these ticked:

- Club contribution amount must be specified

- Ticket pricing must cover food costs

- Final budget breakdown/claim required

Applicants will see exactly those three items in their “Evidence Required for This Grant” section.



### **Step 5: Save**



Save your changes. The grant is now configured.

---



## **Managing the Requirements List**



&nbsp;

### **Understanding Requirements**



Each requirement in the master list defines:


| Field | Purpose |
| ------------------------------ | ---------------------------------------------------------- |
| **Requirement Name** | What applicants see (must be clear and concise) |
| **Documentation Required?** | Yes = they need to provide evidence; No = just information |
| **Evidence Collection Method** | HOW they provide evidence |


### **Evidence Collection Methods**



When you create or edit a requirement, you specify how applicants provide evidence:


| Method | What Applicants Do | Use When |
| ----------------------- | ----------------------------------------- | ----------------------------------------- |
| **Text Input** | Type a response in a text field | You need a written explanation |
| **File Upload** | Upload a document | You need certificates, quotes, invoices |
| **Link/URL** | Provide a web link | Evidence is online somewhere |
| **Acknowledgement** | Tick a checkbox to confirm | They’re agreeing to something |
| **Risk Assessment** | Evidence is in their risk assessment | Info already captured earlier in the form |
| **Draft Event Listing** | Evidence is in their event draft | Info already captured earlier in the form |
| **Club Documents** | Select from their club’s document library | They’ve uploaded it previously |


### **Adding a New Requirement**



- Go to TUSA Internal → Grants → Grant Requirements
- Add a new entry
- Fill in:

– Clear requirement name  
– Whether documentation is required  
– Which evidence methods are acceptable

- Save
- Go to each grant that needs this requirement and tick it



### **Removing a Requirement**



If a requirement is no longer needed:

**Option A: Remove from specific grants**

- Edit each grant
- Untick the requirement
- It won’t appear for those grants anymore

**Option B: Delete entirely**

- Only do this if the requirement isn’t ticked on ANY grant
- Go to Grant Requirements list
- Delete the entry

**Tip:** If unsure, just untick it from all grants rather than deleting. It won’t appear anywhere if it’s not attached to any grant.

---



## **Why Grants Are Integrated with Event Applications**



Grant applications are built into the Event Application form because they share information:


| Shared Information |
| ----------------------------------------- |
| Event details and descriptions |
| Budget breakdowns and expenses |
| Partner organisations and staffing |
| Risk assessments and safety documentation |
| Venue information and attendee numbers |


This means clubs fill out **ONE comprehensive form** instead of:

- A risk assessment
- An event application
- A liquor permit application
- A venue hire form
- AND a separate grant application (with all the same questions repeated)

**Note:** A standalone grant application form is also available for grants that aren’t tied to specific events.

---



## **The Public-Facing Flow**



What students experience:

- Visit the Grants page on the TUSA website
- See all currently open grants (name, description, closing dates)
- Read grant details to find the right one for their event
- Start an Event Application from their Club Dashboard
- Select their chosen grant from the dropdown
- See requirements and caps automatically displayed
- Complete ONE form covering event approval, risk assessment, AND grant application

---



## **What You See When Assessing**



When an application lands in your inbox:

- **Grant Details** – Which grant they applied for
- **Requirements Met** – Evidence they provided for each requirement you configured
- **Caps Applied** – How their request compares to limits
- **Documents Table** – All attached documents in one structured list
- **PDF** – Professional summary you can print for grants meetings

---



## **Common Configuration Tasks**



&nbsp;

### **“I want to add a new grant program”**



- TUSA Internal → Grants → Current Grants → Add New
- Fill in name, description, dates
- Configure caps if applicable
- Tick all relevant requirements
- Save



### **“I want to change what’s required for a grant”**



- Open the grant in Current Grants
- Find Prerequisites/Requirements
- Tick or untick requirements
- Save



### **“I want to add a new requirement that doesn’t exist”**



- TUSA Internal → Grants → Grant Requirements → Add New
- Create the requirement with evidence methods
- Save
- Go to each relevant grant and tick the new requirement



### **“A requirement’s wording needs updating”**



- TUSA Internal → Grants → Grant Requirements
- Find and edit the requirement
- Update the name/description
- Save – it updates everywhere that requirement is used



### **“I want to close a grant to new applications”**



Either:

- Set the Closes date to today (or past)
- Or change status to inactive

The grant will no longer appear in the application dropdown.

---



## **Troubleshooting**



&nbsp;

### **“Applicants can’t see a requirement”**



**Check:**

- Is the requirement ticked on that specific grant?
- Is the requirement entry saved and active?



### **“A requirement appears on the wrong grant”**



**Fix:**

- Open the grant where it shouldn’t appear
- Untick that requirement
- Save



### **“Caps aren’t displaying correctly”**



**Check:**

- Is Cap Type set correctly (dollar vs percentage)?
- Are the cap values entered in the right fields?
- For sub-caps, are entries properly linked to the grant?



### **“A grant isn’t appearing for applicants”**



**Check:**

- Are the Opens and Closes dates correct?
- Is today’s date within that range?
- Is the grant status active?

---



## **Quick Reference**




| Task | Where to Go |
| ---------------------- | ------------------------------------------------------- |
| Configure a grant | TUSA Internal → Grants → Current Grants → [click grant] |
| Add/edit requirements | TUSA Internal → Grants → Grant Requirements |
| See all applications | TUSA Internal → Grants → Applications |
| Process an application | Your Workflow Inbox |


---



## **Related Guides**



- [Processing Grant Applications](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/grants-funding/configuring-grants/#processing-grants) – Reviewing and approving applications
- [Event Approval](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/grants-funding/configuring-grants/#event-approval) – When grants are part of event applications

