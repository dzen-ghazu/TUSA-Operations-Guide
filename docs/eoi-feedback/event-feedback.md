---
title: Managing Event Feedback
hide:
  - toc
---
# **Managing Event Feedback**

This guide covers the **automatic post-event feedback** that runs on every event in the Event Calendar. It’s separate from the [Feedback Forms](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/eois-feedback/managing-event-feedback/managing-feedback.md) system — you don’t set anything up per event, the feedback collection just appears once an event has ended.

---



## **What This Is**



Event feedback **ties into the same review system used for product reviews on the store side** — same star rating, same review storage, same admin moderation view. The event page just adds a few extra training-shaped questions on top of the standard star rating.

Every event on the Event Calendar gets the feedback form on its single page **automatically**, with one rule: it only appears once the event’s end date has passed. Before that, the section is hidden. There’s nothing to configure per event.

The form captures:

- A **star rating** (1–5) — required, the same star rating used on store products
- **Eight optional questions** about the experience (training value, content level, expectations, duration, recommendation, presenters)
- **Two free-text questions** — what other information would have been useful, and any other feedback

Submissions land in the same place store product reviews land: as **reviews on the event** (technically a review-type comment), with the rating recorded against the entry. The event page then shows the reviews publicly with the average rating at the top, using the same star styling as product reviews. Reviews are tagged with an event marker so they can be told apart from product reviews when needed.

---



## **What Attendees See**



&nbsp;

### **Before the event ends**



Nothing. The reviews section on the event page is hidden until the end date passes.



### **After the event ends**



The reviews section appears with three parts:

- **Average rating** — calculated from all reviews submitted so far, displayed as stars.
- **The review form** — the star rating, optional radio questions, and the two text questions. Visible to logged-in users who haven’t already reviewed and (per the page template) have a ticket for the event.
- **Submitted reviews** — public list of every review for this event, newest first, privacy-protected (shows “FirstName L.” not full names).



### **Who can submit**




| Condition | What enforces it |
| ---------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Logged in | The form processor rejects logged-out submissions, and the page shows a “you must be logged in to review an event” message instead of the helper text. |
| Hasn’t already reviewed this event | The form processor checks the comments on this event for an existing review by this user — if one exists, it returns an error message pointing them to email `hello@tusa.utas.edu.au` instead. One review per user per event. |
| Bought a ticket for this event | This is a *page-level guidance condition*, not a hard gate. The “Your review will be submitted from {name}, at {email}” prompt text only shows when the user has bought a ticket for this event. The form itself isn’t hidden if they haven’t — but the lack of the prompt is intended to discourage non-attendees from leaving reviews. |


So in practice: logged-out visitors and people who already reviewed get a clear stop message. Logged-in users who didn’t buy a ticket will see the form but no prompt encouraging them to use it — and any review they did leave would still save (the system trusts the page-level guidance for this).

---



## **What Questions Are Asked**



The form is set up for **training-style and workshop-style events**. The questions don’t fit a stallholder market or an external speaker night without adjustment, so use your judgement when launching events that don’t match this shape — attendees can skip the optional questions, but the form is most useful when the questions match the experience.


| Question | Type | Required? |
| ---------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------ | --------- |
| Your overall rating (1–5 stars) | Star rating | Yes |
| Was this training valuable for you? | Radio: Excellent Value / A lot of Value / A bit of Value / No Value / Not Applicable | Optional |
| Was this information delivered at the right level for your knowledge/expertise? | Yes / No | Optional |
| Were the expectations you had about the training/workshop met? | Yes / Partially / No | Optional |
| Do you feel that the duration of this session was… | Too Short / Just Right / Too Long | Optional |
| Would you recommend this training to others? | Yes / No | Optional |
| Were the presenter(s) approachable and engaging? | Yes / No | Optional |
| Did the presenter(s) deliver the content effectively and sensitively? | Yes / No | Optional |
| Did the presenter(s) handle questions and discussion respectfully? | Yes / No | Optional |
| Is there any other information you would have liked to be included? | Free text | Yes |
| Have more feedback or comments for us? Anything we did great, or that could be improved? | Free text | Yes |


The two free-text fields being required means you always get qualitative feedback alongside the rating.

---



## **Where to Read Reviews**



&nbsp;

### **On the event page itself (public-facing)**



The reviews section on the event’s single page is the easiest place to skim. You see:

- The **average rating** as stars
- Each review’s star rating
- The reviewer’s name as “FirstName L.” (e.g., “Sarah C.” rather than full name)
- The structured radio answers (Training Value, Appropriate Level, etc.) as bold labels with the answer
- The two free-text responses
- Date submitted

This is the same view attendees and the public see, so it’s safe to share or reference.



### **In the admin area (full record + moderation)**



Because event reviews share the same review system as product reviews, they show up in the **same admin view as product reviews**. Two ways to find them:

**Option 1: Comments view**  
Go to **Comments** in the admin area. Filter by type **Reviews** — you’ll see product reviews and event reviews together. To see only event reviews, look at the “in response to” column and pick the ones tied to an event.

**Option 2: Products → Reviews** (the store reviews screen)  
Same data, the store’s dedicated reviews screen. Event reviews appear here too because they share the same review system.

Each review entry has:

- Full reviewer name (not the privacy-shortened version)
- Their email address
- The structured review content (all answered questions formatted)
- The individual answers stored alongside — the rating, each radio answer, the event it was for
- Standard moderation actions: Approve / Unapprove / Spam / Trash / Reply / Edit
- A “verified” flag — note this is set automatically on every event review, it isn’t checked against actual ticket purchase, so don’t rely on it as proof of attendance



### **Per event in admin**



You can also open the event post in the admin area and scroll to the comments section — you’ll see only the reviews for that specific event there.

---



## **Moderating Reviews**



Reviews are **auto-approved** when submitted. They appear publicly straight away. This is intentional — the form requires login, the user must have a ticket, and they can only submit once. The trust bar is high. But sometimes you’ll need to step in.



### **Inappropriate language or personal attacks**



- Find the review in **Comments** (the admin area)
- Click **Trash** to remove it from public view immediately
- If it’s targeting a specific person (e.g., naming a presenter and being personal rather than professional), consider also reaching out to the reviewer to understand the context — there may be a real complaint behind it that needs handling outside the public review system.



### **Off-topic content**



If a review is about something other than the event itself (e.g., a general TUSA grievance, a venue issue not related to the event), you can:

- **Reply** to the comment with a redirect — “Thanks for the feedback. For [topic] please contact [team]@tusa.utas.edu.au and we’ll handle it from there.”
- Or **Trash** if it’s not useful as a public review.



### **Spam**



The standard spam tools work. Mark as **Spam** in the admin area Comments — this trains the spam filter and removes the review from public view.



### **A reviewer wants their review removed**



They can email `hello@tusa.utas.edu.au` (the message they see when trying to review again says this). On request, find the review in the admin area Comments and Trash it.



### **A reviewer wants to amend their review**



The form is one-and-done — they can’t submit a second. Options:

- Trash their existing review and ask them to resubmit (loses the original)
- Trash and add the new feedback yourself as a comment on their behalf, with a note in the comment that this was re-submitted on date X

For substantive amendments the first option is cleaner.

---



## **Replying to Reviews**



You can reply to any review using the **Reply** action in the admin area Comments. Replies appear publicly under the review.

**When replying makes sense:**

- Acknowledging negative feedback (“Thanks for letting us know — we’re going to change the duration for our next session”)
- Correcting factual misunderstandings (“Just to clarify, the workshop was free for TUSA members, but you’re right that the booking page wasn’t clear about that”)
- Pointing them to a resource (“Glad you mentioned this — we have a follow-up resource at [link]”)

**When replying is a mistake:**

- Defending against criticism — let the rating speak; replies that argue make the original review worse, not better
- Reactive replies on a bad day — sleep on it



### **Tone**



Replies are public. Keep it warm, brief, specific. Always thank them for taking the time. Avoid generic “we’re sorry you had a bad experience” boilerplate — name the specific thing they raised.

---



## **Getting Attendees to Leave Feedback**



The single biggest gap in this system: **past events drop off the public Event Calendar listing**. Attendees who’d happily leave a review can’t find their way back to the event page after the event date has passed, because the calendar only shows upcoming events. The reviews form is on the event page — but they don’t know how to get there.

**The answer is to send them a direct link** within a day or two of the event ending. The event post still exists at its original URL — only the calendar *listing* hides it. A direct link works fine.



### **Find the URL of a past event**




| From | How |
| ------------------------------- | --------------------------------------------------------------------------------- |
| **The admin area** | Events → All Events → click the event → copy the URL. URL pattern is `/events//`. |
| **You already know the slug** | Just type `https://tusa-dev.its.utas.edu.au/events//` into your browser. |
| **You ran the event last year** | Same URL pattern works for any past event, no expiry. |


### **Send attendees the link**



You have a few options for getting the link to attendees:


| Option | When to use |
| ----------------------------------------- | -------------------------------------------------------------------------------------------------------------------------- |
| **Event attendee list** (per-event email) | Easiest for one-off events — the event calendar keeps an attendee list per event. Send them an email with the review link. |
| **Personal email to a small cohort** | Workshops with a handful of people — just email them by hand. |


### **Wording for the request**



Keep it short, name the event, link directly to the event page, set expectations on what the form asks. Example:

> Hi [Name],

> > Thanks for coming to **[Event name]** last [day]. We’d love your feedback so we can make our [training/workshops/sessions] better.

> > Leave a quick review here: **[direct link to event page]**

> > It takes about 2 minutes — a star rating, a few optional questions, and a couple of free-text fields if you want to say more. You’ll need to be logged in (the same account you used to book your ticket).

> > Thanks!

> [Your name], TUSA

Two things this wording does that matter: (1) **direct link** so they don’t have to search, (2) **mentions login** so they’re not surprised when the form asks them to sign in.



### **Timing**



The reviews form unlocks the moment the event end date passes (in the post-end-date window). Best results come from sending the request **1–3 days after the event** — fresh in their memory, but past the immediate post-event tiredness. After about 2 weeks, response rates fall off a cliff.



### **Setting up a recurring review-request workflow**



For events that run regularly (training cohorts, weekly sessions), it’s worth setting up a saved email template so the post-event request goes out consistently. Options:

- **Saved email template on the event** — sent as a one-off per event
- **Email automation** — triggered by an event-attended tag in the email tool, with a delay matching your preferred review window

If you want this set up across the team, talk to Sarah about wiring up an automation rather than each coordinator doing it manually.

---



## **How This Relates To Other Feedback**




| System | Where | When | What it captures |
| -------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------- | -------------------------------- | ---------------------------------------------------------------------------------------------------------- |
| **Event feedback** (this guide) | Auto on every Event Calendar entry | After end date | 1 rating + 8 optional radios + 2 free text, training-shaped — saved as a review on the event |
| **Product reviews** (TUSA Store / Hire Store) | Auto on every store product | Anytime after purchase | Star rating + comment, only verified buyers — saved as a review on the product |
| **[Feedback posts](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/eois-feedback/managing-event-feedback/managing-feedback.md)** | Manually configured per topic | Per the open/close dates you set | Configurable: ratings, topics, discovery, anonymous, custom questions — saved as a separate feedback entry |


The first two share the same underlying review system — applied to events on one side and store products on the other. The third is a separate purpose-built feedback system for everything that doesn’t fit either of those.

When someone asks “we want feedback after our [thing]”:

- **Is it on the Event Calendar?** Already covered automatically — send them to the event page after the end date.
- **Is it about a product?** Already covered by the product page reviews.
- **Is it about a campaign, an ongoing service, an opinion pulse, or anonymous input?** That’s a [Feedback post](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/eois-feedback/managing-event-feedback/managing-feedback.md).

---



## **Things to Know Up Front**



&nbsp;

### **Reviews don’t fire any notifications**



Submitting a review doesn’t email the event organiser or land in any workflow inbox. Reviews are public on the event page and visible in the admin Comments view — that’s where you read them. If you want to be told when reviews come in, open the event in the admin area and tick “Notify me of new comments” on that event.



### **The questions are training-focused on purpose**



Most TUSA events that use the Event Calendar are workshops, training, or sessions where the questions fit. For a market day or a stalls-style event, attendees usually skip the optional questions and just rate + leave free-text feedback. That’s still useful.



### **Reviews stay forever (unless you Trash them)**



Reviews don’t auto-archive. They sit on the event page indefinitely. For events that are run repeatedly (annual workshops, quarterly trainings), you can clone the event for the new run rather than reusing the same event post — that way each cohort’s feedback stays attached to the right run.



### **Reviews are privacy-protected on the event page, not in the admin area**



The public event page shows “FirstName L.” — but the admin Comments view shows the full reviewer name and email. Don’t share screenshots from the admin area externally.

---



## **Common Situations**



&nbsp;

### **“We just ran a training and want to send the reviews to the presenter”**



Open the event page → reviews section → screenshot the public reviews, OR open the admin Comments view → filter by event → copy/paste the structured content into an email. The admin view has full names (so use that for internal sharing) but check whether the presenter needs full names or just aggregate sentiment.



### **“An attendee wants to leave a review but the form isn’t there”**



Check:

- Has the event end date actually passed? Before that, the reviews section is hidden.
- Are they logged in? Logged-out visitors see a login prompt instead of the form.
- Did they buy a ticket? The “submit a review” prompt is template-conditioned on having a ticket.
- Have they already reviewed? One per user per event — the form is replaced by the “email hello@” message.



### **“We want to enable feedback before the event ends” (e.g., during a multi-day session)**



Not supported by this system — the visibility condition is hard-coded to the event end date. For mid-event feedback, set up a [Feedback post](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/eois-feedback/managing-event-feedback/managing-feedback.md) for that specific event week and link to it from the event page or the day-of materials.



### **“We want a different question set for this event”**



Not supported per-event — the questions are baked into the page template. If you want different questions, create a [Feedback post](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/eois-feedback/managing-event-feedback/managing-feedback.md) for that event instead and link to it from the event description. The auto event feedback will still appear, but most attendees will follow the link first.



### **“Reviews are showing for a draft / unpublished event”**



They shouldn’t — the form only shows on published events with a passed end date. If you’re seeing reviews on a draft, the event was previously published, attended, and reviewed, then unpublished. The reviews stay attached to the post.

---



## **Quick Reference**



&nbsp;

### **Where to look**




| For… | Go to |
| ---------------------------------------------------------- | ------------------------------------------------------------------------------------ |
| Reading reviews publicly | The single event page |
| Reading reviews in detail (full names, structured answers) | The admin area → Comments → filter Reviews (or Products → Reviews on the store side) |
| Replying to a review | the admin area → Comments → Reply |
| Removing a review | the admin area → Comments → Trash |
| Marking spam | the admin area → Comments → Spam |
| Subscribing to new reviews on an event | Open the event in the admin area, tick “Notify me of new comments” |


### **When you don’t need this guide**



- The thing isn’t on the Event Calendar → use a [Feedback post](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/eois-feedback/managing-event-feedback/managing-feedback.md)
- The thing is a product purchase → product reviews on the store side handle it
- The thing is a campaign/week-long programme → use a [Feedback post](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/eois-feedback/managing-event-feedback/managing-feedback.md) tied to the campaign as a whole

