---
title: Managing Review Forms
hide:
  - toc
---
# **Managing Review Forms**

Reviews are one of three ways to collect input from students and staff. The other two are [Feedback posts](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/eois-feedback/managing-review-forms/managing-feedback.md) and the [automatic post-event feedback](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/eois-feedback/managing-review-forms/managing-event-feedback.md) that runs on Event Calendar entries. Same-ish goal — different mechanics, different surfaces, different best fits. This page is about reviews, including custom review forms with extra structured questions beyond the default star rating.

---



## **Three ways to gather input**




| You want… | Use | Where it appears | What’s stored |
| ----------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------- | ---------------------------------------------------- |
| **A public 1–5 rating + comment on a product or event** | Default review (already on) | Product page or event page | A public review with the author’s name + star rating |
| **A public review with extra structured questions** (fit, course difficulty, recommendation, etc.) | **Custom review form** (this page) | Product page or event page (replaces the default) | A public review with the rating + extra answers |
| **Private input not tied to a specific product or event** (open suggestion box, surveys, campaigns, anonymous opinions) | [Feedback post](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/eois-feedback/managing-review-forms/managing-feedback.md) | Wherever you embed the form (its own page, a sidebar, etc.) | Private feedback that flows into the Workflow Inbox |


Reviews are **public by default** — they show on the product or event page with the reviewer’s first name and rating, contributing to the product’s or event’s average. Feedback posts are **private by default** — they go to staff inbox, never display publicly unless you explicitly choose to.

If the same goal could be met by either path, it usually comes down to: do you want this on the product/event page itself, or somewhere separate? On the page → review. Separate → feedback.

---



## **When you’d reach for a custom review form**



The default star + comment is enough for almost every product and event. Reach for a custom form when you have **specific structured questions** the rating + comment doesn’t capture, e.g.:

- Wetsuit fit feedback (size ran small / true / large)
- Course difficulty calibration (beginner / intermediate / advanced — was it pitched right?)
- Hire condition reporting (any damage, fit issues — feeds back to Hire Store ops)
- Workshop quality breakdown (content / presenter / pacing as separate ratings)

If the request is “we want a 1–5 rating and people to write what they thought” — the default already does that. No custom form needed.

---



## **Building a form**



- Go to **Tracksies → Reviews → Forms** in the admin menu.
- Click **Add New Form**.
- Give it a clear name (e.g. “Wetsuit fit feedback”, “Training course evaluation”). The name is internal — visitors don’t see it.
- Pick the **form type**:

– **Product Review** — for items in the TUSA Store or Hire Store  
– **Event Review** — for events on the Event Calendar  
– **Site / Store Review** — general business reviews not tied to a specific product or event

- Add fields. The first field is always the **star rating** (you can’t remove it — it’s what makes a review a review). Beneath the stars, add as many extra questions as you want.



### **Field types you can add**




| Field type | Use it for |
| --------------------------------- | --------------------------------------------------------------------------------------------- |
| **Short text** | One-line answers — name, location, “what surf level are you” |
| **Long text** | Multi-line — open feedback, what they’d improve |
| **Single choice** (radio buttons) | Pick one — fit (small / true / large), course difficulty (beginner / intermediate / advanced) |
| **Multiple choice** (checkboxes) | Pick any number — what topics were covered, which features matter |
| **Yes / No** | “Would you recommend this?” |
| **Rating** | A second star rating beside the main one — content quality, presenter, value for money |


For each field you can mark it **required** (visitor can’t submit until they fill it in) or optional, and you can show a help-text line under the field to guide them.



### **What visitors see**



The form appears underneath the existing star rating on the product or event page once they’re eligible to review (after purchase for products, after the event end date for events). The fields you added show in the order you put them in, with the help text underneath each.

---



## **Letting reviewers attach photos**



Photo uploads are a **site-wide setting**, not a per-form one. When enabled, every review form (default and custom) gets a “Add photos” upload control alongside the rating + comment.

To turn it on:

- Go to **Tracksies → Settings → Features**
- Enable **Photo Reviews** (sometimes labelled “User Generated Content”)
- Save

Once on, photos uploaded with reviews are auto-resized + compressed, attached to the review, and shown in a lightbox on the product or event page.

To turn it off — same path, untoggle. Existing photos on existing reviews stay; just no new uploads come through.

A few things to know before turning it on:

- It’s all-or-nothing across the site. You can’t have photos on wetsuit reviews but not on training reviews — if it’s on, every form gets the photo upload.
- Customer photos are user-generated content. The standard moderation workflow (approve/reject reviews before they’re public) still applies — photos go through that gate alongside the review text.
- Storage adds up over time. Photos live in the standard media library and count against any storage limits the host imposes.

---



## **Assigning a form**



A form on its own does nothing — it has to be **assigned** to something. The Assignment section on the form edit screen is where you decide where it appears.



### **Assignment scopes**



You can assign a form to any combination of:

- **All products** — applies to every product in the TUSA Store and Hire Store. Catch-all.
- **Specific products** — pick individual products by name. The form only appears on those.
- **Product categories** — pick categories (Wetsuits, Boards, Apparel, etc.). The form applies to every product in those categories.
- **All events** — applies to every event on the Event Calendar.
- **Specific events** — pick individual events.
- **Event categories** — pick event categories. Applies to every event in those categories.

You can also leave a form **unassigned** while you’re drafting it — it won’t appear anywhere until you assign it.



### **Which form wins when assignments overlap**



A product can match more than one form (e.g. you have one form assigned to the “Wetsuits” category and another to “All products”). The system walks the rules from most specific to least specific and returns the first match:

**For products:**

- **Specific product** — exact match by product
- **Product category** — match by one of the product’s categories
- **All products** — catch-all
- **Default review form** (set under Tracksies → Reviews → Settings, if any)

**For events:**

- **Specific event** — exact match
- **Event category**
- **All events**
- **Default review form**

So if you have a “Wetsuits” form and an “All products” form, every wetsuit gets the wetsuit form and every other product gets the all-products form.



### **Quick assignment patterns**



- **One form for every wetsuit, default elsewhere:** Form A assigned to “Wetsuits” category. No other rules.
- **A specific course needs its own questions:** Form A assigned to that specific event. Every other event uses the default.
- **All training events share one set of questions:** Form A assigned to the “Training” event category. Single events outside that category use the default.
- **Hire returns get a fit-and-condition form, store sales use a general form:** Form A assigned to Hire Store products (by category if Hire products share a category, or by individual product picker). Form B assigned to “All products” — applies to anything not in Form A’s scope.

---



## **Editing or removing a form**



- **Editing fields:** changes apply to all *future* submissions. Reviews already submitted under the old field set keep their original answers.
- **Renaming:** internal-only — won’t affect visitors.
- **Changing assignment:** takes effect immediately. If you remove a form from a product, the next visitor sees whatever the new most-specific match is (often the default star + comment).
- **Deactivating a form (toggle off):** form rules are skipped when looking up which form to use. Existing submissions stay.
- **Deleting a form:** the existing submissions stay (they’re stored as reviews, not as form responses). The form definition is gone, so no new submissions can come through it.

---



## **Common gotchas**



- **A product in two categories:** if Form A is on “Wetsuits” and Form B is on “Sale”, a wetsuit on sale matches both at the same specificity level. The form for whichever category appears first in the product’s category list wins. Category order in WordPress isn’t always intuitive — if you need a hard tiebreaker, **assign the form directly to the specific product** (level 1 specificity) and it will trump any category match.
- **Two “All products” forms active at once:** only the oldest one applies. Best practice: keep one “All products” form. If you need a second, deactivate the old one first.
- **Required fields apply to every visitor.** If a wetsuit form has a required “Wetsuit size” question and someone tries to review the wetsuit without picking a size, they can’t submit. Use required sparingly so people don’t bounce.
- **Event reviews don’t appear until the event ends** — even with a custom form assigned. The end date gate is by design and not configurable per event.
- **Removing a form from “All products” does NOT remove it from any specific product or category assignments** — those are independent rules. Check all four scope levels when retiring a form.
- **Custom forms replace the default star + comment for whatever they’re assigned to.** They don’t add fields to it — they replace it. If you want the default plus a few questions, just build a custom form with the star rating (default) plus the extra questions.

---



## **Related**



- [Managing Feedback Forms](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/eois-feedback/managing-review-forms/managing-feedback.md) — for non-product, non-event input (suggestion boxes, campaigns, surveys, anonymous opinions)
- [Managing Event Feedback](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/eois-feedback/managing-review-forms/managing-event-feedback.md) — the automatic post-event feedback that runs on every Event Calendar entry without a custom form

