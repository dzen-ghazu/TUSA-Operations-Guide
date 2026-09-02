---
title: Managing Users Registrations
hide:
  - toc
---
# **Managing User Registrations**

This guide covers new user registrations and profile updates, and how you set up TUSA team members and store staff. Registrations and profile updates apply automatically — there’s no approval queue. What needs a person is **granting elevated roles** (staff / Board / Rep / committee), which you do in wp-admin.

---



## **Overview**



The website allows users to:

- **Register** for a new account (sets their base membership — student / past student / customer, plus junior if under 18)
- **Update their profile** to change their own details (name, contact, relationship to UTAS, etc.)

Registration and profile updates run automatically — neither lets a user claim an elevated role. Elevated roles (TUSA staff, Board, Rep, committee, UTAS staff) and club roles are set by staff through the real channel (HR onboarding, election, EOI, board appointment, affiliation), covered below.

---



## **New User Registrations**



&nbsp;

### **What Happens When Someone Registers**



- User fills out the registration form
- Account is created automatically with their base membership
- User is logged in immediately
- That’s it — there’s no approval step. The join form only sets base membership (student / past student / customer, plus junior by age), so nothing needs verifying or approving.



### **Where Users Can Register**




| Location | How It Works |
| --------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| **Registration page** | The standard registration form |
| **Checkout** | Prompted when a guest tries to purchase – the same registration shown in the “New Here?” tab, cart preserved |
| **Profile icon** | A logged-out visitor who clicks the profile icon is shown a login / join form, so they can sign in or register from there |


**Checkout Registration Flow:**

- Guest adds items to cart and proceeds to checkout
- Sees tabbed interface: “New Here?” (register) or “Already a Member?” (login)
- After registration/login, page reloads and checkout form appears
- Cart is preserved throughout – no lost items



### **What to Review**



Registrations are fully automatic — the join form only sets base membership, so there is nothing to approve. Everyone who registers gets a standard member account (student / past student / customer, plus junior if under 18).

Nobody can register *as* TUSA staff, a board member, or a rep — the form doesn’t ask, and there’s no elevated-claim approval queue. Elevated access is granted afterwards by staff, through the real channel:


| To grant… | Do this | Prompted by |
| ------------------------------------------------- | ------------------------------------------------------------------------- | -------------------------------------------------------------- |
| TUSA staff / Board / Rep / committee / UTAS staff | Set the profile type + tags in wp-admin (Users → Edit → Extended Profile) | HR onboarding, election result, EOI outcome, board appointment |
| Club president / committee | Handled by affiliation / reaffiliation | Club affiliation |
| Food Hub volunteer | A location admin adds them to the Food Hub group | Volunteer signing up at a location |


See [Onboarding a New TUSA Team Member](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/user-management/managing-user-registrations/#onboarding-a-new-tusa-team-member) below and [Checking Profile Update Claims](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/user-management/managing-user-registrations/checking-profile-claims.md) for verification detail.

---



## **Onboarding a New TUSA Team Member**



A new TUSA team member is set up **entirely by a content admin** — there is no form to approve and no automatic process that grants staff access. The person registers a normal account (base membership) like anyone else, and you then elevate them by hand, prompted by HR onboarding. This is intentional: every team member should be individually verified before being given elevated access.



### **The roles a staff member needs — the whole picture**



A TUSA staff member’s access is built from **layers**, and which layers they get depends on their job. Nobody gets “all of it” by default — you add the pieces their role actually needs. Here’s what each layer is and what it unlocks:


| Layer | Role(s) | What it gives them | Give it to staff who… |
| -------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Profile type** | `TUSA Team` (profile type, set in Extended Profile) | Marks them as staff; puts them on the TUSA Team grid if grid-visible | Every TUSA staff member |
| **Backend access** | `Content Admin` **or** `Clubs Super Admin` | Gets them into wp-admin. Content Admin = content (courses, posts, media, EOIs). Clubs Super = users, clubs, stores, orders | Only staff who need the admin area — not everyone does |
| **Triage roles** | `TUSA Clubs Admin`, `TUSA Grants Admin`, `TUSA SASH`, `TUSA Advocates`, `TUSA Internal Admin`, `TUSA Events`, plus the email-routing ones (`TUSA UTE`, `TUSA Social Media`, `TUSA Elections Admin`, `TUSA Admin Role`, `Food Hub Admin`) | Decides what work arrives for them — either in their **Workflow Inbox** or emailed to them as an EOI/feedback team. Carries no admin access on its own | Staff who process that kind of submission. Assign the ones that match their job; they can have several. Full breakdown of what each one receives is in [Step 3](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/user-management/managing-user-registrations/#step-3-assign-triage-roles) |
| **Store staff** | `Vendor Staff` **+** `TUSA Shop Staff` and/or `Hire Store Staff` | Access to run a store — orders, products, customer details | Staff who work the Merch Store or Hire Store |
| **Group membership** | Added to **TUSA Internal** group | The internal group for staff — comms and shared files | Every TUSA staff member |
| **Grid visibility** | Grid fields in Extended Profile | Makes them appear on a public page (Team, Reps, Board…) with a title, bio and photo | Only if they should be shown publicly — see [Managing Users in Grids](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/user-management/managing-user-registrations/#managing-user-grids) |


**How to think about it:** start with the profile type + TUSA Internal group (everyone gets those), then add backend access **only if they need wp-admin**, add the **triage role(s) that match what they’ll process**, add **store staff** if they work a store, and set **grid visibility** only if they go on a public page. The rest of this section walks each of those.

> **Role order matters** whenever you give someone a backend access role — it MUST be their **first** role, or they get stuck in a redirect loop. See [role order](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/user-management/managing-user-registrations/#step-2-set-up-their-backend-access-if-needed) below.



### **Step 1: Verify them, then set their profile type**



- Confirm the person is a legitimate new TUSA staff member — check the staff list / HR onboarding. If you’re unsure, check with HR or management **before** elevating them.
- Make sure they have a normal account (they register one themselves if they don’t).
- Go to **Users → Edit → Extended Profile** and set their profile type to **TUSA Team**, and fill in their role title / bio.
- Add the matching **TUSA Team** tag in FluentCRM.

This is a back-office change — there’s no email to the user and nothing for them to approve. Setting an elevated role in wp-admin is covered step-by-step in [Managing Users in Grids](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/user-management/managing-user-registrations/#managing-user-grids). For the full verification-by-role detail, see [Checking Profile Update Claims](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/user-management/managing-user-registrations/#checking-profile-claims).



### **Step 2: Set Up Their Backend Access (if needed)**



Not all team members need backend (admin area) access. But if they do:

**If they need to manage content (courses, posts, media):**

- Give them the **Content Admin** role

**If they need to manage users, clubs, stores, or orders:**

- Give them the **Clubs Super Admin** role

**IMPORTANT – Role order matters!** If you’re giving someone a backend access role, it MUST be their first role. Otherwise they’ll get stuck in a redirect loop and can’t access the admin area.

**How to set role order correctly:**

- Go to **Users** → find the team member → **Edit**
- Remove all their current roles
- Add the backend access role **first** (Content Admin or Clubs Super Admin)
- Then add their other roles back (editor, customer, etc.)



### **Step 3: Assign Triage Roles**



Triage roles decide **what work arrives for that person**. They are the difference between a submission  
sitting unclaimed and it turning up in someone’s queue. Assign the ones that match what the person is  
actually responsible for processing.

**These roles are safe to hand out.** Every triage role carries exactly one capability, `read`. On its  
own a triage role gives no admin access, no ability to edit anything, and no visibility of the site’s  
back end. It is a routing label. What it does is put matching submissions in front of that person.

There are two kinds, and they behave differently.



#### **Kind 1: Workflow Inbox roles**



The person holding the role sees the item in their **Workflow Inbox** on the site and actions it there.


| Role | Give it to staff who… | What actually lands in their inbox |
| ----------------------- | -------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **TUSA Clubs Admin** | Run club affiliations and club approvals | New Club Applications and Affiliations, Club Reaffiliations, Requests to Change Bank Signatories, the club-side approval on event / risk / stall / liquor / grant applications, and club-related incident reports |
| **TUSA Grants Admin** | Assess and approve grants | Grant Applications, both allocating them and approving them, plus Grant Claims |
| **TUSA SASH** | Are authorised to handle sexual assault and harassment matters | Sexual assault and harassment incident reports, and nothing else. These reports go **only** to this role |
| **TUSA Advocates** | Handle student advocacy cases | The “everything else” incident route, jointly with Internal Admin. This is the route most reports take |
| **TUSA Internal Admin** | Handle TUSA’s own entity matters | TUSA Entity approvals on event / risk / stall / liquor applications, and the “everything else” incident route alongside Advocates |
| **TUSA Events** | Run TUSA events | Event-related incident reports, External Provider Temporary Stall Applications, and both the risk assessment and event application approvals for TUSA’s own events |


**Give someone several if their job spans several.** Somebody who runs both clubs and grants gets both  
roles, and both queues arrive in the one inbox. That is why no two staff members have the same  
combination, and that is correct rather than untidy.

**A joint route needs one person from each role.** The “everything else” incident route is assigned to  
Advocates *and* Internal Admin together, so it needs an action from someone in each of those two  
roles before it moves on. If one of those roles has nobody in it, that queue stops.

**Where a role has several people in it, only one of them needs to act.** Gravity Flow treats a role as  
a single assignee, so the first person in that role to pick the item up completes it for everyone. This  
is exactly why routing to a role beats naming an individual: nobody’s leave stops the queue.



#### **Kind 2: Email routing roles**



These are not inbox roles. They are the **team options you pick when assigning an EOI or a piece of**  
**feedback**. The system looks up who holds the role and emails them a link. They action it from the  
email and do not need to log in.


| Role | Give it to staff who… |
| ------------------------ | ------------------------------------------------------------------- |
| **TUSA UTE** | Run Unique Tassie Experience trips |
| **TUSA Social Media** | Manage TUSA’s social accounts and handle social media complaints |
| **TUSA Elections Admin** | Run student elections. Election EOIs default to this team |
| **TUSA Admin Role** | Should receive the “General” catch-all when an EOI fits nobody else |
| **Food Hub Admin** | Run the Food Hub |


The inbox roles above can also be picked as an EOI or feedback team, so a role can do both jobs. What  
decides who gets the email is simply **who holds the role at the time**.



#### **Before you assign, two things that catch people out**



**A role on its own is not always access.** Store roles are the exception to the “roles are safe”  
rule above: `TUSA Shop Staff` and `Hire Store Staff` do nothing unless the person **also** has  
`Vendor Staff`. Someone with a store role and no Vendor Staff looks correctly set up on their user  
profile and cannot actually work the store. Check both are present.

**Some triage roles can see more than their own queue.** Staff holding **TUSA SASH**, **TUSA Grants**,  
**TUSA Clubs Admin** or **TUSA Admin Role** are additionally granted access to the workflow status and  
activity pages, which list **all** workflow entries, including ones never assigned to them. In  
practice that means a member of the Clubs team can open a SASH entry directly, even though SASH  
reports are never routed to them. If that matters for a particular person, it is a permissions  
question and not something assigning or withholding a triage role will solve. Raise it rather than  
working around it.

**How to assign:**

- Go to **Users** → find the team member → **Edit**
- Add the relevant triage role(s)
- If you added a store role, confirm **Vendor Staff** is there too

Roles are always assigned by hand. Nothing on the site grants a triage role automatically, and that is  
deliberate: these roles decide who sees sensitive material, so a person puts eyes on every one.



### **Step 4: Add to TUSA Internal Group**



Team members need access to the TUSA Internal community group for internal communications and shared files.

- Go to **Groups** → **TUSA Internal** in the community area
- Add the user as a member



### **Step 5: Enable Grid Visibility (if appropriate)**



If the team member should appear on the public Team Directory page:

- Go to **Users** → find the team member → **Edit**
- Make sure their profile is complete (photo, bio, role title)
- Tick the **“Show in Team Grid”** checkbox
- They’ll now appear on the public team page



### **Quick Checklist**



Use this to make sure you haven’t missed anything:



```
[ ] Identity verified against the staff list / HR onboarding
[ ] Profile type set to TUSA Team (Users → Edit → Extended Profile) + TUSA Team tag in FluentCRM
[ ] Backend access role set as FIRST role (if needed)
[ ] Triage roles assigned based on their job
[ ] Added to TUSA Internal group
[ ] Grid visibility enabled (if they should be on the team page)
[ ] Tested: they can log in and see their workflow inbox

```



---



## **Adding TUSA Store or Hire Store Staff**



When someone needs to manage products and orders in the TUSA Merch Store or the Hire Store, they need two roles:

- **Vendor Staff** – This is the required role for any store access
- **A store-specific role** – This is our role that links them to the correct store



### **Which Store Role?**




| Store | Role to assign | What it does |
| ------------------------------ | ------------------------------------------- | --------------------- |
| TUSA Merch Store | **TUSA Shop Staff** (`tusashopadd`) | Links to Vendor ID 14 |
| Hire Store (equipment rentals) | **Hire Store Staff** (`tusahirestorestaff`) | Links to Vendor ID 76 |


### **How to Add Store Staff**



- Go to **Users** → find the person → **Edit**
- Add the **Vendor Staff** role
- Add the store-specific role: **TUSA Shop Staff** and/or **Hire Store Staff**
- Save

**If they also have a backend access role** (Content Admin or Clubs Super Admin), make sure that role is still their **first role**. See the role-order section above.



### **Both Stores**



If someone needs access to both the Merch Store and the Hire Store (common for TUSA team members), give them all three roles:

- Vendor Staff
- TUSA Shop Staff
- Hire Store Staff

They’ll get a **Store Switcher** in their dashboard that lets them switch between the two stores.



### **Alternative: Add via the Store Dashboard**



Store owners and existing store staff can also add people directly from their store:

- Go to **Store Dashboard** → **Team**
- Search for the existing user and add them
- This automatically gives them Vendor Staff + links them to that store

This is useful for quickly adding temporary helpers (e.g., event stall workers).



### **What Store Staff Can Do**



Once set up, store staff can:

- View and manage orders
- Add and edit products
- See customer details (names, emails, purchases)

**Important:** Only add people you trust – store staff see all customer information.



### **Removing Store Staff**



To remove someone’s store access:

- Go to **Users** → find the person → **Edit**
- Remove the **Vendor Staff** role and the store-specific role(s)

Or from the store dashboard:

- **Store Dashboard** → **Team** → **Remove from Store**
- This removes their store link but keeps their account

---



## **Profile Updates**



Users can update their profile at any time via `/update-my-profile/`

The profile update form handles **base membership only**. It lets a regular member edit their own name, nickname, relationship to UTAS, DOB, pronouns, student number, campuses, undergrad/postgrad, year of study, preferred contact email, and personal bio. It does **not** let anyone claim an elevated role — those questions and role/bio fields are no longer on the form.

Because of that, profile updates run through automatically:

- Name / nickname changes
- Relationship to UTAS (Current / Past / Never a student) — profile type + membership tags reconcile
- Contact details, campus, year of study, pronouns, personal bio

**Elevated roles are set by you, not claimed on the form.** When someone is elected, appointed, hired, or their club affiliates, a content admin sets their profile type + role fields in wp-admin (Users → Edit → Extended Profile) — see [Onboarding a New TUSA Team Member](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/user-management/managing-user-registrations/#onboarding-a-new-tusa-team-member) above and [Checking Profile Update Claims](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/user-management/managing-user-registrations/checking-profile-claims.md).

**System email + password** are changed by the member on their **Account** settings, not on the profile update form. If someone asks to change their login email, point them there.

**Blocked for club presidents/admins.** They don’t see the profile update form at all — they get a message telling them to go through affiliation/reaffiliation (contact `clubs@tusa`). Their profile is tied to a specific role and store.

---



## **User Types and What They Mean**



A member’s base profile type comes from their answer to “your relationship to UTAS” (three options) plus their age. Elevated types (UTAS Staff, TUSA Team, Board, Rep, Club roles) are set by staff, not the form.


| Profile Type | Who This Is | Set by |
| ----------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------- |
| **Student** | Current student (18+) | Registration |
| **Junior Member** | Any member under 18 (student, past student, or customer — junior is an age flag on top of their real membership) | Registration |
| **Associate** | Past student | Registration |
| **Customer** | Never been a student — uses the shop/site without a membership relationship (renamed from “Hire Store Customer”; anyone can hire gear regardless) | Registration |
| **UTAS Staff** | University employee | Staff (admin) |
| **TUSA Team** | TUSA employee | Staff (admin) |
| **Board of Management** | Board director | Staff (admin) |
| **Student Rep** | Student representative | Staff (admin) |
| **Club President** | Current club president | Affiliation/reaffiliation |
| **Club Admin** | Club executive committee member | Affiliation/reaffiliation |


Profile types affect:

- What content they can see
- What groups they can join
- What features they can access

---



## **Annual Student Confirmation**



Each year from May 1st, students are prompted to confirm they’re still studying. The system runs itself — your job is to monitor the impact on club committee composition (the 50% student rule) once confirmations start coming in, and handle individual cases if a member’s status comes out wrong.

**Full guide:** [The Annual Student Confirmation](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/user-management/managing-user-registrations/annual-student-confirmation.md) — covers timing, who sees it, what happens when members say yes or no, what staff need to monitor, manual resetting for testing, and common situations.



### **Three sources of student status**



These all feed into a member’s current status — don’t conflate them:


| Source | When | What it does |
| ----------------------- | ------------------- | ----------------------------------------------------- |
| **Registration** | Account creation | Sets initial student/non-student status |
| **Annual confirmation** | From May each year | Confirms or transitions student → associate |
| **Reaffiliation** | Annual club renewal | Captures committee composition, manages role accounts |


---



## **Junior Members (Under 18)**



&nbsp;

### **What Is a Junior Member?**



A junior member is any user under 18 years old (based on their under-18 answer / birth date at registration) — **regardless of student status**. A junior can be a student, a past student, or a customer; “junior” is an age flag layered on top of their real membership.

The system automatically assigns the `junior-member` profile type, and applies the `Junior` tag on top of their membership tag (Student / Associate / Customer).



### **Why Junior Tracking Matters**




| Concern | Implication |
| ------------------------ | ---------------------------------------------------------- |
| **Parental consent** | Clubs need signed consent forms before juniors participate |
| **Insurance** | Different liability considerations for minors |
| **Adventure activities** | Higher risk activities require explicit parental approval |
| **Alcohol restrictions** | Juniors cannot attend events with alcohol |


### **How Juniors Are Identified**



When someone registers, they’re asked whether they’re under 18. If they are, they’re marked as a **Junior Member** on top of whatever their membership is (student, past student, or customer) — it’s an age flag, not a membership in its own right. Nobody has to set this by hand; it happens from their answer at registration.

**Automatic restrictions:**

- Juniors can’t buy tickets to events serving alcohol
- Some content may be hidden from juniors



### **Viewing Junior Members**



**All Clubs Export (TUSA Admin):**

- Go to the All Clubs member export page
- Overall summary shows total juniors across all clubs
- Each club card shows junior count and names
- CSV includes “Is a Junior” column

**Individual Club:**

- Club admins see their juniors in their Ready Reckoner
- Club’s Resources tab has parental consent forms



### **Parental Consent Compliance**



**What clubs must do:**

- Collect signed parental consent form before junior participates
- Store forms in their Resources → Parental Consent (GravityView)
- Cross-reference junior members with received consent forms before events
- Turn away juniors without consent on file

**What TUSA should check:**

- When reviewing event applications for clubs with junior members, note that parental consent is the club’s responsibility
- For high-risk activities (adventure clubs), consider asking if junior consent procedures are in place
- Alcohol events: Confirm club understands juniors cannot attend



### **When Juniors Turn 18**



This happens automatically: on the member’s 18th birthday they’re moved from Junior Member back to the adult membership their status implies (Student, Associate, or Customer), keeping their membership. No manual step is needed. A member can also trigger the same change early by updating their profile.

---



## **Managing Tags in the Back End (FluentCRM)**



Tags are the labels that drive memberships and access across the site. A member’s tags decide which club groups they belong to, what member-only content and deals they see, and which products they can buy. Tags live in **FluentCRM**, in the site’s back end (**wp-admin → FluentCRM**). Both Content Admins and Clubs Super Admins can open FluentCRM and adjust tags.

Almost everything happens automatically — tags are applied when someone registers, buys a membership or ticket, or is approved for a role, and they’re removed on refund or expiry. You only reach into FluentCRM by hand for the occasional exception below.



### **Adjusting a Member’s Tags Manually**



Sometimes a member needs a tag added or removed directly — for example, a membership sold offline that never went through the store, or a tag that needs correcting.

- Go to **wp-admin → FluentCRM → Contacts**.
- Find the contact **by email** (FluentCRM matches members by their email address — search by email, not name, to be sure you have the right person).
- Open the contact and go to their **Tags**.
- **Add** the tag you want (start typing to pick an existing tag) or **remove** one, then save.

The change takes effect the same way an automatic tag does: if you add a club’s membership tag, the member is granted that club’s group; if you remove it, that access is withdrawn.

> **Add by email, and add the tag that already exists.** Don’t create a new tag here just to spell a member’s membership — pick the club’s real tag from the list. Creating a slightly different tag (a typo, a different year) gives the member a label that grants nothing, because it doesn’t match any club’s rules.



### **Creating a New Tag**



**You almost never need to do this.** When a club affiliates or reaffiliates, the system automatically creates that club’s membership tags for **three years** — the current year and the next two. So a club is always already set up with, for example, `Chess Club 2026`, `Chess Club 2027`, and `Chess Club 2028`, and those appear ready to choose in the club’s Membership Rules form. Clubs don’t need anyone to create their normal year tags.

The one time you create a tag by hand is when a club wants to go **further into the future than that three-year window** — for instance, it’s 2026 and a club wants to sell a **2029** membership now. That year hasn’t been created yet, so an admin adds it.

**Follow the exact pattern, or the club won’t find it.** A club’s Membership Rules form only lists tags that match that club, and it matches on the tag’s name. The name must be:

> **Club Name** + one space + **Year**

exactly as the club’s other tags are named — the full club name spelled the same way, then a space, then the four-digit year. For example:


| Club | Year needed | Tag to create |
| ------------------------------------- | ----------- | -------------------------------------------- |
| Chess Club | 2029 | `Chess Club 2029` |
| Tasmanian University Bushwalking Club | 2029 | `Tasmanian University Bushwalking Club 2029` |


Match the existing tags precisely. `Chess-Club 2029`, `Chess Club '29`, or `chess club 2029` all create a tag that the club’s form won’t recognise, so it won’t appear for them to use.

**To create it:**

- Go to **wp-admin → FluentCRM → Tags**.
- Click to add a new tag.
- Name it using the pattern above — copy the club’s existing tag name and change only the year.
- Save. It’s now available for that club to select in their Membership Rules form and to apply to a membership product.



### **The** `{Club} Admin` **Tag — Leave It Alone**



Every club also has a special tag named `Club Name Admin` (for example, `Chess Club Admin`). This one marks a club’s committee as members because they run the club, and the system manages it entirely — it’s created automatically and applied to committee members when they’re set up. It’s deliberately hidden from the club’s own Membership Rules form.

**Don’t create, rename, or hand-edit** `Club Name Admin` **tags.** If a committee member seems to be missing their access, it’s almost never this tag — it’s usually their group role. See [Approving Club Applications](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/user-management/managing-user-registrations/#approving-clubs) for how committee membership is set up, or [Reporting an Issue](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/user-management/managing-user-registrations/#reporting-issues) if something looks wrong.

---



## **Food Hub Volunteers**



Food Hub volunteers are **not** onboarded through the profile forms and there’s no “Food Hub Volunteer” claim to approve. A Food Hub admin adds the person **to the Food Hub group**, and that provisions everything.



### **How someone becomes a Food Hub volunteer**



- They register a normal account first (base membership, like any member).
- A Food Hub admin adds them to the **Food Hub group**.
- That automatically sets up their shift-system record and gives them Food Hub access.
- The Food Hub admin then puts them on the right calendar(s) by hand.

Full detail is in [Setting Up Food Hub People](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/user-management/managing-user-registrations/#setting-up-food-hub-people) and [Food Hub Rosters](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/user-management/managing-user-registrations/#managing-food-hub-rosters).



### **What a Food Hub volunteer gets**



Once they’re in the Food Hub group:

- Access to the volunteer shift calendar (once they’re on a calendar)
- Access to volunteer-only content

---



## **Common Tasks**



&nbsp;

### **Finding a Specific User**



- Go to **Users** in the admin area
- Search by name or email



### **Checking Someone’s Current Status**



- Find their user account (Admin area → Users)
- Check their profile type
- Check their group memberships



### **Changing Someone’s Role/Type**



**Elevated role or profile type (Board, Rep, TUSA Team, UTAS Staff, etc.) — you set it:**

- Find their user account (Users → Edit)
- In **Extended Profile**, set their profile type and any role title / bio / grid-visibility fields
- Add or remove the matching tag in FluentCRM if needed

Don’t send them to the profile update form for this — that form only handles base membership (Student / Associate / Customer + Junior) and deliberately **leaves an elevated profile type unchanged**. If an elevated member’s type “won’t change” after a profile update, that’s by design; change it here in wp-admin.

**Their name, contact details, or base membership** — they can self-update from their own profile, and it applies straight away. **Login email + password** are on their **Account** settings.



### **Removing Access**



If someone should no longer have a particular access level:

- Find their user account
- Remove the relevant role or group membership
- Their profile type may need updating

---



## **Common Issues**



&nbsp;

### **“User says they registered but can’t log in”**



**Check:**

- Did registration complete? (Look in Users)
- Did they verify their email?
- Are they using the right email address?
- Try sending a password reset



### **“User should have access but doesn’t”**



**Check:**

- What’s their profile type? (May be wrong)
- Are they in the right groups?
- Do they have the right role?



### **“Someone has access they shouldn’t have”**



- Check how they got it (legitimate registration? error?)
- Remove inappropriate access
- If suspicious, report to your manager



### **“Food Hub volunteer can’t see the schedule”**



**Check:**

- Are they in the **Food Hub group**? (That’s what provisions their access — adding them to the group is the whole onboarding.)
- Have they been put on a **shift calendar**? (Being in the group makes them available; a Food Hub admin still assigns the calendar by hand.)
- Is the Food Hub admin themselves set up correctly? See [Setting Up Food Hub People](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/user-management/managing-user-registrations/#setting-up-food-hub-people).

---



## **Quick Reference: Where Things Live**




| Need to Find | Where to Go |
| ------------------- | --------------------------------------------------- |
| Individual user | Admin area → Users → Search |
| Food Hub volunteers | Food Hub group members (they’re added to the group) |


---



## **Related Guides**



- [Checking Profile Update Claims](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/user-management/managing-user-registrations/#checking-profile-claims) – What (doesn’t) need approving, and setting elevated roles
- [Managing User Grids](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/user-management/managing-user-registrations/#managing-user-grids) – Student rep and team display pages
- [Setting Up Food Hub People](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/user-management/managing-user-registrations/#setting-up-food-hub-people) – Making a new Food Hub admin, and adding volunteers
- [Food Hub Rosters](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/user-management/managing-user-registrations/#managing-food-hub-rosters) – Day-to-day shift running

