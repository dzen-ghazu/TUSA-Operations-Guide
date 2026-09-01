---
title: Stripe Connected Accounts
hide:
  - toc
---
# **Stripe Connected Accounts**

## **Why We Use Stripe**

TUSA clubs sell memberships, event tickets, merchandise, and hire equipment through their stores. Stripe processes these payments and makes sure the money goes to the right club’s bank account.

Each club gets their own **Stripe Connected Account** that sits under TUSA’s platform account. This means:

- Clubs get paid directly into their own bank account
- TUSA has oversight of all transactions for SSAF reporting
- Clubs operate under TUSA’s umbrella — they don’t need their own ABN



## **How Accounts Are Created**

Stripe Connected Accounts of the type we use (**Custom accounts**) cannot be created through the Stripe dashboard. They must be created via code — we have a custom-built tool for this.



### **Automatic (during affiliation)**

When a new club’s affiliation is approved, the system automatically creates their Stripe account as part of the setup process. You can watch this happen on the **[Club Setup Status](https://tusa-dev.its.utas.edu.au/clubs/clubs-index/tusa-internal/functions/processing/)** dashboard — look for the “Stripe Account” step.



### **Manual (if needed)**

If the automatic creation failed, or you need to create an account separately:

- Go to **TUSA Tools > Stripe Accounts** in wp-admin
- In the **Bulk Club Setup** table, find the club’s row and click **Create Account** in the **Action** column
- The account appears on the Stripe dashboard within a few minutes



### **Creating an account when there’s no store yet (e.g. Food Hub)**

Some accounts need to be set up **before** their Dokan store exists — the Food Hub  
and UTE are examples. The Bulk Club Setup table above only works for things that  
already have a store, so for these you use the simple creation form instead.

- Go to **TUSA Tools > Stripe Accounts** in wp-admin.
- Find the **Create Club Stripe Account** form (near the top of the page).
- Fill in just three things:

– **Club Name** — the name for the account, e.g. `Food Hub`  
– **Club Email** — the central address for that account, e.g. `food.hub@tusa.utas.edu.au`  
– **BuddyBoss Group** — choose the matching group (e.g. **Food Hub**) from the dropdown

- **Leave the Dokan Vendor dropdown set to “— None —”.** There’s no store to link

to yet, and that’s fine — the account attaches to the group for now.

- Click **Create Stripe Account**.

The account is created and the onboarding email goes to **[clubs@tusa.utas.edu.au**](mailto:clubs@tusa.utas.edu.au)  
(the same as for clubs). From there it’s the same as any other account — see  
[Verification](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/club-administration/stripe-connected-accounts/#verification) below for adding the bank details and finishing setup.



#### **Connecting it once the store is built (two steps, in order)**

An account created this way is attached to the **group** but not yet to the store owner, so it will **not** appear in the main “Existing Club Stripe Accounts” table until you connect it. Once the store exists, finish it with these two steps:

- **Connect the account to the store owner.** On the **TUSA Tools > Stripe Accounts** page, scroll to the **Discovered Accounts (not yet connected)** section near the bottom. The account is listed there. Choose the store’s owner from the dropdown and click **Connect**. This anchors the account to the store and makes it appear in the main table.
- **Connect the account to Dokan.** Reload the page; the account now shows in the main “Existing Club Stripe Accounts” table. On its row, click **Connect to Dokan** so the store can take payments. Check it shows “Connected” under the Dokan column.

Nothing is ever re-created — the account you make now is the one the store uses. If the store isn’t ready yet, leave it; the Discovered Accounts section keeps showing it until you connect it. If you’re unsure which owner to pick, ask Sarah.

> **If the group isn’t in the dropdown:** the account can’t be created without either a group or a store to attach it to (this prevents “floating” accounts that aren’t linked to anything). If the group you need isn’t listed, flag it before going any further rather than leaving both dropdowns on “None”.



### **Admin Page Tools**

The **TUSA Tools > Stripe Accounts** page has these actions.

**Per-account (buttons on each row of the Existing Club Stripe Accounts table)**

- **Connect to Dokan** — links the Stripe account to the club’s store. Check it shows “Connected” under the Dokan tab.
- **Regen Link** — regenerates the onboarding link if it expired.
- **Push Rep** — sends the TUSA representative details to Stripe for KYC pre-fill.
- **Push Constitution** — uploads the club’s constitution from their affiliation form to Stripe for business verification.
- **Replace ID** (orange, only on errored rows) — corrects WP’s record when the stored Stripe ID doesn’t match the real account in Stripe. Prompts for the correct ID, verifies it with Stripe before saving, then auto-reconnects to Dokan.
- **Recreate** (red, only on errored rows) — wipes the stored references to an unreachable Stripe account and creates a fresh one. Use only after confirming the original account can’t be recovered (try Replace ID first, or contact Stripe Support). The club will need to redo onboarding on the new account.

**Whole-table actions (buttons above the Existing Club Stripe Accounts table)**

- **Re-check all accounts against Stripe** — forces a live API call for every stored account. Cached statuses normally expire hourly; click this if you’ve just changed something in Stripe and want immediate confirmation.
- **Fix slashed names on Stripe** — scans every account and corrects company or business names that contain backslash-escaped quotes from an older POST-handling bug. Idempotent: clean accounts are skipped.

**Discovered Accounts (section near the bottom of the page)**

This section only appears when there’s something to fix. It lists Stripe accounts that are attached to a **group** but not yet to a **store owner** — which is the normal state for an entity account right after you create it (see “Creating an account when there’s no store yet” above). Such an account does not show in the main table and is invisible to the duplicate-account check, so it needs connecting. Pick the store’s owner from the dropdown on the account’s row and click **Connect**; the account is then anchored to that owner, appears in the main table, and is ready for the **Connect to Dokan** step. If this section is empty, there’s nothing to do.

At the bottom of the table, you’ll see a summary count like `80 stored: 75 verified · 5 errored`.



## **Verification**

After an account is created, Stripe marks it as **Restricted** until business verification is complete. The club cannot accept payments until this is resolved.



### **Constitution Upload**

The club’s constitution is the key verification document. It should be uploaded to Stripe automatically during the affiliation process. If it wasn’t (or if Stripe needs it re-uploaded):

- Try the **Push Constitution** button on the admin page first
- If that doesn’t work, upload manually via the Stripe dashboard:

– Go to **Stripe > Connected accounts** > click the club  
– For each **Action required**, select **Upload directly to us**  
– Scroll to **Upload document > Document Type: Other**  
– Tick all three boxes and upload the constitution  
– Source: SharePoint > Clubs & Societies > Constitutions > [Club name]

If the only option is **Request information** (not “Upload directly to us”), the account type is wrong — contact Sarah.



### **Name and Address Must Match**

The name and address on the Stripe account must match the constitution exactly.

**Name:** If different, go to: Stripe account > Profile > View All > Business details > Edit. Change **Name** to match the constitution. Put the common name in **Doing business as** if it differs.

**Address:** If the constitution has no address or a different one, it needs to say:

> The office address of the Club is to be at the Tasmanian University Student Association Inc. – Social Sciences Building, Level 1 Dobson Road, Sandy Bay Campus 7006.

> > The postal address of the Club for all transactions is to be at PO Box 855, Sandy Bay, 7006.



### **Other Required Information**


| Field | What to enter |
| ---------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Bank account** | Club’s BSB and account number. Source: SharePoint > C&S Archives > [Club] > Bank, or the club sends details to [clubs@tusa.utas.edu.au](mailto:clubs@tusa.utas.edu.au) |
| **Phone number** | Shauna-Lee Ward’s TUSA number: **03 6226 2862** (same for all accounts) |
| **Industry** | Membership organizations > Other membership organizations |


## **When Stripe Rejects the Constitution**

This happens regularly. Stripe’s automated review often rejects the constitution as a verification document because clubs don’t have ABNs. It takes 2-24 hours for Stripe to review, and if it’s rejected the status goes back to **Restricted**.

Contact Stripe Support at **[support@stripe.com](mailto:support@stripe.com)** with this message:

> **Subject:** Ongoing Verification for TUSA Student Club Sub-Accounts

> > Hello Stripe Support Team,

> > I’m writing on behalf of TUSA (Tasmanian University Student Association Inc.) regarding the verification of several newly created connected accounts.

> > TUSA is a registered not-for-profit student association, and we use Stripe to create connected sub-accounts for our affiliated student clubs. These clubs operate under TUSA as not-for-profit entities and do not hold their own ABNs. This model has been in place for some time, and we have already successfully connected and verified many club accounts with Stripe.

> > Previously, we reached an understanding with Stripe that a club’s constitution can be used as an acceptable business verification document in lieu of an ABN, and this approach has worked well for our existing clubs.

> > We are currently experiencing the same verification issue again and would appreciate your assistance in approving the following new accounts under this established arrangement:

> > – [Account Name] — [Account ID]

> > Thank you for your help in resolving this ongoing issue. Please let us know if there is anything further required from our side.

> > Kind regards,

To get the Account ID: Connected accounts > click the club > right side at top > **Copy ID**.

You can batch multiple clubs into one email.



## **Reaffiliation**

Stripe accounts are **not touched during reaffiliation**. The account carries over from year to year. If the president changes, update the representative on the Stripe account via Profile > View All > Edit.



## **Making Changes After Setup**

- **Edit account details:** Club’s Stripe Account > Profile > View All > Edit
- **Change bank account:** Club’s Stripe Account > scroll to External Accounts > three dots > Update



## **Troubleshooting Stripe Status**

If a row in the Existing Club Stripe Accounts table shows **Error** in the Charges column, the stored account ID can’t be retrieved from Stripe.



### **Find out what Stripe actually has**

Open Stripe Dashboard > Connect > Connected accounts and search for the club by name. You’ll see one of three things:

- **An account with a different ID than what’s stored in WP.** Usually a previous failed creation attempt left an orphan ID in WP while the real account remained in Stripe with the right name. Use **Replace ID** on the row, paste in the real ID from Stripe (always use the **Copy ID** button rather than reading the ID off the screen; the `I`, `l`, and `1` characters are visually indistinguishable in sans-serif fonts, and you’ll save the wrong ID). Replace ID auto-reconnects the account to Dokan after saving.
- **No matching account at all.** The account was either deleted, was on a different Stripe platform that’s since been disconnected, or had its application access revoked. Use **Recreate** on the row. The club will need to redo onboarding (bank details) on the new account.
- **The account is there with the same ID as WP.** Click **Re-check all accounts against Stripe** at the top of the table to refresh the cache, then look again. If Error persists, contact Sarah.



### **Backslashes in account names**

If Stripe Dashboard shows a club name with a literal backslash (for example, `Catholic Students' Society`), this is leftover from an older POST-handling bug. New accounts don’t pick up the slashes any more. Click **Fix slashed names on Stripe** at the top of the table to clean up the historical ones. The fix is idempotent: accounts with clean names are skipped.

Some fully-verified non-profit accounts have their company name locked by Stripe and won’t accept the update. For those, the alert reports Stripe’s exact rejection message; the next step is to email Stripe Support requesting a manual name update.