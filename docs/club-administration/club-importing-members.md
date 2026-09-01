---
title: Importing Club Members via CSV
hide:
  - toc
---
# **Importing Club Members via CSV**

At the start of each year, clubs may need to import their existing members from another system. The CSV import tool lets TUSA staff (or club admins) bulk-import members into a club, creating accounts and applying membership tags in one step.

---



## **Where to Find It**

The import tool is inside each club’s group:

**Club Group → Club Admin → CSV Import**

You must be logged in as a **group admin**, **group moderator**, or **site admin** to see and use the import tool.

---



## **Preparing the CSV File**

The CSV file needs these columns in this order:


| Column | Required | Notes |
| ------------------ | -------- | ------------------------------------------ |
| **First Name** | Yes |  |
| **Family Name** | Yes | Last name / surname |
| **Email** | Yes | Must be a valid email address |
| **Student Number** | No | Stored in the member’s profile if provided |


The importer is flexible with column headers — it recognises variations like “first_name”, “firstname”, “given_name”, “surname”, “last_name”, “email_address”, “student_id”, etc.



### **Example CSV**

```
First Name,Family Name,Email,Student Number
Jane,Smith,jane.smith@utas.edu.au,123456
Tom,Jones,tom.jones@utas.edu.au,789012

```



---



## **Step-by-Step Process**

### **Step 1: Select Membership Tags**

The tool automatically shows the membership tags that match the club name. Select the tags you want applied to every imported member (e.g., the club’s current year membership tag).

Hold **Ctrl** (or **Cmd** on Mac) to select multiple tags.

> If no tags appear, the club’s membership tags haven’t been set up yet. Contact the TUSA web person to create them before importing.



### **Step 2: Upload the CSV**

Drag and drop the CSV file onto the upload area, or click to browse. The file must be a `.csv` file.



### **Step 3: Review the Preview**

The tool reads the file and shows a preview table:

- **Green rows** — Valid, ready to import
- **Red rows** — Invalid (missing email, invalid email, or missing name)
- Stats at the top show total, valid, and invalid counts
- Preview shows the first 50 rows — larger files are still fully imported, but only previewed partially

**Check the preview carefully before importing.** Invalid rows are skipped automatically.



### **Step 4: Click “Start Import”**

Confirm the import when prompted. The tool processes members in batches of 5 and shows a live log:

- **Created** (green) — New account created, tags applied, added to group
- **Updated** (blue) — User already existed, tags applied, added to group if not already a member
- **Error** (red) — Something went wrong for that row



### **Step 5: Review the Summary**

After import completes, you’ll see counts of created, updated, and errored records.

---



## **What the Import Does**

### **For new users (email doesn’t already exist on the site)**

- Creates a site account with the customer role
- Sets the profile type based on whether a student number was provided:

– **With student number** → student profile type  
– **Without student number** → hire-store-customer profile type

- Generates a random password (they’ll need to use “Lost Password” to set one)
- Sets their student number in their profile (if provided)
- Applies the selected membership tags
- Adds them to the club’s group

### **For existing users (email already on the site)**

- Applies the selected membership tags
- Adds them to the club’s group (if not already a member)
- Does **not** overwrite any existing profile data

This means **duplicates are handled safely** — importing the same person twice won’t create a second account. They’ll just get the tags applied again.

---



## **Common Scenarios**

### **Club transitioning from another membership system**

This is the primary use case. The club exports their member list from the old system as a CSV and imports it here. All members get accounts and the correct membership tags in one go.

### **Re-tagging members at the start of a new year**

If the club needs to apply a new year’s membership tag to their existing members, they can export their current member list and re-import it with the new tag selected. Existing users will just get the new tag — no duplicates.

---



## **Troubleshooting**

### **“No matching tags found”**

The tool filters membership tags by the club’s group name. If no tags match:

- Check that membership tags have been set up for this club
- Check that the tag names contain the club name (the tool matches on the club group name)
- If neither helps, contact the TUSA web person — they can set up the missing tags

### **CSV won’t upload**

- Make sure it’s a `.csv` file (not `.xlsx`)
- If exported from Excel, use “Save As → CSV (Comma delimited)”
- Check there are no special characters in the filename

### **All rows showing as invalid**

- Check the column headers match what the tool expects (First Name, Family Name, Email, Student Number)
- Make sure emails are valid (no spaces, proper format)
- Every row needs at least a first name or last name plus a valid email 

### **Some members showing as “Updated” instead of “Created”**

This means those email addresses already had site accounts. The import applied tags and added them to the group, but didn’t create new accounts. This is normal and expected — it’s the duplicate protection working.

### **Members can’t log in after import**

New accounts are created with a random password. Members need to use the **Lost Password** / **Reset Password** flow on the login page to set their own password. They won’t receive a welcome email with credentials automatically.

---



## **When something goes wrong that isn’t covered above**

Don’t try to diagnose or fix it yourself — see [Reporting an Issue](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/club-administration/importing-club-members-via-csv/#reporting-issues) for what to send so it can be looked at.
