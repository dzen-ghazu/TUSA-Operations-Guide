---
title: Managing Feedback Forms
hide:
  - toc
---
# **Managing Feedback Forms**

Feedback is a flexible system for collecting opinions, ratings, suggestions, surveys, and any input from students or staff. Each feedback post is a Feedback entry that configures a shared submission form — you set up the feedback post, and the form adapts automatically.

---



## **Why this exists**



Almost every “we need a new form for X” request can be served without building a new form from scratch. Work through these checks in order before creating anything new:



### **1. Would the General Contact form do?**



The General Contact form (lands in `hello@tusa.utas.edu.au`) already handles “I have a question,” “I want to tell you something,” “How do I…?” If the request is really just “people need a way to get in touch about X,” send them to the contact form — no new feedback post needed.



### **2. Is feedback already baked in?**



Some surfaces collect feedback automatically — you don’t need a Feedback post for these:


| Surface | What’s automatic |
| ------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Events on the Event Calendar** | The single-event page shows a star rating + workshop/training feedback form **automatically once the event end date passes**. Saves as a review on the event. Average rating displayed publicly. No setup needed per event. |
| **Products in the TUSA Store / Hire Store** | The standard product reviews — star rating + comment, shown on the product page. |


So if the request is “we want feedback after our training session” or “we want feedback after our workshop” and the session is on the event calendar, you’re already covered. Direct attendees to the event page after the end date and the form is there.

A separate Feedback post is right when:

- The thing isn’t on the event calendar (an ongoing service like Food Hub, a campaign rather than a single dated event, an open suggestion box)
- You need different questions than the standard training/workshop set
- You want anonymous mode, or specific topic categories, or campus-tied responses
- You want it to flow into the Workflow Inbox and EOIs + Feedback view, not the event’s comments



### **3. If a structured form *is* needed — EOI or Feedback?**




| If you’re collecting… | Use |
| ------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Applications, registrations, sign-ups, intent to participate, candidate nominations | **EOI** — see [Managing Expressions of Interest](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/eois-feedback/managing-feedback-forms/managing-eois.md) |
| Opinions, ratings, surveys, suggestions, post-event reflection, anonymous input, “how did it go” | **Feedback** (this guide) |


Both systems have the same backbone: configure a post, the form rewrites itself, submissions appear in a frontend list view in the TUSA Internal group, and approvals/responses route to the right team.

---



## **How It Works**



- You create a **Feedback post** and configure it using the settings tabs
- The Feedback post’s single page automatically shows the submission form
- The form reads the post’s settings to show or hide each section — campus dropdown, topic checkboxes, rating scales, text questions, identity collection, anonymous mode, etc.
- Submissions go to the assigned staff member and team — they see them in their Workflow inbox
- Staff review and respond (with notes if a follow-up was requested)

**Key concept:** the form has every possible question built in but hidden by default. Your settings on the feedback post turn the relevant sections on. You never edit the form itself.

---



## **Creating a Feedback Form**



Go to **Feedback > Add New** in the admin area.



### **Title**



The name of the feedback (e.g., “O-Week 2026 Feedback”, “Food Hub Service Survey”, “Anonymous Wellbeing Pulse — Sem 1”). This is what students see at the top of the page and in the listing views.



### **Tab 1: Basics**




| Field | Purpose |
| -------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| **Opens** | When the form starts accepting submissions. Before this date, the page shows a “not yet open” message. |
| **Closes** | When submissions close. After this date, the page shows a “closed” message. Existing submissions are unaffected. |
| **Allow Anonymous** | If on, the form tells the submitter their feedback is anonymous and doesn’t require name/email. |
| **Collect from submitter** | Pick which identity fields to ask for: Name, Email, Student ID. Tick none to keep it fully anonymous. |
| **Follow-up Question** | Off / Yes-No / Three-option (“yes / no / maybe later”). Use this when you might want to contact the submitter back. |
| **Ask for Campus** | Off / Optional / Required. Adds the standard campus dropdown (Hobart – Sandy Bay, Hobart – City, Launceston – Inveresk, Cradle Coast, etc.). |


### **Tab 2: Topics**



Topics let the submitter tell you what their feedback is *about* before they get into details.


| Field | Purpose |
| ------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------ |
| **Topic Selection** | Off (no topic question), Predefined (pick from preset categories), Custom (you write your own list), Free Text (they type it). |
| **Topic Field Label** | The question shown to the submitter, e.g., “What’s your feedback about?” |
| **Categories to Show** *(predefined mode)* | Tick which preset topics to offer: Academic, Facilities, Fees, Wellbeing, Transport, Housing, Clubs, Food. |
| **Custom Topics** *(custom mode)* | One topic per line, e.g., “Café experience / Menu / Pricing / Opening hours” — these become checkboxes. |


### **Tab 3: Discovery**



Optional questions that help you understand reach and awareness.


| Field | Purpose |
| ----------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| **Discovery Questions** | Tick any of: “How did you hear about us?”, “Is this your first time using this service?”, “Are you aware of other TUSA services?” |
| **“How heard” Options** | If “how heard” is on, list one option per line (e.g., “Friend / Social media / O-Week / Email / Poster on campus”). |


### **Tab 4: Ratings**



Up to **4 rating scale questions**, each on a 1–5 scale. Leave any blank to skip.

For each rating you can set:

- **Question** — e.g., “How would you rate the quality of the event?”
- **Low (1) label** — e.g., “Poor”
- **High (5) label** — e.g., “Excellent”

The labels anchor the scale so submitters know which end is which.



### **Tab 5: Text Questions**



Up to **2 free-text questions** with longer answers. Each one can be marked required.

A general “Additional feedback or comments” textarea always shows at the end — you don’t need to add that yourself.



### **Tab 6: Content**




| Field | Where it shows |
| ------------------------ | ------------------------------------------------------------------------------------------------- |
| **Introduction Message** | Top of the form. Set the context — what is this feedback for, who reads it, what happens with it. |
| **Confirmation Message** | After submission. Thank them and explain next steps. |


### **Tab 7: Notifications**




| Field | Purpose |
| --------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Assigned Staff** | The TUSA staff member who manages this feedback. They get notified by email AND see submissions in their Workflow inbox. |
| **Assigned Team** | Which TUSA team handles this feedback (Events, Social Media, Grants, SASH, Clubs, Food Hub, UTE, Advocates). Team members see submissions in their workflow inbox. |
| **Additional Emails** | Extra email addresses to be notified (email only, no workflow inbox). |


---



## **Viewing Submissions**




| Where | What you see |
| ----------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------ |
| **TUSA Internal group → EOIs + Feedback tab** ([link](https://tusa-dev.its.utas.edu.au/clubs/clubs-index/tusa-internal/eoi/)) | Combined view of every EOI and feedback submission, filterable by name, type, status |
| **Feedback only view** ([link](https://tusa-dev.its.utas.edu.au/clubs/clubs-index/tusa-internal/eoi/feedback/)) | Just feedback submissions |
| **Workflow Inbox** (Profile avatar → Workflow Inbox in the admin area) | Pending submissions assigned to you or your team |
| **Form Entries** (Forms > Entries > Feedback Submission Form) | All raw submissions for all feedback posts |


The frontend views are the easiest place to triage day-to-day. The Workflow Inbox is for when something needs an action (responding to a follow-up request, escalating).

---



## **After the Feedback Closes**



Once the close date passes:

- The form automatically shows a “Feedback Closed” message
- Existing submissions stay in the workflow — you can still respond to follow-ups
- The feedback post stays published as a record but no new submissions can come in
- To reopen, just push the close date out

---



## **Common Scenarios**



These walk through the actual ad hoc form requests staff have raised — so when someone asks “can we have a form for X,” the answer is usually one of these patterns.



### **General contact form (replaces a Hello@ form)**



The “got a question, want to tell us something” form that lands in Hello@.

- **Type:** Feedback
- **Title:** “Get In Touch” (or whatever fits the page).
- **Basics:** Allow Anonymous *off* (we need to be able to reply). Collect: Name, Email. Follow-up: Off (a reply is implied). Ask for Campus: Optional.
- **Topics:** Predefined — tick all 8 categories so they can tell you what it’s about.
- **Discovery:** Tick “How did you hear about us?” if you want reach data.
- **Ratings:** Skip all.
- **Text Questions:** “What can we help with?” (required).
- **Notifications:** Assigned to whoever owns Hello@. Additional Emails: hello@tusa.utas.edu.au.



### **Campaign or week-long feedback (e.g. SHAG Week, O-Week, C&S Festival)**



> Stop and check first: if the thing is **a single training session or workshop on the Event Calendar**, the event page already collects post-event feedback automatically (see [Is feedback already baked in?](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/eois-feedback/managing-feedback-forms/#2-is-feedback-already-baked-in)). This scenario is for *campaign-level* or *cross-event* feedback — when you want overall reflection on a week or festival rather than per-session reviews.

- **Type:** Feedback
- **Title:** “SHAG Week 2026 — Your Feedback” (or equivalent campaign name).
- Opens = day after the campaign closes. Closes = 2–3 weeks later.
- **Basics:** Allow Anonymous on. Collect: optional email if they want a reply about a specific issue. Follow-up: Yes-No. Ask for Campus: Optional.
- **Topics:** Custom — list the events/components that ran during the week, e.g. “Panel discussion / Stalls / Workshop / Social event”
- **Ratings:** Two or three — overall experience, was it informative, was it accessible.
- **Text Questions:** “What worked well?” and “What would have made the campaign stronger?”
- **Notifications:** Assigned to campaign coordinator, team = Events or SASH (depending on campaign). Additional Emails: events@tusa.utas.edu.au or the relevant team inbox.



### **Food Hub experience feedback**



- **Type:** Feedback
- **Title:** “Food Hub Feedback”.
- Opens = ongoing. Closes = end of semester (then duplicate for next semester).
- **Basics:** Allow Anonymous on. Collect: nothing. Follow-up: Off. Ask for Campus: Required (so you can tell which Food Hub).
- **Discovery:** Tick “Is this your first time?” + “Are you aware of other TUSA services?”
- **Topics:** Custom — “Quality / Range / Pricing / Staff / Opening hours / Cleanliness”.
- **Ratings:** Two — overall experience and likelihood to recommend.
- **Text Questions:** “Anything else we should know?” (not required).
- **Notifications:** Assigned to Food Hub coordinator, team = Food Hub.



### **Anonymous wellbeing pulse (per semester)**



- **Type:** Feedback
- **Title:** “Wellbeing Pulse — Semester 1 2026”.
- Open for one week per semester.
- **Basics:** Allow Anonymous on. Collect: nothing. Follow-up: Off. Ask for Campus: Optional.
- **Topics:** Predefined — tick Wellbeing, Academic, Housing, Fees.
- **Ratings:** Four — stress level, study/life balance, awareness of TUSA support services, overall wellbeing.
- **Text Questions:** “What would help you most right now?” (not required).
- **Notifications:** Assigned to SASH lead, team = SASH.



### **Advocacy issue intake**



This is feedback rather than an EOI — students aren’t applying for anything, they’re reporting an issue.

- **Type:** Feedback
- **Title:** “Speak to an Advocate”.
- Always open.
- **Basics:** Allow Anonymous *off*. Collect: Name, Email, Student ID. Follow-up: Three-option (“yes / no / an advocate can decide if needed”). Ask for Campus: Required.
- **Topics:** Custom — “Academic appeal / Misconduct / Tenancy / Financial / Other”.
- **Ratings:** Off (this is intake, not satisfaction).
- **Text Questions:** “What’s the issue?” (required) and “What outcome are you hoping for?” (not required).
- **Notifications:** Assigned to Advocates lead, team = Advocates.

---



## **Troubleshooting**



&nbsp;

### **Form shows “Feedback Not Yet Open”**



The current date is before the **Opens** date. Check the date is correct.



### **Form shows “Feedback Closed”**



The current date is past the **Closes** date. Update the close date if you need to extend.



### **A configured field isn’t showing on the form**



The form rebuilds itself from your settings each time it loads. If a section isn’t showing, check:

- The toggle for that section is on (e.g., “Ask for Campus” is set to Optional or Required, not Off)
- For ratings/text questions, the **Question** field is filled in — blank questions are skipped
- For predefined topics, you’ve actually ticked some categories
- You’ve published the feedback post (not Draft)



### **Submissions not appearing in the Workflow inbox**



Check that **Assigned Staff** or **Assigned Team** is set on the feedback post. If neither is set, the workflow has no assignees and submissions stall.



### **Ratings show as 1-5 with no labels**



The Low/High labels weren’t filled in. Edit the feedback post and add the anchor labels (e.g., “Poor” and “Excellent”).



### **A submitter wants to be contacted but didn’t tick follow-up**



Check the entry in Forms > Entries — the email field is captured even if follow-up wasn’t requested. You can reply directly. If they were anonymous, you can’t reach them; that’s the trade-off of allowing anonymous mode.