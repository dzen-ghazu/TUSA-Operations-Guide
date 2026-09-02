---
title: Managing Expressions of Interest (EOIs)
hide:
  - toc
---
# **Managing Expressions of Interest (EOIs)**

EOIs are used across TUSA for collecting applications for events (market days, expos, SHAG), volunteering opportunities (including student rep candidacy), club formation, training enrolment, and almost any “we need a form for X” request that asks people to register their interest in something. Each EOI is a custom post that configures a shared submission form — you set up the EOI post, and the form automatically populates and adapts based on the choices you make.

---



## **Why this exists**



Almost every ad hoc form request that comes through MarComms can be served *without* building a new form from scratch. Work through these three checks in order before creating anything new:



### **1. Would the General Contact form do?**



The existing General Contact form (lands in `hello@tusa.utas.edu.au`) already handles “I have a question,” “I want to tell you something,” “How do I…?” — anything that’s really a one-off message rather than a structured application. **If the request is “people need a way to get in touch about X,” the answer is usually: send them to the contact form.** No new post needed.



### **2. If a structured form *is* needed — EOI or Feedback?**



Between EOIs and [Feedback forms](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/eois-feedback/managing-expressions-of-interest-eois/managing-feedback.md), almost every ad hoc structured-form request is covered.


| If you’re collecting… | Use |
| ------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Applications, registrations, sign-ups, intent to participate, candidate nominations, training enrolment | **EOI** (this guide) |
| Opinions, ratings, surveys, suggestions, post-event reflection, anonymous input | **Feedback** — see [Managing Feedback Forms](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/eois-feedback/managing-expressions-of-interest-eois/managing-feedback.md) |


### **3. Is this an event? Then attendees just need a ticket**



**EOIs are for people *running* something (stallholders, contributors, volunteers, candidates, applicants). Not for people *attending* it.** If the thing is a scheduled event with a date and a location, attendees reserve a ticket through the **Event Calendar** — they don’t need an EOI.

So before creating an EOI, ask: **who’s it for?**


| Who | What they need |
| ----------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------- |
| Someone *attending* a scheduled event (e.g. coming to a market day, attending a training session, going to a SHAG week panel) | Calendar entry with an event ticket — no EOI |
| Someone *running a stall* or *contributing to* an event (e.g. having a stall at C&S Day, presenting in SHAG Week) | **EOI** — and the event itself goes on the calendar separately |
| Someone applying for an *ongoing role* (volunteering, candidacy, club formation) | **EOI** — no calendar entry (it’s not a dated event) |
| Someone asking when the *next cohort opens* (training waitlist, “let me know when this comes back”) | **EOI** for waitlist, or General Contact form for “let me know” |


Common pattern for events with stallholders/contributors: **two posts** — a calendar entry for the event itself (where attendees grab a ticket), and an EOI for stallholders to apply. Each does a different job. The EOI lives at `/get-involved/expressions-of-interest//`, the calendar entry at `/events//`.

> Note: post-event feedback for sessions/workshops on the Event Calendar is **automatic** — the event page shows a star rating + feedback form once the end date has passed, no setup needed. So you don’t need an EOI or a Feedback post for that. See [Managing Feedback Forms — Is feedback already baked in?](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/eois-feedback/managing-expressions-of-interest-eois/managing-feedback.md#2-is-feedback-already-baked-in) for when you’d build a separate Feedback post anyway.

---



## **How It Works**



- You create an **EOI post**, set its **type**, and configure it using the settings that appear (for Event / Volunteering / Club Formation the type is the **EOI Type dropdown** in the main editor; for an Election nomination round you tick **Election** in the sidebar instead)
- The EOI post’s single page automatically shows the shared submission form
- The form reads the EOI post’s settings and type to show/hide questions, set applicant types, display content, etc.
- Submissions go through an **approval workflow** — the assigned staff member and team see it in their Workflow Inbox
- Staff approve or reject with notes — the applicant gets notified by email

---



## **An EOI collects interest, not documents**



An EOI is exactly what its name says: an **expression of interest**. Someone is telling you they’d like to take part: to volunteer, run a stall, or stand for a role. The form captures who they are and what they’re interested in, and sends them to the right team to review. That is the whole job.

It is **not** where you collect or store the paperwork someone needs before they can start. Working with Vulnerable People cards, food handling certificates, IDs, signed agreements: those are onboarding records, and they live in the operational system for whoever manages that person, not in the EOI form itself.

- **TUSA staff and volunteers:** their records live in your people-management system (Employment Hero), where they stay secure and expiry dates are tracked.
- **Clubs are different:** a club holds its own members’ and helpers’ certificates in its club area, so club admins have them on hand for risk assessments and event applications. That’s a deliberate part of how clubs self-manage.

Either way, the EOI form is the front door, not the filing cabinet: it records who is interested, not their documents.

**But do tell people what they’ll need.** If a role requires a certificate or a card before someone can begin, say so on the form, in **Details & Requirements** or the **Closing Message** (Step 3), so applicants know what to expect once they’re accepted. You are setting expectations, not gathering documents. The requirements themselves are yours to set, so adjust the wording to whatever the opportunity actually needs. For example:

> “If your application is successful, you’ll need to provide a current Working with Vulnerable People card and a Safe Food Handling certificate before your first shift. You arrange these during onboarding, so you don’t need them to apply. The Working with Vulnerable People registration costs $22.92 and isn’t covered by TUSA.”

The short version: **interest on the form, documents at onboarding.** Two steps, in two systems.

---



## **Creating an EOI**



Go to **EOIs > Add New** in the admin area.



### **Step 1: Basic Setup**



- **Title** — The name of the opportunity (e.g., “O-Week Market Day 2026”, “Student Representative Candidate”)
- **EOI Type** (required) — for a normal opportunity, choose the type from the **EOI Type dropdown** in the main part of the editor:

– **Event** — Market days, expos, SHAG, careers fairs, etc.  
– **Volunteering** — Ongoing volunteer roles, training waitlists, committee applications, election *interest* phase  
– **Club Formation** — For starting a new club

An **Election** nomination round is set up a little differently: instead of the dropdown, you tick **Election** in the **EOI Types** box in the right-hand sidebar (see [Election EOIs](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/eois-feedback/managing-expressions-of-interest-eois/#election-eois) below). The formal election replaces the old standalone nomination form.

> **If the settings look wrong or empty, check the type first.** For Event / Volunteering / Club Formation, that’s the **EOI Type dropdown** in the main editor — pick one and the matching settings load below. For an Election, it’s the **Election** tick in the right-hand sidebar. The type you choose decides which settings appear and which questions the applicant sees.

The EOI type controls which fields appear in the rest of the configuration and which questions the applicant sees.



### **Which fields apply to which EOI type**



The fields below show or hide on the EOI edit screen based on which type you tick. This is so you only see what’s relevant to the kind of EOI you’re building.


| Setting | Event | Volunteering | Club Formation | Election |
| --------------------------------------------------------------- | ----- | ------------ | -------------- | -------- |
| Event Date / Times / Bump In / Bump Out | ✓ | — | — | — |
| Stall Options | ✓ | — | — | — |
| Equipment Hire Available | ✓ | — | — | — |
| Show Food Question | ✓ | — | — | — |
| Show Activity Question | ✓ | — | — | — |
| Show Space Requests | ✓ | — | — | — |
| Show Portfolio/URL Field | — | ✓ | — | — |
| Proposed Club Name / Club Type / Concept *(on the form itself)* | — | — | ✓ | — |
| Submissions Open/Close | ✓ | ✓ | ✓ | ✓ |
| Content (intro, description, closing, confirmation) | ✓ | ✓ | ✓ | ✓ |
| Applications accepted from | ✓ | ✓ | ✓ | — |
| Require Secondary Contact | ✓ | ✓ | ✓ | — |
| Require Insurance | ✓ | ✓ | ✓ | — |
| Require Attachment | ✓ | ✓ | ✓ | — |
| Collect Student ID | ✓ | ✓ | ✓ | — |
| Custom Questions 1–3 | ✓ | ✓ | ✓ | — |
| Acknowledgements | ✓ | ✓ | ✓ | — |
| Notifications (Assigned Staff, Team, Additional Emails) | ✓ | ✓ | ✓ | ✓ |
| Position list *(one position per line)* | — | — | — | ✓ |


> **Election is deliberately different.** When you tick **Election**, the editor swaps to a small, dedicated set of settings — the nomination window, who receives nominations (Returning Officer / team), and a **position list**. It does **not** show the event/volunteering/club options or the custom questions, because the whole structured nomination form (position, nominators, declarations, candidate statement, photo, agent) is built in already and appears to the applicant automatically. You configure *when* and *who* and *which positions*; the form provides the rest. See the [Student elections — Formal nomination phase](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/eois-feedback/managing-expressions-of-interest-eois/#student-elections--formal-nomination-phase) scenario below.

A few fields are conditional on a *parent toggle* rather than the EOI type:

- **Equipment Items** — only shows when Equipment Hire Available is on
- **Insurance Minimum** — only shows when Require Insurance is on
- **Attachment Instructions** — only shows when Require Attachment is on



### **Step 2: Dates & Timing**




| Field | Purpose | Notes |
| -------------------------------- | ------------------------------ | ------------------------------------------ |
| **Event Date** | When the event takes place | Events only |
| **Start Time / End Time** | Event hours | Events only |
| **Bump In / Bump Out** | Setup and packdown times | Events only |
| **Submissions Open** (required) | When people can start applying | Form shows “not yet open” before this date |
| **Submissions Close** (required) | Application deadline | Form shows “closed” after this date |


### **Step 3: Content**



These WYSIWYG fields control what the applicant sees on the form:


| Field | Where It Shows | What to Write |
| -------------------------- | --------------------------------- | --------------------------------------------------------------------------- |
| **Introduction Message** | Top of the form | Welcome the applicant, explain what this EOI is for |
| **Details & Requirements** | Below the intro, before questions | Full details — what’s provided, expectations, eligibility, responsibilities |
| **Closing Message** | Bottom of the form, before submit | Final instructions or encouragement |
| **Confirmation Message** | After submission | Thank them and explain next steps |


### **Step 4: Form Options**



These toggles control which questions appear on the form:


| Option | What It Does |
| ------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Applications accepted from** | Which applicant types can apply — Student, External Organisation, UTAS Team/Service, Club. Each selected type becomes a radio option on the form. |
| **Require Secondary Contact** | Adds a second contact person section |
| **Stall Options** | For events — turn on to show the standard 3-tier stall picker (Small Lot / Sharing / Big Lot) |
| **Equipment Hire Available** | Adds equipment hire question and item list |
| **Require Insurance** | Asks external applicants about public liability insurance |
| **Show Food Question** | Asks if they’ll be serving food |
| **Show Activity Question** | Asks what activities they have planned |
| **Show Space Requests** | Lets applicants request specific space or locations |
| **Require Attachment** | Adds a file upload section with custom instructions |
| **Collect Student ID** | Asks student applicants for their UTAS student ID |
| **Show Portfolio/URL Field** | Lets applicants share a website, portfolio, or social media link |


> **Not for personal onboarding documents.** Require Attachment is for things like a proposal, a stall layout, a portfolio, or an organisation’s insurance certificate. It is **not** the place to gather personal compliance records such as Working with Vulnerable People cards, food handling certificates, or IDs. Those are held in the system that manages that person (Employment Hero for TUSA people; the club’s own area for clubs), see **An EOI collects interest, not documents** above.



### **Step 5: Custom Questions**



Up to 3 custom free-text questions. Leave blank to skip. These are WYSIWYG fields so you can include formatting, links, or images in the question text.

**This is how you add location choice, opportunity selection, or any other question specific to your EOI.** You don’t need a separate form — just write the question here and the form will show it to applicants. For example:

- “Which campus would you like to volunteer at?”
- “Which opportunity are you interested in? (Food Hub / Events / Student Advocacy)”
- “Do you have any relevant experience or qualifications?”



### **Step 6: Acknowledgements**



A single WYSIWYG field listing everything the applicant must agree to. They tick **one checkbox** to confirm they’ve read and agree to all points.

Common acknowledgements for events:

- TUSA will only provide equipment I have requested to hire
- If I have a Big Lot with my own marquee, I will bring my own weights
- I must stay for the entire duration
- This is a smoke-free campus
- External organisations must provide proof of insurance

Common acknowledgements for volunteering:

- I understand the time commitment
- I meet the eligibility requirements
- I consent to my information being used for selection



### **Step 7: Notifications & Assignment**




| Field | Purpose |
| ---------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Assigned Staff Member** | The TUSA staff member who manages this EOI. They receive email notifications AND see submissions in their **Workflow Inbox** for approval. |
| **Additional Notification Emails** | Extra email addresses to receive submission notifications (email only, no workflow inbox). |
| **Assigned Team** | Which TUSA team handles this EOI. Options: Events, Social Media, Grants, SASH, Elections, Clubs, Food Hub, UTE, Advocates, General. Team members see submissions in their workflow inbox. |


---



## **Making sure applications reach the right people**



This is the part to get right, because it is the single thing that decides where a submission lands and who can action it. **An EOI sends its submissions wherever *that EOI post* is set to send them — nowhere else.** Routing is per-EOI, and it is set by you on the EOI post, under the **Notifications** tab (Step 7 above). There is no site-wide rule and nothing routes automatically by topic — if an EOI is assigned to a person, it goes to that person; if it is assigned to a team, it goes to that team.

So whenever you build an EOI, ask one question: **who needs to receive and approve these applications?** Then set that on the EOI post.

- **To send applications to a specific person** — set them as the **Assigned Staff Member**. They get the email and see it in their Workflow Inbox.
- **To send applications to a whole team** — set the **Assigned Team**. Everyone in that team sees it in their inbox, and the first to act completes it. (This is more robust than a single person, because it does not depend on one individual being available.)
- **To simply notify someone without giving them an approval inbox** — add their address to **Additional Notification Emails**. They get an email copy but do not action it.

You can set a staff member *and* a team — the submission then reaches both.



### **“Someone submitted, but the coordinator can’t see it”**



This is almost always the same thing: **the person looking is not who the EOI is assigned to.** A submission does not appear in someone’s inbox just because it is about their area — it appears because that EOI names them (or their team). If a coordinator cannot find an application, open the EOI post and check the **Notifications** tab: whoever is set there is who receives it. If it should go somewhere else, change the assignment and re-test.

> Worked example — **Food Hub volunteers.** Say you want Food Hub volunteer applications to land with the Food Hub coordinator rather than with general intake. Create (or edit) a **Volunteering** EOI and, on the **Notifications** tab, set the **Assigned Team to Food Hub** — and, if you want a named person too, set the coordinator as the **Assigned Staff Member**. From then on those applications appear in the Food Hub team’s Workflow Inbox. If instead you route all volunteering through one general EOI, applications go to whoever *that* EOI is assigned to, and that person triages and passes people on — both approaches are valid, it just depends how you want to work. The point is that it is a setting on the EOI, and it is yours to set.

---



## **The Approval Workflow**



Each EOI submission goes through an approval workflow:

**Start → Approval → Complete**



### **How approval works**



- Submission arrives → assigned staff member and team are notified
- The submission appears in their **Workflow Inbox** (Profile avatar → Workflow Inbox in the admin area)
- They review the submission details
- They choose **Approve** or **Reject**
- They **must add a workflow note** explaining the decision — this note is sent to the applicant
- The applicant receives an email:

– **Approved**: “Your EOI has been successful” + the workflow note  
– **Rejected**: “Your EOI has not been successful” + the workflow note



### **Writing good workflow notes**



The workflow note goes directly to the applicant, so write it as if you’re speaking to them:

**Good approval note:**

> “Welcome aboard! Please arrive by 7:30am for bump-in. We’ll send a site map and final details closer to the date.”

**Good rejection note:**

> “Unfortunately we’ve reached capacity for external stallholders at this event. We’d love to have you at our next market day — keep an eye on the EOI page for upcoming opportunities.”



### **Approval policy**



The approval step is set to **“any”** — meaning either the assigned staff member OR anyone in the assigned team can approve/reject. The first person to act completes the step.

---



## **Viewing Submissions**




| Where | What you see |
| ----------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- |
| **TUSA Internal group → EOIs + Feedback tab** ([link](https://tusa-dev.its.utas.edu.au/clubs/clubs-index/tusa-internal/eoi/)) | Combined view of every EOI and feedback submission, filterable by name, applicant type, status |
| **Open EOIs view** ([link](https://tusa-dev.its.utas.edu.au/clubs/clubs-index/tusa-internal/eoi/open/)) | Just currently-open EOI submissions |
| **Feedback view** ([link](https://tusa-dev.its.utas.edu.au/clubs/clubs-index/tusa-internal/eoi/feedback/)) | Just feedback submissions |
| **Workflow Inbox** (Profile avatar → Workflow Inbox in the admin area) | Pending submissions assigned to you or your team |
| **Form Entries** (Forms > Entries > EOI Submission Form) | All raw submissions for all EOIs, filter by EOI name |


The frontend views are the easiest place to triage day-to-day. The Workflow Inbox is for when something needs your action (approval/rejection).

---



## **After the EOI Closes**



Once the submissions close date passes:

- The form automatically shows a “Submissions Closed” message
- Existing submissions in the workflow are unaffected — you can still approve/reject them
- The EOI post remains published (as a record) but no new submissions can be made

To reopen an EOI, just update the close date to a future date.

---



## **Common Scenarios**



These walk through the actual ad hoc EOI requests staff have raised — so when someone asks “can we have a form for X,” the answer is usually one of these patterns. Each is just a configuration of the same EOI post type — you don’t need a different form per scenario.



### **Market Day, Expo, SHAG Week, C&S Day**



- Create EOI with type **Event**
- Set event date, bump in/out times, submission window
- Enable: Stall Options, Equipment Hire Available (and list the items in Equipment Items), Show Food Question, Require Insurance (and set Insurance Minimum), Show Activity Question, Show Space Requests
- Applications from: Student, External Organisation, UTAS Team/Service, Club
- Add acknowledgements about equipment, bump out, smoke-free campus, public liability insurance
- **Notifications:** Assigned to event coordinator. Team = Events. Additional Emails = events@tusa.utas.edu.au (or clubs@tusa.utas.edu.au if it’s a club-led event)



### **Training waitlist / pre-registration (e.g. Mental Health First Aid)**



> **Stop and check first:** is a training cohort currently scheduled with a date? If yes, students reserve a ticket through the calendar entry — **don’t** create an EOI for that. This scenario is for the *opposite* case: training that isn’t scheduled yet, where you’re collecting interest so you can plan a cohort and contact people when it opens.

- Create EOI with type **Volunteering** (a training waitlist is the same shape — they’re saying “I want to be told when this opens”)
- Submission window: open ongoing, close once you have enough interest to schedule a cohort
- Applications from: Student
- **Collect Student ID:** on
- **Custom Question 1:**

> “When do you need your certification by? (e.g., before March 2026, no rush, etc.)”

- **Custom Question 2:**

> “Preferred training location:  
> – Hobart  
> – Launceston  
> – Burnie  
> – Online”

- Acknowledgements about commitment, prerequisites, willingness to be contacted when a cohort opens
- **Notifications:** Assigned to the training coordinator. Team = General. Additional Emails = training@tusa.utas.edu.au.

When you’ve gathered enough interest, schedule the cohort as an Event Calendar entry with tickets — and let the waitlist know via the email addresses they submitted.

> Why text-answer for location instead of a dropdown? The form’s custom questions are free-text on purpose — staff triage by reading and following up. A strict dropdown adds nothing because you’re coordinating the training session afterwards anyway. If a staff member writes the question with the four options listed in a bullet list, applicants pick one.



### **Volunteering EOI (full campus + interest list)**



The general TUSA volunteering EOI as Renee scoped it.

- Create EOI with type **Volunteering**
- Set submission window (typically a semester window)
- Applications from: Student
- **Collect Student ID:** on
- **Custom Question 1:**

> “Which campus would you like to volunteer at?  
> – Hobart – Sandy Bay  
> – Hobart – City  
> – Hobart – Hedberg  
> – Hobart – IMAS  
> – Hobart – Medical Science Precinct  
> – Hobart – Creative Arts Precinct  
> – Launceston – Inveresk  
> – Launceston – Newnham  
> – Cradle Coast (Burnie)  
> – Sydney (Rozelle)  
> – Online/Distance”

- **Custom Question 2:**

> “What are you interested in volunteering for?  
> – **Food Hub** — if you’re passionate about food and cooking, volunteer to assist at our Food Hub  
> – **Student Media Team** — if you’re keen on upskilling for media and communications  
> – **Events team** — if you have an interest in running events  
> – **Student Representatives** — if you’re passionate about student issues and want to help campaigns  
> – **TUSA team** — if you’re not sure, help us in the office”

- Acknowledgements about time commitment, responsibilities, conduct
- **Notifications:** Assigned to Bus. Admin. Team = General/Advocates. Additional Emails = hello@tusa.utas.edu.au.

Custom questions are formatted text fields — you can include bullet lists, links, bold, anything. Applicants answer in a text box, and the formatted question text gives them the options. This means **one volunteering EOI covers every region and every opportunity** — you don’t need a separate form per area.



### **Committee / officer applications (e.g. Equity Committee)**



A request like the Equity Committee — “applications are open for two officer roles, collect a few details and a short why” — is just a Volunteering EOI. You set it up the same way as the others. **You don’t need a separate form, and you don’t need to ask anyone to build one.**

- Create EOI with type **Volunteering**
- Set the submission window (when applications open and close)
- Applications from: Student
- **Collect Student ID:** on
- **Custom Question 1 — the role:**

> “Which Equity Officer role are you applying for?  
> – International Students Officer  
> – Carers Officer”  
>  
> (List whichever roles are open this round — change them next time without touching anything else.)

- **Custom Question 2 — pronouns:**

> “Your pronouns (optional).”

- **Custom Question 3 — study details:**

> “Your course and year of study (e.g. 2nd Year Medicine), and your campus or study mode.”

- **Custom Question 4 — why:**

> “Tell us why you’re interested in the role.”

- **Acknowledgements** — put both confirmations in the one Acknowledgements box, one per line. The applicant agrees to all of them with the single tick:

> – I identify as a member of the community I am applying to be an Equity Officer for.  
> – I consent to UTAS releasing my information to TUSA to confirm my enrolment as a current student, and to check my record of academic and behavioural conduct.

- **Notifications:** Assigned to the staff member who runs the committee. Team = the relevant team. Additional Emails = the committee’s contact address.

That’s the whole form. Name and email are collected automatically, the role and questions come from the custom questions above, and the two confirmations sit under the single acknowledgement tick.

> **About the confirmations:** the current standalone form has these as two separate tickboxes. In an EOI they become two lines under one tick — the applicant is still agreeing to both, and both are recorded against their submission. If you ever need each confirmation recorded as its own separate tick (rather than one combined agreement), that’s a change request — flag it, don’t try to build it.

> **Re-running next round:** duplicate the EOI post and update the dates and the list of roles in Custom Question 1. Nothing else changes.



### **Student elections — Interest phase**



Use this *weeks or months before nominations open*, to gauge who’s thinking about running. It is deliberately lightweight — it is **not** the formal nomination, so it uses the ordinary **Volunteering** type (not Election).

- Create an EOI and choose type **Volunteering** from the EOI Type dropdown in the main editor
- Set the submission window for the interest period
- Applications from: Student only
- **Custom Question 1:** “Which position area are you interested in?”
- **Custom Question 2:** “Why are you interested in running?”
- **Notifications:** Assigned to the Returning Officer. Team = Elections. Additional Emails = elections@tusa.utas.edu.au.

That’s all — no nomination-specific config in this phase.



### **Student elections — Formal nomination phase**



This is the **Election** EOI type, and it **replaces the old standalone Elections Nomination Form**. Everything that form collected — position, nominators, declarations, candidate statement, photo, election agent — is **built into the shared EOI form already**. You do **not** rebuild those questions each cycle and you do **not** paste them into custom questions. Your job is just to open a nomination round and say who handles it.

> **Don’t build a new Gravity Form for elections.** The nomination form is provided by the Election type. If a nomination needs a field that isn’t there, raise it — we extend the built-in form, we don’t spin up a one-off form.

**How to open a nomination round**

- **EOIs → Add New.** Give it a clear title (e.g. “2026 Annual Elections — Nominations”).
- In the **right-hand column**, tick the **Election** type. The editor now shows the small Election settings set (and hides the event/volunteering/club options — that’s expected).
- Set the **nomination window** (submissions open / close) to the official nominations dates.
- Set who receives and approves nominations: the **Returning Officer** as the assigned person, and/or the assigned **team** (Elections). This is who sees nominations in their Workflow Inbox.
- Fill in the **Position list** — **one position per line**. These become the positions a candidate can choose from on the nomination form. (It’s a plain list, so you can change the positions each cycle without anyone rebuilding a dropdown.)
- Publish.

That’s the whole setup. When a student opens the EOI during the nomination window, the form automatically presents the full structured nomination: the position picker (from your list), their enrolment name, pronouns and ballot name, student ID, address, region, contact details, NUS delegate opt-in, social media handles, nominators, the candidate statement (1000-character limit), the candidate photo upload, the declarations, individual-vs-group, and the election-agent question. If they name an agent, that agent is emailed a notice on submission.

**What the built-in form already handles (so you don’t):**

- The **candidate declaration** — the full set of consents (nomination consent + eligibility, UTAS releasing enrolment details, nominator consent, Election Policy, campaigning requirements section 6.4, availability if elected, individual vs group). These are baked into the form as required tick items.
- The **candidate photo** upload with the passport-style instruction.
- The **election agent** notification on submission.
- **One position per nomination** — a candidate seeking two positions submits two nominations (one position, one statement, one declaration set each). That keeps each nomination self-contained.

**Notifications**

Assigned to the **Returning Officer**. Team = Elections. Additional notification address = elections@tusa.utas.edu.au.

> **Re-running next cycle:** duplicate the Election EOI post and update the dates and the position list. You don’t touch the nomination questions — they’re part of the form.

> **What’s intentionally not collected:** a drawn signature (the declaration ticks + submission timestamp + verified UTAS email serve the same purpose). The Personal Information Protection statement lives in the EOI’s intro/closing message.



### **New club formation**



- Create EOI with type **Club Formation**
- Set submission window
- Applications from: Student only (the Club option shows a message directing existing clubs to their dashboard instead)
- The form automatically shows club-specific fields: proposed name, club type, concept & vision
- **Notifications:** Assigned to Clubs coordinator. Team = Clubs. Additional Emails = clubs@tusa.utas.edu.au.



### **General contact / “Get In Touch”**



If the request is genuinely “let people get in touch with us,” that’s a [Feedback form](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/eois-feedback/managing-expressions-of-interest-eois/managing-feedback.md), not an EOI — they’re not registering interest in anything specific. See the General Contact scenario in the feedback guide.

---



## **Troubleshooting**



&nbsp;

### **Form shows “Submissions Not Yet Open”**



The current date is before the **Submissions Open** date. Check the date is correct.



### **Form shows “Submissions Closed”**



The current date is past the **Submissions Close** date. Update the close date if you need to extend.



### **No applicant type options showing**



The **Applications accepted from** checkboxes haven’t been ticked on the EOI post. Edit the EOI and select at least one applicant type.



### **Applicant type shows as one combined option**



This is a known issue with how the form receives the multi-value applicant types field. A small fix in the page template should split them into individual options. If it’s not working, contact the site administrator.



### **Submissions not appearing in the Workflow Inbox**



Check that the **Assigned Staff Member** or **Assigned Team** is set on the EOI post. If neither is set, the approval step has no assignees and submissions will stall.



### **Applicant didn’t receive approval/rejection email**



Open the entry in the form’s entries list and look at the workflow timeline — it should show the approval action and email dispatch. If the email failed, ask a site administrator to check delivery logs.