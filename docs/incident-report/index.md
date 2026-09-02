---
title: Handling Incident Reports
hide:
  - toc
---
# **Handling Incident Reports**

This guide covers how to receive and process incident reports submitted through the Report Anything system.

---



## **Important: Sensitivity and Confidentiality**



Incident reports may contain sensitive information about:

- Sexual assault and harassment (SASH)
- Discrimination
- Safety concerns
- Personal disclosures

**Always:**

- Treat all reports with appropriate confidentiality
- Follow TUSA’s incident response policies
- Escalate to your manager when unsure
- Respect reporter privacy, especially for anonymous submissions

**Never:**

- Share report details with unauthorised people
- Discuss reports in public areas
- Leave reports visible on your screen unattended

---



## **How the System Works**



The Report Anything system has two parts behind the scenes:

- **The report** — what the reporter fills out. This creates the original report record.
- **The investigation** — created automatically when a report comes in. This is where allocation and investigation happen.

You don’t need to worry about this distinction day-to-day, but it’s useful to know:

- **Received Reports** (TUSA Internal → Reports tab) shows the original reports as submitted
- **Investigations** (TUSA Internal → Reports tab) shows the investigations — what staff work on
- **Your workflow inbox** shows the investigation steps — allocation tasks and investigation tasks

---



## **How Reports Come In**



&nbsp;

### **Online Submissions**



Reports are submitted through `/report-anything/`

Reporters can choose:

- **Anonymous** – No personal details collected
- **Named** – Includes reporter’s contact information



### **Phone/In-Person Reports**



For reports received by phone or in person, staff enter them manually using the same reporting form:

**Where:** TUSA Internal → Reports tab → **New** sub-tab

---



## **Finding Reports**



&nbsp;

### **Your Workflow Inbox**



**Where:** Profile avatar → Profile → Workflow Inbox tab  
**Direct URL:** `/my/workflow-inbox/`

Reports are **automatically routed** based on incident type. You’ll only see reports assigned to your role.



### **TUSA Internal Group**



**Where:** `/clubs/clubs-index/tusa-internal/` → **Reports** tab


| Sub-tab | What’s Here |
| -------------------- | ----------------------------------------------------- |
| **Received Reports** | All incoming reports, as submitted by the reporter |
| **Investigations** | Investigation records and progress — where staff work |
| **New** | Form for manual entry of phone/in-person reports |


---



## **How Reports Are Routed**



When a report is submitted, the system automatically creates an investigation entry and routes it based on the incident type. Reports are processed in **priority order** — the first matching category handles it:


| Priority | Incident Type | Assigned To |
| -------- | ------------------------------------ | -------------------------------------------------------------------------- |
| 1 | **Sexual assault/harassment (SASH)** | SASH team (`tusa_sash` role) |
| 2 | **TUSA or UTAS staff involved** | Shauna Lee Ward (named individual, not a team) |
| 3 | **Club-related incidents** | Clubs admin team (`tusa_admin_clubs` role) |
| 4 | **TUSA events** | Events team (`tusaevents` role) |
| 5 | **Other incidents** | Advocates (`tusaadvocates`) **and** Internal admin (`tusa_admin_internal`) |


**The “Other incidents” route needs one action from each of the two groups**, not one in total. Nobody currently holds `tusaadvocates`, so until somebody does, that route cannot complete. This is the route most reports take.

**SASH isolation:** SASH reports are handled exclusively by the SASH team. If a report is categorised as SASH, it goes only to the SASH team — no other team sees it. This is by design due to the extreme sensitivity of sexual assault content.

**One team per report:** Each report goes to exactly one team. The system processes categories in priority order and stops at the first match. For example, a SASH incident at a club event goes to the SASH team only, not to the clubs team.



### **The email alert when a report arrives**



Separately from the workflow queue above, submitting the form sends one email alert to a mailbox.  
Exactly one of these two goes out:


| Alert | Goes to | When |
| --------------------------------- | -------------------------- | ------------------------------------------------------------------------------------------------------------------ |
| Report received | Clubs | `clubs@tusa.utas.edu.au` | The report is about someone from a club or society, **and** it is not a sexual assault or sexual harassment matter |
| Report received | Student support | `support@tusa.utas.edu.au` | Everything else, **including every sexual assault or sexual harassment report regardless of who it is about** |


**Sexual assault and harassment always overrides the club split.** A SASH matter involving a club goes  
to `support@`, never to `clubs@`. This mirrors the SASH isolation in the workflow routing, so the email  
alert and the workflow queue agree with each other.

“Sexual assault or sexual harassment” here means either of the two things that send a report to the  
SASH team: incident type (field 24) set to sexual assault or sexual misconduct, **or** online incident  
type (field 59) ticked as “Sexual harassment or unwanted sexual messages”. Both are tested, because a  
report can reach the SASH queue through either one.

There is also a **SASH Notification** on the form pointed at a named individual. It is currently  
switched off. When a dedicated SASH mailbox exists it should be repointed there and enabled, rather  
than at a person.

**You will only see reports that match your role’s permissions.**

When a report lands in your workflow inbox, you’ll receive an email notification.

---



## **Processing a Report**



&nbsp;

### **Step 1: Allocation**



When a report appears in your team’s workflow inbox, your job is to:

- **Review the report content** to understand what happened
- **Select the assigned team** — **required**
- **Nominate an investigator** — **required**. The list is limited to TUSA staff
- **Approve** to send the report to the nominated investigator

The investigator will receive an email notification that they’ve been assigned.

**Both fields are required, and this matters.** If an allocation is completed with either left blank, the investigation step has nobody assigned and closes itself as approved — no investigator, no findings, no notification to anyone. It looks identical to a finished investigation. Making both fields required is what prevents that.



### **Step 2: Investigation**



The assigned investigator works on the investigation in their workflow inbox. The investigation form includes:


| Field | Purpose |
| ------------------------------------ | ---------------------------------- |
| **Assigned team** | Which team is handling this |
| **Investigator** | Who is investigating |
| **Notes, findings, recommendations** | Investigation details and outcomes |
| **Signature** | Investigator’s sign-off |


The investigator can:

- Work over multiple sessions (Save & Continue is available)
- See the original report details (prefilled for reference)



### **Step 3: Close the Investigation**



When the investigation is complete:

- Fill in the notes, findings, and recommendations
- Add your signature
- **Approve** in the workflow inbox to close the investigation

There is no “status” field to update — approving the workflow step closes the investigation.

When an investigation is closed, whether approved or rejected, a notification now goes to the assigned team. Nothing was sent previously.



### **Reassigning an Investigation**



The investigator cannot reassign the investigation themselves, and **editing the “Investigator” field after the step has started does not move it** — Gravity Flow works out the assignee when the step begins, so changing the field afterwards updates the record but not who holds the task.

To actually reassign, someone with Gravity Flow admin access uses “Send to Step” to push the entry back to the allocation step. That is currently Renee de Villeneuve, Shauna Lee Ward, Chris Vinaviles, Hannah Robinson, Johana Tincu and Bronwyn Brown.

---



## **Anonymous vs Named Reports**



&nbsp;

### **Anonymous Reports**



**What you DON’T have:**

- Reporter’s name
- Contact details
- Ability to follow up with reporter

**What you CAN do:**

- Investigate based on information provided
- Take action if sufficient detail
- Record for pattern tracking

**Important:** The system ensures anonymous reports truly contain no identifying information. Don’t try to identify anonymous reporters.



### **Named Reports**



**What you have:**

- Reporter’s identity and contact details
- Ability to contact for more information
- Their stated preference for contact

**Follow their wishes:**

- If they don’t want to be contacted, respect that
- If they want updates, keep them informed (per policy)

---



## **Manual Report Entry**



For reports received by phone, email, or in person:

**Where:** TUSA Internal → Reports → **New** sub-tab

This uses the same multi-page reporting form that reporters use online. Fill it out on their behalf:

- Complete the form with details provided
- Select appropriate incident type (this determines routing)
- Indicate how the report was received
- Submit

The system will:

- Create the report record
- Automatically create an investigation
- Route to the appropriate team

---



## **Access Restrictions**



**Strict access controls protect sensitive reports:**


| Role | What They Can See |
| ------------- | ----------------------------- |
| General staff | Only reports assigned to them |
| SASH team | SASH-related reports only |
| Advocates | Reports assigned to advocates |
| Admin | Reports in their area |


**Through the workflow, you cannot see:**

- Reports assigned to other teams
- SASH reports (unless you’re on the SASH team)
- Investigation details you’re not assigned to

This is intentional — it protects reporter confidentiality and ensures appropriate handling.



### **Important limit on that**



**The protection above describes the workflow, not the whole site.** Routing controls which queue a report enters. It does not control who can browse form entries in the WordPress admin.

Members of the Clubs admin team (`tusa_admin_clubs`) hold `gravityforms_view_entries` and `gravityflow_status_view_all`, so they can open investigation entries and view workflow statuses directly, **including SASH ones**, without ever being assigned. Administrators can too.

If SASH content must be unreadable to the Clubs team, that needs a permissions change, not a routing change. Flagged 2026-08-19 and not yet actioned, because narrowing that role also affects grants and club documents.

---



## **Common Situations**



&nbsp;

### **“I received a report that should go to another team”**



If a report seems miscategorised:

- Don’t reassign it yourself unless you have permission
- Contact your manager
- They can arrange proper routing via Gravity Flow admin



### **“The reporter wants to change from anonymous to named”**



- They would need to submit a new report with their details
- Note this in the investigation if relevant
- You cannot retroactively add details to an anonymous report



### **“I need more information but the report is anonymous”**



**You cannot contact an anonymous reporter.** Work with what you have, or:

- Note in investigation that insufficient information was provided
- Close if no action possible
- Record for pattern tracking



### **“Someone is asking about a report”**



**Do not confirm or deny reports exist** unless:

- They are the assigned investigator
- They are authorised management
- They are the reporter asking about their own named report



### **“I accidentally saw a report I shouldn’t have access to”**



- Don’t read further
- Don’t discuss what you saw
- Report the access issue to your manager
- This may indicate a permissions configuration problem

---



## **Quick Reference: Where Things Live**




| Need to Find | Where to Go |
| ----------------------- | ------------------------------------------ |
| Reports assigned to you | Your workflow inbox |
| All received reports | TUSA Internal → Reports → Received Reports |
| Investigations | TUSA Internal → Reports → Investigations |
| Manual entry form | TUSA Internal → Reports → New |


---



## **Getting Help**



Incident handling can be challenging. Remember:

- **Policy questions** → Your manager or policy documents
- **System issues** → IT/developer support
- **Personal support** → EAP or support services if dealing with difficult content

