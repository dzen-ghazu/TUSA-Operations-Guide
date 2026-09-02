---
title: Moderating Reviews
hide:
  - toc
---
# **Moderating Reviews**

Reviews are public — they appear on the product or event page once approved, with the reviewer’s name and rating contributing to the public average. This page covers the workflow for approving, rejecting, editing, and replying to reviews after they’re submitted.

For information on building the forms that collect reviews, see [Managing Review Forms](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/eois-feedback/moderating-reviews/managing-review-forms.md). This page is about what happens after a review is submitted.

---



## **What needs your attention**



When someone submits a review, one of three things happens:

- **It goes into the moderation queue** — pending your approval. It does NOT show on the product or event page yet.
- **It auto-publishes** — appears immediately if its rating is at or above your auto-approve threshold (see below).
- **It bounces** — the spam filter caught it, or it failed validation. Rare; you’ll see it in the spam folder if so.

Your job in moderation is to look at queued reviews and decide: approve, reject, mark as spam, or edit-then-approve.

---



## **The auto-approve threshold**



Under **Tracksies → Reviews → Settings → Moderation** there’s a star-rating threshold that controls auto-publishing:

- **Threshold of 0 (or “Manual moderation”)** — every review goes to the queue. Nothing publishes without you.
- **Threshold of 4** — reviews of 4 stars or higher publish immediately. 1–3 star reviews queue for your decision.
- **Threshold of 5** — only 5-star reviews auto-publish. Everything else queues.

Pick the level your team can keep up with. Common patterns:

- **High-trust, low-volume:** Threshold of 4 or 5. Mostly auto-publish, you only need to look at the lower ratings (which are also the ones most likely to need a thoughtful response anyway).
- **High-volume, sensitive content:** Threshold of 0. Everything queues. More work but nothing surprising goes public.
- **Mixed:** Threshold of 4 is a reasonable default — quickly publishes positive reviews while giving you a window to handle negative ones before they’re public.

Reviews submitted with photos still go through this same threshold — there’s no separate gate for photos.

---



## **Where to find pending reviews**



**Tracksies → Reviews → Moderation**

The Moderation tab shows everything awaiting approval. The pending count appears as a red badge next to the menu item, so it’s visible from anywhere in the admin.

You can also see all reviews regardless of status under **Tracksies → Reviews → All Reviews** — useful for finding an already-approved review to edit, reply to, or remove.

---



## **Per-review actions**



Each pending review has these actions available:


| Action | What it does |
| ----------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Approve** | Publishes the review. Appears on the product or event page; counts toward the public average. |
| **Reject** | Holds the review. Stays out of public view. The reviewer isn’t notified. Useful when a review is borderline — keeps it for later, no commitment either way. |
| **Spam** | Marks as spam. Stays hidden, and the system learns from the pattern. Use for obvious junk (link spam, off-topic ads, abuse). |
| **Edit** | Open the full review for editing — fix typos, trim PII, normalise capitalisation. Edits are silent (no notification to the reviewer). |
| **Feature** | Mark a review as “featured” — appears highlighted in the reviews display, often pulled into homepage or marketing surfaces. Useful for showcasing a particularly good review. (Pro only.) |
| **Delete** | Permanent removal. The review row goes; the rating it contributed is removed from the average. No undo. |


### **When to edit before approving**



- **Personally-identifying information** in the review body (full names of staff or other students, phone numbers, addresses). Trim it.
- **Profanity or harassment** — depending on the policy, either reject outright or edit out and approve.
- **Out-of-context references** — “I bought this with the order I made on the 15th” — usually fine to leave, but if the date/order detail is misleading, trim.
- **Off-topic but otherwise positive** — a review of a wetsuit that’s mostly about the staff member who fitted it. Edit to be about the product, or reject and ask the reviewer to resubmit via Feedback if the comment is about staff.

Edits don’t notify the reviewer. The published review will be the edited version.

---



## **Replying to reviews (owner responses)**



You can publicly reply to any approved review. The reply appears underneath the review on the product or event page, marked with your name (or “TUSA” or whatever owner identity is configured) so visitors can see it’s the official response.

To reply:

- Open the review in **Tracksies → Reviews → All Reviews**
- Click **Reply**
- Write your response. Plain text, no formatting.
- Save.

The reply is public immediately — there’s no separate moderation gate for owner responses (since the staff person posting it is already trusted).

When to reply:

- **Critical or 1–2 star reviews** — always worth a thoughtful response. Acknowledge the issue, describe what’s been done. Public replies on negative reviews often help future visitors more than the original review hurts.
- **Detailed positive reviews** — a brief thanks adds warmth and shows you’re paying attention.
- **Reviews asking a question** — answer in the reply rather than leaving it hanging.

When NOT to reply:

- **Defensive responses to negative reviews.** A defensive reply makes the negative review look worse, not better. Walk away from these or wait until you can write something measured.
- **One-line “thanks” replies on every positive review.** Looks spammy and dilutes the value of the replies that matter.

---



## **Photos and moderation**



If you’ve enabled photo reviews (see [Managing Review Forms](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/eois-feedback/moderating-reviews/managing-review-forms.md) → “Letting reviewers attach photos”), photos go through the **same moderation gate as the review text**. There’s no separate “approve photo” step:

- A queued review with photos shows the photos in the moderation view. Approve = photos and text both go public. Reject = both stay hidden.
- An auto-approved review with photos publishes both immediately. (If your auto-approve threshold lets a 5-star review through, the photos publish with it — without you seeing them first.)

If you want the option to approve text but not the photo (e.g. a 5-star review with a blurry photo you’d rather not show), the workflow is:

- Edit the review
- Remove the photo from the review
- Approve

Or, if your policy is “every photo needs eyes on it before it’s public,” set the auto-approve threshold to 0 (manual moderation for everything) — that’s the only way to guarantee a human sees every photo before publish.

---



## **Notifications**



Trustie has its own notification setting under **Tracksies → Reviews → Settings → Reviews**, separate from WordPress’s built-in comment notifications. Two fields:

- **“Send email when a new review is submitted”** (checkbox) — turns notifications on or off.
- **Notification Email** — the address that gets the email. Defaults to the site admin email. Change it to a shared staff inbox (e.g. `reviews@tusa.utas.edu.au`) to keep all review notifications in one place.

There’s a separate Notification Email under Testimonial settings if you want testimonials and product reviews routed to different inboxes.

A few things to know:

- The notification fires for **every review submitted**, regardless of whether it’s auto-approved or held for moderation. There’s no “only pending” filter and no daily digest — one email per review.
- WordPress’s built-in **Settings → Discussion → Email me whenever** options can also fire notifications for the same reviews, since reviews are stored as comments. To avoid double emails, leave WordPress’s “Anyone posts a comment” / “A comment is held for moderation” boxes off and rely on Trustie’s Notification Email instead.
- If notifications start to feel like noise on busy days, the practical move is to turn the toggle off and check the Moderation tab on a schedule — the red badge counter is always accurate.

---



## **Common gotchas**



- **An auto-approved review can’t be “un-auto-approved” retroactively.** Once it publishes, it’s public. You can unapprove it after-the-fact (it disappears from the page) but it was visible in between.
- **Editing the rating after approval** — the rating CAN be edited, and the public average will recalculate to match. But this is unusual; the right move is usually to edit just the text.
- **A spam-marked review’s rating stays out of the average.** Spam is hidden completely.
- **A featured review still counts toward the average** — featuring is purely visual highlighting, not a different category. To exclude a review from the average, reject or delete it instead.
- **Photos and review text share fate.** No way to approve text but reject photo, or vice versa, without manually editing the photo out of the review first.
- **Reviewers don’t see review status.** Whether you approve, reject, or hold a review, the reviewer doesn’t get a notification or a status update. They submitted; they don’t know what happened. If you reject a review and want them to know why, that’s a manual outreach conversation outside the review system.

---



## **Related**



- [Managing Review Forms](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/eois-feedback/moderating-reviews/managing-review-forms.md) — building custom review forms and assigning them
- [Managing Feedback Forms](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/eois-feedback/moderating-reviews/managing-feedback.md) — for non-product, non-event input
- [Managing Event Feedback](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/eois-feedback/moderating-reviews/managing-event-feedback.md) — automatic post-event feedback on Event Calendar entries

