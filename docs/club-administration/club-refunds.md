---
title: Handling Club Refunds
---
# **Handling Club Refunds**

This guide is for TUSA staff. **Clubs process their own refunds** from their Store Manager dashboard — you don’t click refund for them. What reaches the Clubs team is the **edge cases and money questions** the club-facing guide tells clubs to send to `clubs@tusa.utas.edu.au`.

The club-side guide is [Refunding Customers](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/club-administration/club-guide/refunds.md); this is the staff side of it.

---



## **How club refunds work (the staff view)**

- Each club store is a **Stripe-connected account.** When a customer pays, the money lands in the club’s Stripe balance and **pays out to the club’s bank account within the day.**
- When a club refunds an order, the money goes back to the customer **from their current Stripe balance** — so a refund a few days later can push the balance **negative** (the original sale has usually already paid out).
- **Clubs can’t see their Stripe balance; TUSA can.** Anything that depends on knowing the balance comes to you.

The club does the refund itself. Your role is to **advise on policy**, **point clubs to the parts they handle themselves** (like clearing leftover tags), and **route anything to do with money to finance**.

---



## **What the Clubs team handles**

### **Refund policy questions**

Clubs email when they’re unsure *whether* to refund — event already happened, membership mid-year, something outside their stated policy. There’s no system action here: give guidance based on what the club told its members and TUSA’s general position. The club still processes the refund themselves.

### **Leftover access tags after a refund — clubs do this themselves**

When a club refunds a **membership** or **event ticket**, the money goes back correctly, but the **tags don’t change on their own.** Updating them is part of how clubs manage their members — it’s the **club’s** job, not the Clubs team’s. Club presidents and admins manage their own members’ tags from their dashboard.

If a club asks you to remove a leftover tag for them, point them back to their own member management (the club guide, [Refunding Customers](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/club-administration/club-guide/refunds.md) → “What happens to memberships, tickets, and tags”). Removing tags is just part of running their club — it stays with them.

### **Guiding a club whose refund won’t go through**

If a club says the **Request Refund** button won’t appear or submit, it’s usually one of: the order’s already fully refunded, an earlier refund request is still pending, or the order’s payment status is off. Walk them through checking the order status. If it genuinely won’t process (for example the order is past Stripe’s refund window), that’s a **money matter** → finance (below).

---



## **What goes to Finance**

**Anything that touches money, balances, or Stripe goes to the TUSA finance team — not the Clubs team, and not the back end.** Clubs work with finance to iron out their club finances. Hand these over rather than attempting them:


| The club is asking about… | Why it’s finance |
| ------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------ |
| **“What’s our Stripe balance?”** | Only finance works in Stripe; balances aren’t visible from the site |
| **A large or bulk refund** (e.g. a whole cancelled event) | Needs a balance check first — finance confirms the balance can cover it |
| **A negative balance / top-up** | Clearing a negative balance (a top-up, or waiting for sales to clear it) is a finance action in Stripe |
| **A dispute or chargeback** | Responding to disputes happens in Stripe, on a deadline — finance handles it |
| **A double charge / a payment that looks wrong** | Has to be checked against Stripe directly |
| **A refund that won’t process because the order is too old** | Past Stripe’s window — finance works out how to settle |


Pass the club’s details and the order info to finance and let them work it through with the club.

---



## **Hire refunds**

Hire Store orders aren’t club-store orders — they’re handled through the hire process, not by clubs. See [Handling Club Hire Orders](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/club-administration/handling-club-refunds/#handling-hire-orders).

---



## **Quick reference**


| Club contacts you about… | You… |
| -------------------------------------------------------- | ---------------------------------------------------------------------------- |
| Whether they *should* refund | Advise on policy; they process it themselves |
| A leftover access tag after a refund | It’s theirs to clear — point them to their own member management |
| Refund button won’t work | Help them check order status; escalate to finance if it’s a Stripe/age issue |
| Balance, big/bulk refund, top-up, dispute, double charge | **Route to finance** |
| A hire refund | Point to the hire process |


