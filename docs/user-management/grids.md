---
title: Managing Users in Grids
hide:
  - toc
---
# **Managing Users in Grids**

The public pages that show people — Elected Representatives, Board of Management, Equity Committee, TUSA Team, Student Advocates — are called grids. This guide is how you add someone to one, take them off, and set the order they show in.

You do this by editing the person’s user account. Members can’t put themselves on these pages, and can’t set their own role title, public bio or photo for them — that’s your job. So when someone takes up a role, **you get their details from them** (their role title, a short bio, and a photo) and set them up.

There are four things that make someone show up correctly:

- **Turn their visibility on** — the switch that makes them appear on the page.
- **Set their role title** — the label on their card (e.g. “President”).
- **Give them an order number** — where they sit on the page (lower number = nearer the top).
- **Add a bio and photo** — so their card looks complete.

It’s done by hand on purpose, so nobody appears on a public page before their details are ready.

---



## **Quick reference: all grids**




| Grid | Page | Turn on with | Role title field (card label) | Order number field |
| ---------------------------------- | ----------------- | ----------------------------- | ----------------------------- | ------------------------------------- |
| **Student Representatives** | Elected Reps page | “Is an Elected Rep” | “Elected Rep Role” | **Elected Reps Grid Order** |
| **Student Representatives (home)** | Homepage block | “Is an Elected Rep” | “Elected Rep Role” | **Elected Reps Home Page Grid Order** |
| **Board of Management** | Board page | “Is a Board Member” | “Board Role Title” | **BoM Grid Order** |
| **Equity Committee** | Equity page | “Is Equity Committee Member” | “Equity Committee Role Title” | **Equity Committee Grid Order** |
| **Sustain & Support** | Support grid | (Sustain & Support opt-in) | — | **Sustain and Support Grid Order** |
| **TUSA Team** | Staff page | Profile type set to TUSA Team | — | **TUSA Staff Grid Order** |
| **Student Advocates** | Advocates page | “Are you a Student Advocate?” | — | *(alphabetical — no order number)* |
| **TELs (Experience Leaders)** | TEL page | “Is a TEL” | “TEL Role Title” | *(a typed list — see note)* |


> **Reps show in two places:** the Elected Reps page **and** the homepage block, and each has its **own** order number. So you can put the President top of both, or order them differently in each. Set both if the person appears in both.

> > **TELs:** the Experience Leaders page is a hand-typed list, not one of these grids. If you’d like it to work like the others, ask the dev team.

---



## **Adding someone to a grid**



- Go to **Users**, search for the person, and open their account to edit.
- **Turn their visibility on.** Find the field for that grid (see the table above — e.g. “Is a Board Member”) and set it to **Yes**.
- **Set their role title** (the card label). For example “President”, “Chair”, “External Board Member”. This is only the label — it doesn’t affect the order.
- **Give them an order number** (see the table for the field name — e.g. “BoM Grid Order”). Lower number shows nearer the top. See [Setting the order](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/user-management/managing-users-in-grids/#setting-the-order) below.
- **Check they have a photo and a bio** in the bio field for that grid (“Rep Bio”, “Board Bio”, “Committee Bio”).
- **Save.**

They should now appear on the page. If not, see [If someone doesn’t show up right](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/user-management/managing-users-in-grids/#if-someone-doesnt-show-up-right).

> **Two spots on the same page:** the visibility switches and role titles are down in the profile section, but the order number sits near the top of the person’s account screen. Two different places on the same edit page.

---



## **Removing someone from a grid**



When someone leaves a role:

- Go to **Users**, find the person, and open their account to edit.
- Find the grid’s visibility field (e.g. “Is a Board Member”) and set it to **No**.
- **Save.**

They come off the page straight away. You don’t need to clear their title or bio — turning visibility off is enough.

---



## **Setting the order**



The order number decides where someone sits. One rule for every grid:

- **Lowest number shows first** (nearest the top).
- **No number = the bottom**, in alphabetical order. You only need to number the people whose position matters.
- **Count in tens** (10, 20, 30…) so you can slot someone in later without renumbering everyone.



### **Example — Student Representatives**



To get this order on the page, set each person’s **Elected Reps Grid Order** to the number shown:


| Order number | Person | Role (card label) |
| ------------ | ------- | --------------------------------- |
| 10 | Jack | President |
| 20 | Molly | General Secretary |
| 30 | Kashif | Equity President |
| 40 | Solomon | Undergraduate Education President |
| 50 | Jeppe | Postgraduate Education President |
| 60 | Oliver | Southern Campus President |
| 70 | Liv | Northern Campus President |
| 80 | Kayla | Cradle Coast Campus President |
| 90 | Henry | Rozelle Campus President |


**Slotting someone in later:** a new Campus President needs to sit between Oliver (60) and Liv (70)? Give them **65**. Nobody else changes — that’s why you count in tens.

**Moving someone up or down:** just change their number. To move Kashif above Molly (who’s 20), give Kashif something lower, like 15.

**Same person on two grids:** the reps appear on the Elected Reps page and the homepage, each with its own order number. Set both — same numbers, or different if you want a different order in each.

---



## **When roles change over**



&nbsp;

### **Elected Representatives (after an election)**



- **Take the outgoing reps off:** set “Is an Elected Rep” to **No** for each.
- **Add the incoming reps:** for each new rep, set “Is an Elected Rep” to **Yes**, set their “Elected Rep Role” (the card label), give them an “Elected Reps Grid Order” number (and “Elected Reps Home Page Grid Order” if they’re on the homepage too), and check they have a bio and photo.
- **Save each one.**

Common titles: President, General Secretary, Equity President, Education President (Undergraduate), Education President (Postgraduate), and the campus presidents (Sandy Bay, Inveresk, Cradle Coast, Sydney).



### **Board of Management (when the board changes)**



- **New members:** set “Is a Board Member” to **Yes**, set “Board Role Title”, give them a “BoM Grid Order” number, add their bio and photo.
- **Departing members:** set “Is a Board Member” to **No**.

Common titles: Chair, UTAS Board, External Board Member, Ex-President, Student Board.



### **TUSA Team**



Team members show on the staff page because their **profile type is TUSA Team** (there’s no on/off switch like the other grids).

- **To add someone:** their profile type needs to be TUSA Team (set when they’re onboarded — see [Managing User Registrations](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/user-management/managing-users-in-grids/managing-users.md#onboarding-a-new-tusa-team-member)). Then set their team (“Student Experience”, “Advocacy”) and their job title, and add a bio and photo.
- **To take someone off:** change their profile type, or ask the dev team if their type shouldn’t change.

---



## **If someone doesn’t show up right**



**They’re not appearing at all:**

- Check the visibility field is set to **Yes** (exactly “Yes” from the dropdown).
- Check they have a photo — some pages hide people without one.
- Refresh the page (Ctrl+Shift+R on Windows, Cmd+Shift+R on Mac). If it still doesn’t show, ask the dev team.

**They’re in the wrong order:**

- Check you gave them an order number — no number sends them to the bottom.
- Lower number shows higher up. If they’re too low, give them a smaller number than the person above them.
- For reps, check you set the right one — the page and the homepage have separate order numbers.
- Save, then refresh the page.

**Two people sitting together:** they’ve got the same number. Give them different numbers to force one above the other.

**The page looks out of date:** refresh with Ctrl+Shift+R (or Cmd+Shift+R). Give it a minute if it’s still stale.

**You can’t see the fields when editing someone:** your access might not cover them — ask an administrator.

---



## **Tips**



- Changes go live straight away, so make big changes at a quiet time.
- When you’re swapping people over, take the old person off first, then add the new one.
- After changes, look at the actual page to check it’s right.
- Before an election changeover, screenshot the current page so you have a record.

---



## **Related**



- [Managing User Registrations](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/user-management/managing-users-in-grids/#managing-users) — setting up members and TUSA staff
- [Page Builder Guide](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/user-management/managing-users-in-grids/#page-builder-guide) — editing pages

