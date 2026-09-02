---
title: Managing Website Menus
hide:
  - toc
---
# **Managing Website Menus**



## **The Short Version**



You can add, remove, and rearrange menu items without editing the website template. Go to **Appearance > Menus** in your WordPress dashboard. Each section of the navigation has its own menu that you can edit independently.

**You do NOT need Bricks Builder, a developer, or any technical knowledge to manage menus.**

---



## **Menus vs Sitemap — What’s the Difference?**



These are two different things:


|  | Menu | Sitemap |
| -------------------------------------------- | -------------------------------------------------------- | ------------------------------------------------- |
| **What it is** | The navigation links visitors click on | A list of all pages on the site for Google |
| **Where it lives** | Appearance > Menus | Generated automatically by SEOPress |
| **Who manages it** | You — add/remove items anytime | Automatic — updates when you publish/delete pages |
| **What happens when you add a page** | Nothing — you choose whether to add it to a menu | It appears in the sitemap automatically |
| **What happens when you remove a menu item** | The link disappears from the nav — the page still exists | Nothing changes |


**Key point:** Adding a page to the website does NOT automatically add it to the navigation menu. You need to add it manually in Appearance > Menus. Similarly, removing a menu item does NOT delete the page — it just removes the link from the navigation.

---



## **How the Navigation Is Set Up**



The main navigation uses **mega menu dropdowns**. Each dropdown (About, Support, Events, etc.) contains columns, and each column is powered by a separate WordPress menu.



### **The Dropdown Sections and Their Menu Names**



Each column in the navigation is a separate WordPress menu. Here are the exact menu names as they appear in **Appearance > Menus**:


| Navigation Dropdown | Menu Name in WordPress | What it controls |
| ------------------- | ------------------------------------ | ------------------------------- |
| **About** | `About TUSA` | Main About TUSA links |
| **About** | `About TUSA > Board` | Board and governance links |
| **About** | `About TUSA > Important Stuff` | Key documents and info |
| **Support** | `Support > Advocacy` | Advocacy services links |
| **Support** | `Support > Food` | Food Hub and food support links |
| **Support** | `Support > Wellbeing` | Wellbeing services links |
| **Support** | `Support > Financial Support` | Financial support links |
| **Events** | `Events` | Event categories and links |
| **Get Involved** | `Get Involved` | Ways to get involved |
| **Representation** | `Representation > Your Reps` | Your Reps links |
| **Representation** | `Representation > Equity` | Equity pages |
| **Representation** | `Representation > Student Feedback` | Student feedback links |
| **Representation** | `Representation > Student Elections` | Elections links |
| **Clubs** | `Clubs > find a club` | Finding and joining clubs |
| **Clubs** | `Clubs > resources` | Club resources and admin |
| **Footer** | `Footer > Site Policies` | Privacy, terms, accessibility |
| **Footer** | `Footer > What we do` | Footer navigation links |


Each menu is independent. Editing “Support > Food” only changes the Food column — nothing else is affected.

---



## **How to Edit a Menu**



&nbsp;

### **Step 1: Go to Appearance > Menus**



In your WordPress dashboard, go to **Appearance > Menus** in the left sidebar.



### **Step 2: Select the Menu to Edit**



Use the dropdown at the top to select which menu you want to edit. The menus are named to match their location in the navigation (e.g., “Support – Advocacy Column”, “Clubs – Resources Column”).



### **Step 3: Add Items**



On the left side, you’ll see panels for **Pages**, **Posts**, **Custom Links**, and **Categories**. To add an item:

- Expand the panel (e.g., Pages)
- Tick the page(s) you want to add
- Click **Add to Menu**
- The item appears at the bottom of the menu on the right



### **Step 4: Rearrange Items**



Drag and drop menu items to reorder them. You can also drag items slightly to the right to make them sub-items (indented under a parent).



### **Step 5: Remove Items**



Click the small arrow on any menu item to expand it, then click **Remove**.



### **Step 6: Save**



Click **Save Menu** at the bottom. Your changes are live immediately.

---



## **Important Rules**



- **Don’t rename the menus themselves** — the names are linked to their position in the template. Renaming a menu could break its connection to the navigation.
- **Don’t delete a menu** — if you want to remove all items from a section, remove the individual items instead. Deleting the menu itself will leave a blank space in the navigation.
- **You can add any type of content** — pages, posts, custom links (external URLs), categories. They all work the same way in menus.
- **The mobile menu uses the same menus** — any changes you make will appear in both the desktop mega menu and the mobile hamburger menu.
- **Menu changes are instant** — there’s no need to clear cache or rebuild anything. Save and it’s live.

---



## **Adding a New Page to the Navigation**



When you create a new page on the site, it will NOT automatically appear in the navigation. To add it:

- Create and publish the page as normal
- Go to **Appearance > Menus**
- Select the menu for the correct navigation column
- Find your new page in the Pages panel on the left
- Tick it and click **Add to Menu**
- Drag it to the correct position
- Click **Save Menu**

---



## **Common Tasks**



&nbsp;

### **“I want to add a new page under Support > Food”**

- Go to Appearance > Menus
- Select `Support > Food` from the dropdown
- Add your page from the Pages panel on the left
- Drag it to the right position
- Click Save Menu



### **“I want to remove a page from the Clubs dropdown”**

- Go to Appearance > Menus
- Select `Clubs > resources` (or `Clubs > find a club`, whichever column it’s in)
- Expand the item you want to remove
- Click Remove
- Click Save Menu

**Remember:** removing a menu item does NOT delete the page. The page still exists on the site — it just won’t have a navigation link.



### **“I want to reorder items in a dropdown column”**

- Go to Appearance > Menus
- Select the menu
- Drag items up or down
- Save

---



## **What You Should NOT Do**



- **Don’t edit the Bricks Builder template** — the mega menu structure (columns, styling, animations) is set in the template. Editing it can break the navigation layout across the whole site.
- **Don’t add more columns** — the number of columns per dropdown is fixed in the template. If you need a new column, that’s a developer task.
- **Don’t change menu assignments** — each menu is assigned to a specific location in the template. Changing which menu is assigned where will break the layout.

If you need structural changes to the navigation (new dropdowns, new columns, different layout), that’s a separate piece of work. Menu items within the existing structure are yours to manage.