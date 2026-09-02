---
title: The Annual Student Confirmation
hide:
  - toc
---
# **The Annual Student Confirmation**

Once a year, from **May 1st onwards**, every member who’s marked as a current student gets asked to confirm whether they’re still studying. This page explains what the prompt is, who sees it, what happens when members respond, and what TUSA staff need to do about the consequences.

The student-facing experience is built into the site — there’s no setup per member, the system just runs. Your job as TUSA staff is to monitor what happens *after* members start responding, especially the impact on club committee composition.

---



## **Why This Exists**



TUSA is funded by SSAF (the Student Services and Amenities Fee), which only enrolled students pay. To stay accurate and compliant, TUSA needs to know which members are currently students vs which have moved on to associate status.

Without an annual check-in, the membership data drifts year on year. People graduate, take leave, finish their course — but unless they actively update their profile, the records still show them as students. That distorts SSAF figures, club composition reporting, and the comms each member receives.

So once a year, every member who’s still flagged as a student gets a one-question prompt. They click yes or no, and the system updates accordingly.

---



## **When the Prompt Appears**



**From May 1st each year.** The date is deliberate:

- Semester 1 census: 17 March
- Withdrawal-without-fail deadline: 20 April
- By 1 May, enrolment data is settled

Before May 1st nothing fires. From May 1st onwards, eligible members start seeing the prompt the next time they log in.

Once a member responds (yes OR no), they won’t see it again until the *following* year. There’s no “ask twice” or “remind in 3 months.”

If a member dismisses the prompt without answering, it comes back next page load — across sessions. Dismissal is treated as “ask me later, not now.”

---



## **Who Sees the Prompt**




| Will see it | Will not see it |
| --------------------------------------------------------- | -------------------------------------------------------------- |
| Members marked as current students in their profile | Members already marked as associates (or any non-student type) |
| Students who are also TUSA employees, board members, reps | Club president / committee role accounts (see below) |
| Students who are members of any club | Anyone who’s already confirmed this year |


### **Why club leader accounts are skipped**



When a club has a “president account” or “committee account” (e.g. `president@theclub.tusa.utas.edu.au`), that account represents the **role**, not the human filling it. Whether the role-holder is a student is captured during the annual reaffiliation process, not by this prompt.

The actual person behind the role has their own personal account, and *that* account will get the prompt like any other student.

If a club president is using their personal account as the group admin (instead of a separate role account), they’ll be skipped here — which isn’t ideal — but their student status is still captured during reaffiliation.

---



## **What Members Experience**



A popup appears on page load:

> **Are you still a student?**

> Each year we ask our student members to confirm their status. This helps us ensure you receive the right benefits and information. We’ll keep asking until you confirm — it only takes a second!

> > **[YES! Still a Student]** **[NO! Not a Student]**



### **If they click “YES! Still a Student”**



- Their confirmation is recorded for the year
- They see a thank-you with a prompt to also update their campus or course if anything’s changed
- A **Visit My Profile** button takes them to their profile edit page
- They won’t see the prompt again until the next May



### **If they click “NO! Not a Student”**



- Their profile updates: profile type changes from Student to Associate, and the underlying student-status field changes to “No, I am not currently a student”
- Their tags update through the standard sync (the Student tag is swapped for associate-level tags)
- They see a friendly message that switching to associate status doesn’t affect their level of access
- A **Visit My Profile** button is offered for any further updates
- They won’t see the prompt again — they’re no longer a student in the system



### **What stays the same when they say no**



- Their account stays active
- They keep their club memberships
- They keep access to anything an associate can access (most of the site)
- Their club admin / committee status (if any) stays attached — but their *student* status now reads as no, which feeds into club composition reporting

They are **not** logged out, locked out, or removed from anything. The transition is administrative, not punitive.

---



## **What TUSA Staff Need to Monitor After May**



The annual confirmation is largely self-running, but there are knock-on effects you need to watch for.



### **Club committee composition**



Clubs must maintain **at least 50% students on their executive committees**. A president can be a non-student, but associates can’t exceed 50% of the exec.

When committee members transition student → associate via the May confirmation, **their club’s ratio shifts**. Some clubs will dip below 50%. You need to:

- After May (when confirmations are flowing in), run the All Clubs member export
- Check each club’s student vs non-student counts
- Flag clubs whose executive committees drop below the 50% threshold
- Reach out to those clubs — they’ll need to either recruit student members onto the exec or have someone reaffirm a different status



### **Three sources of student status**



Don’t conflate them — they each have a different role:


| Source | When | What it does |
| ------------------------------------ | ------------------- | ----------------------------------------------------- |
| **Registration** | Account creation | Sets initial student/non-student status |
| **Annual confirmation** (this guide) | From May each year | Confirms or transitions student → associate |
| **Reaffiliation** | Annual club renewal | Captures committee composition; handles role accounts |


If someone’s status seems wrong, work out which source captured it most recently — that’s the one driving their current state.

---



## **When the Prompt Should Have Fired But Didn’t**



Occasionally a member will tell you they should be seeing the confirmation but aren’t. Walk through:


| Check | What to look for |
| -------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------- |
| **Is it May or later?** | Before May 1st, the prompt doesn’t fire — that’s by design |
| **Is their profile flagged as student?** | If their profile already says “No, I am not currently a student”, the prompt doesn’t fire (no need — they’ve already declared) |
| **Have they already confirmed this year?** | Check their confirmation-year metadata in their profile. If it shows the current year, they’ve already responded |
| **Are they a group admin?** | Group admins are skipped on purpose. If their status needs updating, do it through reaffiliation or a manual profile change |
| **Have they recently changed profile type?** | If they were just upgraded from associate to student (e.g. via a profile update), the system will catch them at the next page load |


If none of those explain it, contact whoever maintains the site — there may be a bug to look at.

---



## **Manually Resetting for Testing**



If you have admin access and want to test the prompt yourself:

- Log in as an admin
- Go to any admin-area page and add `?reset_student_confirm=1` to the URL (e.g. tack it onto your dashboard URL after a `?`)
- You’ll see a confirmation banner saying the reset has happened
- Log out and back in — the prompt should fire on your next page load

This only resets *your own* confirmation. It doesn’t affect other members.

---



## **Common Situations**



&nbsp;

### **“A member said NO by mistake — they ARE still a student”**



Their profile type and student-status field have been changed. Fix it manually:

- Open the member in the admin area → Users
- Open their profile → switch profile type back to Student
- Update the student-status field back to “Yes, I am currently a student”
- Save

The prompt won’t re-fire for them this year (they’ve already “responded”), but their status is corrected for everything else.



### **“A club’s ratio dropped below 50% after May”**



Reach out to the club. Their options are typically:

- Recruit more student members onto the exec to rebalance
- Reaffirm a non-student member’s status if it was changed in error
- If genuinely below 50% with no fix, flag for follow-up at next reaffiliation



### **“A student’s prompt keeps coming back even after they answered”**



This shouldn’t happen — once they respond (yes or no), the pending flag clears. If a member reports this, ask them:

- Did they actually click one of the buttons, or just close the popup? Closing without clicking re-shows it.
- Did the click actually register? (network errors can cause silent failures)

If they confirm they clicked but it keeps appearing, there’s likely a bug — escalate to the site administrator.



### **“We need to mass-reset confirmations” (e.g. testing or annual cycle restart)**



This isn’t currently supported by a UI tool. Contact the site administrator — it requires a database-level operation.



### **“A member became a student mid-year (e.g. enrolled at mid-year intake)”**



If someone updates their profile from associate to student between January and April (before the prompt window opens), they’ll get the prompt the next May like any other student.

If they update after May 1st, they won’t get the prompt that year — but they’re already explicitly confirmed as a student via the profile update they just submitted. The prompt will fire for them the *following* May.

---



## **Quick Reference**



&nbsp;

### **What you do, when**




| When | What |
| ------------------ | -------------------------------------------------------------------- |
| Year-round | Nothing — the system runs itself |
| Early May | Watch for confirmations starting to come through |
| Through May–June | Monitor the All Clubs export, flag any clubs below 50% student ratio |
| Mid-year if needed | Manual reset / fix for individual members |
| End of year | Reaffiliation cycle handles role accounts and committee composition |


### **Where to look**




| For… | Go to |
| ------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Checking a member’s confirmation status | Admin area → Users → open the user → check their student-status field |
| Resetting your own confirmation for testing | Add `?reset_student_confirm=1` to any admin-area URL |
| Club student/non-student composition | All Clubs member export |
| Bigger picture of profile types and updates | [Managing User Registrations](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/user-management/the-annual-student-confirmation/managing-users.md) |
| The system underneath this | `STUDENT-CONFIRMATION-EXPLAINER.md` (design spec) |


---



## **Related Guides**



- [Managing User Registrations](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/user-management/the-annual-student-confirmation/managing-users.md) — broader user management, profile types, junior members
- [Checking Profile Update Claims](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/user-management/the-annual-student-confirmation/checking-profile-claims.md) — when members manually change their own affiliation through the profile form
- [Approving Clubs / Reaffiliation](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/user-management/the-annual-student-confirmation/approving-clubs.md) — the annual reaffiliation that captures committee composition

  
