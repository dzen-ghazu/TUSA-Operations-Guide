---
title: Handling Club Hire Orders
hide:
  - toc
---
# **Handling Club Hire Orders**

This guide is for TUSA staff who handle club equipment hire during the event approval process. It covers what to check on a hire order, when to charge, how to adjust pricing, how to invoice, and what to do if an event isn’t approved.

The club-side equivalent (what clubs do to *place* hire orders) is in [Hiring Equipment from TUSA](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/events/club-guide/gear-hire.md). This guide covers the staff side.

---



## **How the Hire Process Works (the staff view)**



When a club hires equipment for an event, this is the flow:

- **Club places the hire order first.** Eligible users (club presidents, club admins, TUSA staff) get an automatic 100% discount coupon at checkout. The order completes at $0.
- **Stock is reserved on checkout.** The equipment is held for the dates they specified.
- **Club submits their event application.** They enter the hire order number in the “Hire order number” field on the event application.
- **You review the event application AND the linked hire order together.** The hire order is *not* automatically tied to the event in the system — it’s a procedural link via the order number on the form.
- **You decide what happens to the hire order** based on the event approval outcome.

> The 100% discount is **provisional**. It auto-applies so the club can secure the booking, but you make the final call on whether they actually pay nothing, pay something, or have the order cancelled.

---



## **Three Outcomes**



When you finish reviewing the event application, the hire order needs one of three resolutions:


| Outcome | What you do | What happens to the order |
| ----------------------------------- | ------------------------------------------------------------------------ | ----------------------------------------------------------- |
| **Full discount** | Approve the event, leave the hire order alone | Order stays at $0, equipment ready for pickup |
| **Partial discount or full charge** | Approve the event, then adjust the hire order price and invoice the club | Order moves to “pending payment”, equipment held until paid |
| **Event rejected** | Reject the event application, then cancel the hire order | Stock released back to the catalogue |


---



## **Finding the Hire Order**



Each event application has the club’s hire order number in the **Hire order number** field. Use that to find the order.


| From | How |
| ---------------------------- | ------------------------------------------------------------------------------------------- |
| **Order number on the form** | Open Orders in the admin area → search by order number → open the order |
| **Club’s name** | Open Orders → filter by customer (the club admin / president account that placed the order) |
| **Date range** | Filter by date if you know roughly when they ordered |


Open the order to see what they’ve booked, the dates, and confirm it matches the event application (e.g., the dates they hired equipment for align with the event date, the equipment matches what they described).

---



## **Verifying the Order Against the Event**



Before deciding the outcome, do a sanity check:


| Check | What to look for |
| ------------------------------------- | ----------------------------------------------------------------------------------------------------------- |
| **Dates align** | Hire dates cover the event date plus any setup/packdown |
| **Equipment matches** | What they ordered matches what they said they’d need in the event app |
| **Pickup location** | They’ve selected a location they can actually get to (Hobart vs Launceston warehouse) |
| **No suspicious quantities** | Quantities are reasonable for the event size — flag if a small members’ meeting somehow needs five marquees |
| **All hire items, no other products** | Hire orders can’t have non-hire items — this should already be enforced at checkout, but worth a glance |


If something’s off, return the event application for amendment with a note explaining what needs to change. The club can update the order (or place a new one) and resubmit.

---



## **Outcome 1: Full Discount**



This is the default — most club events get the full discount.

**What you do:** Approve the event. Leave the hire order as is. The order stays at $0 and the equipment is ready for the club to collect on the booked dates.

No further action needed. The club already knows their order is at $0 from when they checked out.

---



## **Outcome 2: Partial Discount or Full Charge**



If TUSA’s policy says this club / this event / this equipment isn’t fully covered (or only partially covered), you adjust the order so the club pays the difference.



### **Step-by-step**



- **Approve the event application** in your Workflow Inbox first — this publishes the event so they can run it. The hire-order pricing is a separate workflow.
- Open the hire order in the admin area.
- **Remove the discount coupon.** Edit the order, find the “Club Equipment Hire (100% off)” coupon, remove it. The order total updates to the standard hire price.
- **Adjust line items if needed.** If the club is paying a partial amount (not the full standard price), edit each line item’s price to the agreed amount, OR add a fee row with a negative amount labelled (e.g.) “TUSA partial subsidy -$50”. Either approach works — pick whichever’s clearer for the order summary.
- **Update the order.** Save changes.
- **Send the invoice.** Open the order’s actions menu and choose “Email invoice / order details to customer.” The club gets an email with the new total and a “pay now” link.
- **Add an order note** documenting why the price was adjusted. e.g., “Partial discount — event is fundraising for external charity, policy doesn’t cover full subsidy. 50% subsidy applied per [your name].”



### **What the club sees**



- An email with the invoice and a payment link
- The order in their account showing “pending payment”
- Once they pay, the order moves to “processing” and they can pick up the equipment



### **Equipment release**



Equipment isn’t physically released until payment is confirmed. The Hire Store team handles the actual pickup — they’ll see the order status and only release equipment for orders that are paid (or remain at $0).

---



## **Outcome 3: Event Rejected**



If you reject the event application, the hire order needs to be cancelled so the stock goes back to the catalogue.



### **Step-by-step**



- **Reject the event application** in your Workflow Inbox with a note explaining why.
- Open the hire order in the admin area.
- **Change the order status to “Cancelled”** and save.
- **Add an order note** stating the event wasn’t approved. e.g., “Event application not approved — order cancelled and stock released.”
- The club is automatically notified by email of the cancellation.

If the club resubmits a corrected event application, they’ll need to place a new hire order — the cancelled one isn’t reactivated.

---



## **Common Situations**



&nbsp;

### **“The club placed an order but never submitted an event application”**



You’ll see a hire order at $0 sitting there with no matching event application. Reach out to the club admin who placed it and ask whether they’re still planning to submit. If not, cancel the order to release the stock.

You can find these by filtering the orders list to “Hire Store” + recent orders, then cross-checking against pending event applications in your Workflow Inbox.



### **“The order number on the event app doesn’t exist”**



Most likely the club typed it wrong. Open the orders list, filter by their account, and find the actual order. If you can’t find one, return the event application asking them to confirm the order number — they may have submitted the event app before completing checkout.



### **“The hire dates don’t cover the event date”**



E.g., event is Saturday 3pm, hire is Saturday 10am to 2pm. Return the event application asking the club to update the hire order with corrected dates. They’ll need to contact the Hire Store to amend the order or cancel and re-place.



### **“External NFP wants to hire equipment too”**



That’s a different workflow — see “Manual Orders for External Parties” in the [Event Approval guide](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/events/handling-club-hire-orders/event-approval.md). External hire isn’t part of the auto-discount system; it’s a manually-created order with a custom discount applied case-by-case.



### **“The club asked to extend their hire dates after approval”**



Open the order, edit the line item dates, save. Check stock availability for the extra days first — if something else is booked then, the extension can’t go through and you’ll need to tell them.



### **“A club says their order shows the wrong amount”**



Check whether you’ve already adjusted the order. If you’ve removed the coupon and they’re seeing the standard price, that’s the post-adjustment view. Confirm with them what they were expecting — it may be that the policy outcome wasn’t communicated clearly.



### **“We accidentally charged the club but they should’ve had the full discount”**



Open the order, re-apply the “club-equipment-hire” coupon, save. If the club already paid, refund them through the order’s refund tools and add an order note explaining what happened.

---



## **When NOT to Use This Process**




| Situation | What to do instead |
| ------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| External NFP hiring for a TUSA event (e.g., NFP stallholder at SLE) | Manual order with case-by-case discount — see [Event Approval](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/events/handling-club-hire-orders/event-approval.md#manual-orders-for-external-parties) |
| General public renting equipment | Standard checkout, no discount, full price applies |
| TUSA-run event hiring its own equipment | TUSA staff are eligible for the auto-discount, same flow as clubs |
| Internal stock movement between Hobart and Launceston warehouses | Not an order — handled by Hire Store team directly |


---



## **Quick Reference**



&nbsp;

### **Resolution checklist**



&nbsp;

```
[ ] Event application reviewed
[ ] Hire order found via the hire order number on the application
[ ] Dates and equipment cross-checked against event details
[ ] Outcome decided (full / partial / cancel)
[ ] Event application action taken (approve / reject)
[ ] Hire order action taken (leave / adjust + invoice / cancel)
[ ] Order note added documenting the decision

```



&nbsp;

### **Where to look**




| For… | Go to |
| ---------------------------------- | ----------------------------------------------------------- |
| Event applications awaiting review | Workflow Inbox in the admin area |
| The linked hire order | Orders → search by the hire order number on the application |
| All recent hire orders | Orders → filter by Hire Store / Vendor 76 |
| A specific club’s hire history | Orders → filter by customer |
| Order email + payment status | Open the order → Order details panel |


---



## **Related Guides**



- [Event Approval](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/events/handling-club-hire-orders/event-approval.md) — the broader event approval process (categories, ticketing, manual orders for externals)
- [Hiring Equipment from TUSA](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/events/club-guide/gear-hire.md) — the club-side guide that this is the staff equivalent of
- [Managing Hire Store Products](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/events/handling-club-hire-orders/managing-hire-store.md) — adding/managing the rental items themselves (not the order workflow)

  
