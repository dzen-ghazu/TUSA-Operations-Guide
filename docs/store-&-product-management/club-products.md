---
title: Managing Club Store Products (Clubs super Admin)
hide:
  - toc
---
# **Managing Club Store Products (Clubs Super Admin)**

As a Clubs Super Admin, you can create and edit products for any club’s store through the site admin. This is for when clubs need help setting up their store, fixing product issues, or troubleshooting.

**This is different from managing TUSA or Hire Store products** — club store products belong to individual club vendor accounts and appear in each club’s own store.

---



## **Who Can Do This**



- **Clubs Super Admin** (`clubs_super` role) — via the site admin
- **Site administrators** — via the site admin
- **Club admins themselves** — via the Store Manager on their own store’s frontend (they do not need site admin access)

Clubs Super Admin manages products through the WordPress backend when clubs need assistance. Club presidents and treasurers manage their own products through the frontend Store Manager — see the [Club Admin Guide: Adding Products](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/store-product-management/club-guide/adding-products.md).

---



## **Accessing Club Products**



- Log into WordPress with your clubs_super account
- In the left sidebar, click **Products**
- You will see all products across ALL stores — TUSA Store, Hire Store, and every club store



### **Finding a Specific Club’s Products**



The product list shows everything. To narrow it down:

- Look for the **Vendor** column — this shows which store owns each product
- If the Vendor column is not visible, click **Screen Options** (top right) and enable it
- You can also search by product name or filter by category

---



## **Creating a Product for a Club**



&nbsp;

### **Step 1: Create the Product**



- Go to **Products > Add New**
- Enter the product details:

– **Product Name** — be clear and include the club name if helpful (e.g., “Chess Club Hoodie – Navy”)  
– **Price** — the regular selling price  
– **Description** — what the customer gets  
– **Product Image** — upload a clear photo  
– **Category** — select the appropriate category (Merchandise, Membership, Tickets)



### **Step 2: Assign to the Correct Club Store**



**This is the most important step. If you skip this or pick the wrong store, the product ends up in the wrong place.**

- Look for the **Vendor** or **Store** meta box — it appears on the right side of the product editor, or in the Dokan section of the product data tabs
- It may be labelled:

– “Sold by” with a dropdown  
– “Vendor” with a search/select field  
– Under the “Dokan” tab in the product data area

- **Select the club’s store** from the dropdown
- If you cannot find the club’s store, they may not have completed their vendor setup — check **Dokan > Vendors** for their profile

**Common mistakes:**

- Leaving the vendor as your own account (or blank) — the product ends up unassigned or in the wrong store
- Accidentally selecting “TUSA Store” or “Hire Store” instead of the club
- Not checking the vendor field at all — it defaults to the logged-in user



### **Step 3: Publish**



- Set status to **Published** (or **Draft** if the club is not ready yet)
- Click **Publish** or **Update**
- Verify the product appears on the club’s store page

---



## **Moving a Product Between Stores**



If a product was accidentally created in the wrong store:

- Open the product in the editor
- Find the **Vendor/Store** field
- Change it to the correct club’s store
- Click **Update**

The product immediately moves — it disappears from the old store and appears in the new one.

---



## **Common Tasks**




| Task | How |
| --------------------------------- | --------------------------------------------------------------- |
| Fix wrong price | Edit product > change price > Update |
| Fix wrong image | Edit product > replace Product Image > Update |
| Product not showing in club store | Check: Published? Has category? Assigned to correct vendor? |
| Product in wrong store | Change the vendor assignment |
| Add size/colour variations | Change to Variable Product, add attributes, generate variations |
| Set stock level | Edit > Inventory > enable Manage Stock > set quantity |
| Hide product temporarily | Change status to Draft (do not delete — they may want it back) |


---



## **What You Cannot Do**



Clubs Super Admin has product access but NOT:

- Plugin settings or WordPress settings
- Theme or page builder editing
- Code snippets or developer tools
- Coupon management (handled by site administrators)
- Editing or deleting administrator accounts

---



## **If Something Goes Wrong**



**“You are not allowed to edit this product”**

- Refresh the page — permissions may need a moment to apply after login
- If it persists, check that your clubs_super role is your FIRST WordPress role (role order matters — see [CLAUDE.md](http://CLAUDE.md) for details)

**“Product not showing in the club’s store page”**

- Is the product **Published**? (not Draft or Pending)
- Is it assigned to the **correct vendor**?
- Does it have a **category** selected?
- Does it have a **price** set? (even free items need $0)

**“I created a product but it appeared in the TUSA Store”**

- You forgot to change the vendor. Edit the product, change the vendor to the correct club, and Update.

---



## **Related Guides**



- [Managing TUSA Merch Store](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/store-product-management/managing-club-store-products-clubs-super-admin/#managing-tusa-store) — TUSA’s own merchandise
- [Managing Hire Store](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/store-product-management/managing-club-store-products-clubs-super-admin/#managing-hire-store) — rental equipment
- [Club Admin Guide: Adding Products](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/store-product-management/club-guide/adding-products.md) — for club admins using the frontend

