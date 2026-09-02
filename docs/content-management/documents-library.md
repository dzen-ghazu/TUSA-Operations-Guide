---
title: Managing the Documents Library
hide:
  - toc
---
# **TUSA Page Builder Guide**

A complete guide to editing pages on the TUSA website using Gutenberg and our custom blocks.

---



## **Table of Contents**



- [Creating a New Page](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/content-management/tusa-page-builder-guide/#creating-a-new-page)
- [Understanding Your Tools](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/content-management/tusa-page-builder-guide/#understanding-your-tools)
- [Getting Started – The Editor Interface](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/content-management/tusa-page-builder-guide/#getting-started---the-editor-interface)
- [The List View – Your Best Friend](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/content-management/tusa-page-builder-guide/#the-list-view---your-best-friend)
- [Understanding Block Types](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/content-management/tusa-page-builder-guide/#understanding-block-types)
- [Editing Gutenbricks Blocks](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/content-management/tusa-page-builder-guide/#editing-gutenbricks-blocks-tusa-custom-blocks)
- [Block Settings vs Page Settings](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/content-management/tusa-page-builder-guide/#block-settings-vs-page-settings)
- [Featured Images and Headers](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/content-management/tusa-page-builder-guide/#featured-images-and-headers)
- [Page Excerpts](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/content-management/tusa-page-builder-guide/#page-excerpts---always-add-one)
- [What You CAN Edit](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/content-management/tusa-page-builder-guide/#what-you-can-edit)
- [What You CANNOT Edit](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/content-management/tusa-page-builder-guide/#what-you-cannot-edit)
- [Creating Layouts Step by Step](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/content-management/tusa-page-builder-guide/#creating-layouts-step-by-step)
- [Block Settings and Customisation](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/content-management/tusa-page-builder-guide/#block-settings-and-customisation)
- [Common Tasks](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/content-management/tusa-page-builder-guide/#common-tasks)
- [When Things Go Wrong](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/content-management/tusa-page-builder-guide/#when-things-go-wrong)
- [Best Practices Summary](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/content-management/tusa-page-builder-guide/#best-practices-summary)
- [Getting Help](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/content-management/tusa-page-builder-guide/#getting-help)

---



## **Creating a New Page**



Before you can add content, you need to create the page itself. Here’s the step-by-step process.



### **Step 1: Go to Pages**



- In WordPress admin, go to **Pages** in the left menu
- Click **Add New**



### **Step 2: Set the Page Title**



- At the top of the editor, you’ll see “Add title”
- Type your page title
- This becomes the page heading AND part of the URL

**Title tips:**

- Keep it clear and descriptive
- Use sentence case (capitalise first word and proper nouns only)
- Avoid special characters



### **Step 3: Set the Parent Page (Important!)**



The parent page determines where your page sits in the site hierarchy and navigation.

- Look at the **Page Settings panel** on the right (click the Page tab if needed)
- Find **“Page Attributes”** or **“Parent”**
- Select the correct parent page from the dropdown


| If your page is… | Parent should be… |
| ------------------------ | ----------------- |
| A main section page | (no parent) |
| A sub-page of Clubs | “Clubs” |
| A sub-page of Events | “Events” |
| A sub-page of About TUSA | “About TUSA” |


**Why this matters:**

- Controls breadcrumb navigation
- Affects URL structure
- Determines where it appears in menus (if added)
- Helps with site organisation



### **Step 4: Set the Featured Image**



The featured image appears in the page header and when the page is shared.

- In Page Settings panel, find **“Featured Image”**
- Click **“Set featured image”**
- Upload a new image or choose from Media Library
- Click **“Set featured image”** to confirm

**Image requirements:**

- Landscape orientation works best
- Important content should be in the centre (headers crop from edges)
- Minimum 1200px wide recommended



### **Step 5: Add the Page Excerpt**



**Always add an excerpt** – it’s used for search results, page cards, and social sharing.

- In Page Settings panel, find **“Excerpt”** (may need to scroll or click a button to expand)
- Write 1-2 sentences describing what the page is about
- Keep it brief and informative

**Example excerpts:**

- “Learn how to apply for TUSA grants and funding for your club activities.”
- “Find out about volunteering opportunities at TUSA Food Hub locations.”



### **Step 6: Add Your Content**



Now you’re ready to build the page content using the editor. See the sections below for how to:

- Use the editor interface
- Add and arrange blocks
- Create layouts



### **Step 7: Preview and Publish**



- Click **Preview** to see how the page looks
- Check the featured image displays correctly
- Review your content
- When ready, click **Publish**

If editing an existing page, you’ll see **Update** instead of Publish.



### **Quick Checklist for New Pages**



Before publishing, confirm:

- [ ] Page title is set
- [ ] Parent page is correct
- [ ] Featured image is added
- [ ] Excerpt is written
- [ ] Content is complete
- [ ] Preview looks correct

---



## **Understanding Your Tools**



&nbsp;

### **What Are These Tools?**




| Tool | What It Is | Your Role |
| ------------------- | --------------------------------------- | ---------------------------------------- |
| **Gutenberg** | WordPress’s built-in block editor | This is what you use to edit pages |
| **Bricks** | Professional page builder for templates | Developers use this – you don’t touch it |
| **Gutenbricks** | Our custom blocks | These appear as blocks you can use |
| **WP Grid Builder** | Dynamic content grids | Display only – cannot be edited by you |


### **Why It Works This Way**



This system was built so you can edit content **without breaking anything**:

- **Edit safely** – You can’t accidentally break the site’s design
- **No waiting** – Make updates instantly without developer help
- **Automatic styling** – Everything follows TUSA brand guidelines automatically
- **Professional results** – Get designer-quality pages without design experience

---



## **Getting Started – The Editor Interface**



When you open a page to edit, you’ll see the Gutenberg editor. Here’s what you’re looking at:



```
┌─────────────────────────────────────────────────────────────────┐
│  [←]  Page Title                              [Preview] [Update]│  ← Top Toolbar
├─────────────────────────────────────────────────────────────────┤
│                                                    │            │
│                                                    │  Settings  │
│              Page Content Area                     │   Panel    │
│                                                    │    (→)     │
│            (What you're editing)                   │            │
│                                                    │            │
├─────────────────────────────────────────────────────────────────┤
│  [+] Add Block                     [≡ List View]  [⚙ Settings] │  ← Bottom/Side Tools
└─────────────────────────────────────────────────────────────────┘

```



&nbsp;

### **Key Areas to Know**




| Area | Location | Purpose |
| ------------------ | -------------------- | ------------------------------ |
| **Top Toolbar** | Very top | Save, preview, undo/redo |
| **Content Area** | Centre | Where you edit the actual page |
| **Settings Panel** | Right side | Block and page settings |
| **Block Inserter** | Blue [+] button | Add new blocks |
| **List View** | Three lines icon (≡) | See page structure |


---



## **The List View – Your Best Friend**



**This is the most important tool you need to learn.** When you feel lost on a page, open List View.



### **How to Open List View**



- Look for the **three horizontal lines icon (≡)** in the top toolbar
- Click it
- A panel opens showing your entire page structure



```
List View Panel:
├── Group
│   ├── Heading
│   ├── Paragraph
│   └── Image
├── Spacer
├── Group
│   ├── Columns
│   │   ├── Column
│   │   │   └── Heading
│   │   └── Column
│   │       └── Paragraph
│   └── Button
└── Spacer

```



&nbsp;

### **Why List View Matters**




| Problem | How List View Helps |
| ---------------------------------------- | --------------------------------------- |
| “I can’t find something” | See ALL blocks on the page |
| “I clicked but selected the wrong thing” | Click exactly what you want in the list |
| “I don’t know what’s inside what” | See the nested structure clearly |
| “I need to move something” | Drag and drop in the list |
| “I accidentally deleted something” | Notice immediately in the list |


### **Using List View**



**To select a block:** Click its name in the list

**To expand/collapse:** Click the arrow (▶) next to groups

**To move blocks:** Drag and drop within the list

**To see what’s selected:** It highlights in the list AND on the page



### **Pro Tip: Keep List View Open**



While editing complex pages, keep List View open on the left side. It makes everything easier.

---



## **Understanding Block Types**



&nbsp;

### **How to Identify Block Types**



When you click [+] to add a block or look at List View, you’ll see different icons:


| Icon | Meaning |
| --------------- | ---------------------------------------------------- |
| **TUSA logo** | Custom TUSA block – built specifically for this site |
| **Other icons** | Standard Gutenberg blocks |
| **Grid icon** | WP Grid Builder – DO NOT EDIT |


### **Our Custom TUSA Blocks (TUSA logo icon)**



Blocks showing the **TUSA logo** as their icon are custom-built for TUSA. Look for it when browsing  
blocks or scanning List View: if a block carries the TUSA logo, it was made specifically for our site.  
Everything else is either a standard WordPress block or a plugin block.

These include:

- Pre-built sections with TUSA styling
- Special functionality blocks
- Branded components

**These are safe to use** – they’re designed to look right automatically and follow brand guidelines.



### **Standard Gutenberg Blocks**



All other blocks are standard WordPress blocks:


| Block | Use For |
| ------------- | --------------------------------- |
| **Paragraph** | Regular text |
| **Heading** | Section titles (H1, H2, H3, etc.) |
| **Image** | Single images |
| **List** | Bullet or numbered lists |
| **Group** | Container for other blocks |
| **Columns** | Two-column layouts |
| **Spacer** | Vertical spacing between sections |
| **Button** | Clickable buttons |


### **WP Grid Builder Blocks & Shortcodes – DO NOT EDIT**



**You will see WP Grid Builder blocks and shortcodes on pages. DO NOT try to edit them.**



#### **WP Grid Builder Blocks**



These blocks display dynamic content from the database:

- Club directories
- Event listings
- Staff grids
- Filtered content displays

**Why you can’t edit them:**

- They pull live data from multiple systems
- The layouts are controlled by custom code
- Changing them could break data connections
- The styling is precisely calibrated

**How to recognise them:**

- They show “WP Grid Builder” in the block name
- They often display cards or grids of content
- The content updates automatically (you’ll see different data each time)



#### **Shortcodes**



Shortcodes look like this: `[something_here]` or `[shortcode param="value"]`

These are also backend functionality that you cannot edit directly. Sometimes we use shortcodes instead of WP Grid Builder blocks – they serve similar purposes.

**If you see a shortcode:** Don’t modify it. If you need changes to what it displays, contact the dev team.

**What to do if you need changes to either:**  
Contact the development team. We need to modify the underlying queries, templates, or shortcode parameters.

---



## **Editing Gutenbricks Blocks (TUSA Custom Blocks)**



Our custom TUSA blocks (the ones showing the TUSA logo icon) have special editing panels. Here’s how to use them.



### **How to Edit a Gutenbricks Block**



- **Select the block** (click it or use List View)
- **Look at the Settings Panel** on the right side
- The panel shows different tabs/sections for that block



### **Common Gutenbricks Settings**



&nbsp;

#### **Editing Buttons**



To edit a button inside a Gutenbricks block:

- **Click directly on the button** in the content area
- A small toolbar appears with:

– Text editing (type to change button text)  
– Link icon (click to set the URL)

- Or use the Settings Panel > Button section

**Note:** Button settings (visibility, style) are usually in a “Button” section in the Settings Panel.



#### **Visibility Settings**



Many blocks have visibility toggles to show or hide elements:

- Select the block
- Look for **“Visibility”** or **“Show/Hide”** options in Settings Panel
- Toggle elements on/off as needed

This lets you hide parts of a block you don’t want to display without deleting them.



#### **Styles Panel**



To change colours or background images:

- Select the block
- Find the **“Styles”** section in the Settings Panel
- Options may include:

– Background colour  
– Background image  
– Text colours  
– Borders

**Remember:** All colour options are from the approved TUSA palette – you can’t go off-brand!



#### **Animation Settings**



Some blocks have optional animations:

- Select the block
- Look for **“Animation”** in the Settings Panel
- Toggle **“Animation Visible”** or similar to ON
- Then choose which animation from the dropdown

**Tip:** Use animations sparingly – they should enhance, not distract.

---



## **Block Settings vs Page Settings**



This is a common source of confusion. The Settings Panel on the right shows DIFFERENT things depending on what’s selected.



### **Block Settings**



**When you have a block selected**, the panel shows settings for THAT BLOCK:

- Block-specific options
- Colours and styles for that block
- Visibility toggles
- Advanced settings (CSS classes)

**How to know you’re in Block Settings:**

- A block is highlighted/selected on the page
- The panel header shows the block name (e.g., “Group”, “Heading”)



### **Page Settings**



**When NO block is selected**, the panel shows settings for THE PAGE:

- Page title
- URL slug
- Featured image
- Page excerpt
- Template selection
- Publication settings

**How to get to Page Settings:**

- Click somewhere empty on the page (not on a block)
- Or click the page title at the very top
- Or look for a “Page” tab at the top of the Settings Panel



### **Quick Switch**



At the top of the Settings Panel, you may see tabs:

- **Block** – Settings for selected block
- **Page** (or document icon) – Settings for the page

Click these to switch between them.

---



## **Featured Images and Headers**



&nbsp;

### **What is the Featured Image?**



The **Featured Image** for a page is what appears in the header section at the top of the page. This is set in the **Page Settings** (not Block Settings).



### **Setting a Featured Image**



- Make sure no block is selected (click empty area)
- In the Settings Panel, find **“Featured Image”**
- Click to set or change the image
- Choose from Media Library or upload new



### **Header Images Are Centred**



All header sections **centre the image both horizontally and vertically**. This means:

- The middle of your image is what shows most prominently
- The top and bottom may be cropped depending on screen size
- Very tall images may have the top cut off



### **If Your Header Image Doesn’t Look Right**



If the image isn’t sitting correctly (e.g., important content is cut off at the top):

**You may need to crop the image:**

- Go to **Media Library** (Media > Library in admin menu)
- Find your image and click to open it
- Click **“Edit Image”** below the image
- Use the **crop tool** to trim the top of the image
- This moves the “centre point” down
- Save the cropped version
- Re-select it as the Featured Image

**Cropping Tips:**

- Crop from the TOP if heads are being cut off
- Aim to put the most important content in the vertical centre
- Preview the page after changing to check the result

---



## **Page Excerpts – ALWAYS ADD ONE**



**Every page should have an excerpt.** This is used throughout the site for page summaries, search results, and previews.



### **What is a Page Excerpt?**



A short summary of what the page is about (1-2 sentences). It appears:

- In search results
- In page listings and cards
- When the page is shared on social media
- In various navigation elements



### **How to Add a Page Excerpt**



- **Open the page for editing**
- **Make sure no block is selected** (click empty area)
- Look for the **blue “Excerpt” button** or find “Excerpt” in Page Settings
- Click to open the excerpt field
- **Write a brief summary** (1-2 sentences describing the page)
- Save/Update the page



### **Writing Good Excerpts**



**Do:**

- Keep it brief (1-2 sentences)
- Describe what the page is about
- Use plain language
- Include key information someone would want to know

**Don’t:**

- Leave it blank
- Copy the entire first paragraph
- Use “This page is about…”
- Include formatting or links

**Example excerpts:**

- “Find out how to join TUSA clubs and societies and get involved in student life.”
- “Information about Food Hub locations, opening hours, and how to access free groceries.”
- “Submit a risk assessment for your upcoming club event or activity.”

---



## **What You CAN Edit**



&nbsp;

### **Safe to Edit Yourself**




| Content Type | How to Edit |
| -------------------- | ----------------------------------------- |
| **Text/headings** | Click directly and type |
| **Images** | Click and use Replace in toolbar |
| **Buttons** | Click to edit text, use settings for link |
| **Spacer size** | Select and adjust in settings panel |
| **Page excerpts** | Use the blue excerpt button |
| **Block visibility** | Toggle in block settings |
| **Block order** | Drag in List View |


### **Adding New Content**



You can safely add:

- New text blocks
- New images
- New Groups with content inside
- New Columns layouts
- New Spacers
- Any block from the TUSA custom blocks (
  ![🔗](https://s.w.org/images/core/emoji/17.0.2/svg/1f517.svg)

  )

---



## **What You CANNOT Edit**



&nbsp;

### **Do Not Touch – Contact Dev Team**




| Item | Why | What To Do Instead |
| ---------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------ |
| **WP Grid Builder blocks** | Complex data connections | Contact dev team |
| **Shortcodes** | Backend functionality | Contact dev team |
| **Template areas** | Controlled by Bricks | Contact dev team |
| **Header/Footer** | Site-wide templates | Contact dev team |
| **Navigation menus** | Managed separately | Contact dev team |
| **Anything inside the Forms menu** | Forms are now wired into automation — affiliations, grants, events, webhooks, emails, payments. Edits need to land across everything attached at once. | Send through to dev team |
| **Form embeds on a page** | The`Oops! We could not locate your form.`shortcode is placed deliberately | Send through to dev team |


### **Signs You’re in the Wrong Place**



**Stop and ask for help if:**

- You see code or shortcodes like `[shortcode_name]`
- You’re in the Bricks editor (not Gutenberg)
- You see “Template” in the editing interface
- You’re editing something in Appearance > Widgets
- The page looks completely different from what you expected

---



## **Creating Layouts Step by Step**



&nbsp;

### **The Basic Pattern**



Almost every section follows this pattern:



```
Group (container)
  └── Your content
Spacer (breathing room)

```



&nbsp;

### **Creating a Basic Content Section**



**Step 1:** Add a Group block

- Click the blue [+] button
- Search for “Group”
- Click to add it

**Step 2:** Add content inside the Group

- Click inside the Group
- Click [+] to add blocks inside
- Add headings, text, images, etc.

**Step 3:** Add a Spacer after the Group

- Click outside/below the Group
- Add a Spacer block
- This creates consistent spacing



### **Creating Two-Column Layouts**



**Best for:** Text beside images, split content



#### **Understanding Group Structures**



When you add a Group block, it asks you to choose a layout structure. **This is important:**

- **If you choose “Columns” directly in the Group**, it turns the Group itself into columns
- **If you want columns INSIDE a Group** (recommended), choose **One Column** first, then add a separate Columns block inside



#### **Content-Width Two Columns (Recommended)**



This keeps your columns aligned with the rest of your page content, with proper padding on the sides.

**Step 1:** Add a Group block

- Click [+] and add a Group
- **Choose “One Column” structure** when prompted

**Step 2:** Add a Columns block inside the Group

- Click inside the Group
- Click [+] and search “Columns”
- **Choose “Two Columns” structure** when prompted

**Step 3:** Add content to each column

- Click in left column, add your content
- Click in right column, add your content

**Step 4:** Add Spacer after the Group



```
Result:
Group (One Column) ← Sets content width
  └── Columns (Two Column)
        ├── Column 1 - Your content
        └── Column 2 - Your content
Spacer

```



&nbsp;

#### **Full-Width Two Columns (Edge to Edge)**



If you want columns that span the entire page width with no padding on either side, put the Columns block **outside** of a Group.

**Step 1:** Add a Columns block directly (not inside a Group)

- Click [+] and add Columns
- Choose “Two Columns” structure

**Step 2:** Add content to each column

**Note:** This is less common – most of the time you want content-width columns.



### **Creating Three+ Column Layouts**



**Important:** For 3+ columns, use Grid blocks with a special class.

**Step 1:** Add a Group block

**Step 2:** Inside the Group, add a Grid block

**Step 3:** Add the responsive class

- Select the Grid block
- Open Settings panel (right side)
- Expand “Advanced” section
- In “Additional CSS class(es)” add: `threecolgutgrid`

**Step 4:** Add content to grid items

**Step 5:** Add Spacer after the Group

---



## **Block Settings and Customisation**



&nbsp;

### **Accessing Settings**



- **Select a block** (click it or use List View)
- **Look at the right panel** – this shows settings for that block
- **If panel is closed**, click the Settings icon (⚙) in top toolbar



### **Common Settings**




| Setting | Where to Find | What It Does |
| --------------------- | --------------------------- | ------------------- |
| **Text alignment** | Block toolbar | Left, centre, right |
| **Heading level** | Block toolbar | H1, H2, H3, etc. |
| **Background colour** | Settings panel > Colour | Block background |
| **Text colour** | Settings panel > Colour | Text colour |
| **Spacing** | Settings panel > Dimensions | Padding/margins |
| **Advanced** | Settings panel > Advanced | CSS classes |


### **Heading Levels – Important!**



Use headings in order for accessibility:

- **H1** – Main page title (usually only one per page)
- **H2** – Major sections
- **H3** – Subsections within H2
- **H4** – Subsections within H3

**Wrong:** H1 → H3 → H2 (skipping around)  
**Right:** H1 → H2 → H3 → H2 → H3 (sequential)

---



## **Common Tasks**



&nbsp;

### **Editing Existing Text**



- Click directly on the text
- Type your changes
- Click Update to save



### **Replacing an Image**



- Click on the image
- Click “Replace” in the toolbar that appears
- Upload new image or choose from Media Library
- Click Update to save



### **Adding a New Section**



- Open List View to see where to add it
- Click where you want the new section
- Click [+] and add a Group
- Add content inside the Group
- Add a Spacer after
- Click Update to save



### **Moving a Section**



- Open List View
- Find the section (usually a Group)
- Drag it to the new position
- Click Update to save



### **Deleting a Section**



**Important:** You must delete the BLOCK itself, not just clear its content. If you just select all the text and delete it, you’ll have an empty block left behind.

**To delete a single block:**

- Open List View
- Click on the block to delete (it turns blue/highlighted)
- Press Delete key, or click the three dots (⋮) and choose “Remove”
- Click Update to save

**To delete multiple blocks at once:**

- Open List View
- Hold **Ctrl** (Windows) or **Cmd** (Mac)
- Click each block you want to delete (they turn blue)
- Press **Delete** key
- All selected blocks are removed
- Click Update to save

**Common mistake:** Selecting text inside a block and pressing Delete only clears the text – the empty block remains. Always select the block itself (use List View!) and delete the whole block.



### **Duplicating a Section**



- Open List View
- Click on the section to duplicate
- Click the three dots (⋮) in the toolbar
- Choose “Duplicate”
- Edit the copy as needed
- Click Update to save

---



## **When Things Go Wrong**



&nbsp;

### **“I’m lost on the page”**



**Solution:** Open List View (≡ icon in toolbar)

- See the full page structure
- Click exactly what you want to select
- Understand what’s nested inside what



### **“I selected the wrong thing”**



**Solution:** Use List View to select precisely

- Don’t click randomly on the page
- Click the exact block name in List View



### **“I can’t find where to type”**



**Solution:** Look for the cursor or click in List View

- Some blocks need you to click inside them first
- List View shows you exactly what you have



### **“Something disappeared”**



**Solution:** Use Undo immediately

- Press Ctrl+Z (Windows) or Cmd+Z (Mac)
- Or click the Undo arrow in the top toolbar
- You can undo multiple times



### **“The page looks broken”**



**Solution:** Don’t panic – you probably haven’t saved yet

- Click Preview to see actual page
- If Preview looks wrong, DON’T click Update
- Use Undo to reverse changes
- If you already saved and it’s broken, contact dev team



### **“I see code or shortcodes”**



**Solution:** Don’t edit these directly

- Shortcodes like `[something]` are backend functionality
- Editing them may break features
- Contact dev team for changes



### **“I accidentally edited something I shouldn’t have”**



**Solution:** Undo and/or don’t save

- Ctrl+Z / Cmd+Z to undo
- If unsure, close without saving (click X, choose “Don’t save”)
- Refresh the page to start fresh

---



## **Best Practices Summary**



&nbsp;

### **DO These Things**

![✅](https://s.w.org/images/core/emoji/17.0.2/svg/2705.svg)




| Practice | Why |
| --------------------------------------------------- | ------------------------------------ |
| **Use List View** | Navigate pages easily |
| **Start with Groups** | Proper content containment |
| **Add Spacers between sections** | Consistent spacing |
| **Use Columns for 2-column layouts** | Works better than Grid |
| **Use Grid +** `threecolgutgrid` **for 3+ columns** | Proper responsiveness |
| **Keep headings sequential** | Accessibility |
| **Always add page excerpts** | Used in search, cards, social shares |
| **Preview before updating** | Catch problems early |
| **Save regularly** | Don’t lose work |
| **Click directly into text** | Fastest editing method |
| **Duplicate sections to reuse** | Saves time |


### **AVOID These Things**

![❌](https://s.w.org/images/core/emoji/17.0.2/svg/274c.svg)




| Practice | Why |
| ---------------------------------------------------- | -------------------------------- |
| **Editing WP Grid Builder blocks** | Breaks data connections |
| **Editing shortcodes** | Breaks backend features |
| **Using Accordion blocks** | Accessibility issues (see below) |
| **Skipping heading levels** | Accessibility issues |
| **Using Grid for 2 columns** | Columns work better |
| **Adding custom CSS yourself** | May break responsiveness |
| **Editing in Bricks** | That’s for developers |
| **Deleting things you don’t understand** | May break page |
| **Ignoring page excerpts** | Required for site features |
| **Just clearing content instead of deleting blocks** | Leaves empty blocks behind |


### **About Accordions – Important Warning**



**Avoid using Accordion blocks** unless specifically instructed to.

Accordions (expandable/collapsible sections) have significant accessibility requirements:

- They need proper ARIA attributes
- They need keyboard navigation
- They need focus management
- They need proper heading structure

Simply dropping an accordion block onto a page – even a TUSA custom one – may not have the correct parameters for your specific use case.

**Where accordions ARE properly set up:**

- Mobile navigation menu (carefully built with accessibility)
- Specific templates where we’ve configured them correctly

**If you think you need an accordion:** Contact the dev team. We can either set one up properly or suggest an alternative layout that’s more accessible.

---



## **Quick Reference Card**



&nbsp;

### **Keyboard Shortcuts**




| Action | Windows | Mac |
| ----------------------- | ----------------- | ----------------- |
| Undo | Ctrl + Z | Cmd + Z |
| Redo | Ctrl + Shift + Z | Cmd + Shift + Z |
| Save | Ctrl + S | Cmd + S |
| Add block | / (forward slash) | / (forward slash) |
| Select all | Ctrl + A | Cmd + A |
| Copy | Ctrl + C | Cmd + C |
| Paste | Ctrl + V | Cmd + V |
| **Multi-select blocks** | Ctrl + Click | Cmd + Click |
| Delete selected | Delete | Delete |
| Duplicate block | Ctrl + Shift + D | Cmd + Shift + D |


### **Common Blocks**




| Block | When to Use |
| ------------------------ | ---------------------- |
| Group | Container for sections |
| Columns | 2-column layouts |
| Grid + `threecolgutgrid` | 3+ column layouts |
| Spacer | Between sections |
| Heading | Section titles |
| Paragraph | Regular text |
| Image | Single images |
| Button | Call-to-action links |


---



## **Getting Help**



&nbsp;

### **Before Asking for Help**



- Try using **List View** to understand the page
- Use **Undo** if something went wrong
- Use **Preview** to check your changes
- Check this guide for your specific task



### **When to Contact Development Team**



Contact us for:

- WP Grid Builder changes
- Shortcode modifications
- Template changes
- New functionality
- Anything that looks like code
- When something is actually broken



### **How to Ask for Help**



When you contact us, please include:

- Which page you’re working on (URL)
- What you were trying to do
- What happened instead
- Screenshot if possible

---



## **Remember**



**You can’t break the site by editing content normally.** The system is designed to be safe.

If something looks wrong:

- Don’t panic
- Undo your changes (Ctrl+Z)
- Preview before saving
- Ask for help if needed

The most powerful tool is **List View**. When in doubt, open List View!