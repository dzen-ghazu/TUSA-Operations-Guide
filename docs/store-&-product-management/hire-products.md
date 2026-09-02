---
title: Managing Hire Store Products
hide:
  - toc
---
# **Managing Hire Store Products**

The Hire Store handles rental equipment — marquees, BBQs, audio gear, and other items clubs can hire for events.

---



## **Who Can Manage This**



- **Site administrators** — full access via the site admin
- **Hire Store staff** — manage products through the Store Manager (the front-end store dashboard)

---



## **Accessing via Store Manager (Frontend)**



If you are a member of the Hire Store team:

- Go to your **Profile**
- Click the **Store Manager** tab
- You should see “Hire Store” at the top — confirm you are in the right store
- Click **Products** to see existing hire items or add new ones

---



## **Accessing via the Site Admin (Administrators)**



- Go to **Products** in the site admin sidebar
- Filter or search for Hire Store products
- When creating a new product, make sure the **Vendor** field is set to **Hire Store**

---



## **Adding Hire Products**



Hire products are **rental products**:

- Click **Add New Product**
- Set the product type to the **rental** type
- Enter the details:

– **Product Name** — be specific (e.g., “3x3m Marquee – White”)  
– **Description** — condition notes, what is included, setup instructions

- Set the price (see **Setting the hire price** below)
- **Tick the “Hire Store” product category** (see warning below)
- Add clear product images showing the item
- Set how many you have if you are tracking quantity (e.g., “we have 4 marquees”)
- Publish



### **Setting the hire price**



Set the hire rate in the **Regular Price** box — the same price box you use for any other product. That is the hire price.

**If the item comes in different options** (for example a marquee in 3x3m, 3x6m and 6x6m):

Each option has its own row. In each row, fill in:

- **Regular Price** — the hire rate for that option
- **Security Deposit** — the bond for that option, if there is one
- **Stock** — how many of that option you have, if you are tracking it



### **Always tick the “Hire Store” category**



Every hire product must have the **Hire Store** category ticked. You can also tick more specific categories like Equipment, Furniture, Games, Audio Equipment, etc., but **Hire Store** is mandatory.

The product page template uses this category to show:

- How many of the item are available
- Pickup location information
- Other hire-specific content panels

Without the Hire Store category, those panels do not appear on the product page even though the rest of the booking form works. If you create a product and the “available” or “pickup location” sections are missing, this is almost always why.

---



## **Managing Availability**



- Stock levels determine how many of each item can be hired simultaneously
- When an item is hired (order placed), stock decreases
- When returned (order completed/refunded), update stock manually
- Set items to “Out of Stock” if they are damaged or being serviced

---



## **Pickup time settings (appointment-based booking)**



The Hire Store works on an **appointment** model: customers must select a specific hour for pickup and another for return. They cannot rock up whenever they like — the time slots in the booking form are the hire desk’s appointment slots.



### **Standard hours**



The store-wide standard is **hourly appointments from 10am to 4pm**. Each slot is named by its start time, but the customer has a one-hour window to actually arrive — so the 4pm slot effectively runs until 5pm. In practice this means:

- Earliest appointment: 10am (10am-11am window)
- Latest appointment: 4pm (4pm-5pm window)
- Total bookable slots per day: 7

This matches how the team operated the rental store on the previous booking system.



### **Where the standard is configured**



**Rentals → Settings → Catalog tab → “In person pick up/return defaults”**

The four time/fee fields on that page list the appointment slots a customer can choose. These are the only options the customer sees in the booking dropdowns, so this is where you change the available appointment times for the whole store.


| Setting | Value |  |  |  |  |  |  |
| ----------------------------------------- | ---------------------------------------------------------------------------- | --------- | --------- | --------- | --------- | --------- | --------- |
| Time restrictions | `Unrestricted` |  |  |  |  |  |  |
| Return date | `Same day (rent to date)` (or `Next day` — match the team’s operating model) |  |  |  |  |  |  |
| Pick up times/fees (multiple day rentals) | `1000:0.00` | 1100:0.00 | 1200:0.00 | 1300:0.00 | 1400:0.00 | 1500:0.00 | 1600:0.00 |
| Pick up times/fees (single day rentals) | same value |  |  |  |  |  |  |
| Return times/fees (multiple day rentals) | same value |  |  |  |  |  |  |
| Return times/fees (single day rentals) | same value |  |  |  |  |  |  |


Format is `HHMM:fee` separated by `|`. The `0.00` after each colon is the fee for that slot (no surcharge). If you ever want to charge for an inconvenient slot (e.g., $5 extra for after-hours collection), change the number: `1700:5.00` adds a $5 fee to the 5pm slot.



### **Overriding the standard for one product**



The standard is set at the plugin level so the team does not need to configure it on every product. When you create a new hire product, **leave the time fields on the product blank** — the product will automatically use the store-wide standard hours.

If a specific product needs different hours (for example, a piece of equipment that can only be picked up during business hours, or a high-value item that needs same-day return only), edit the product, scroll to the Rental section, and fill in custom values for that product. Per-product values **override** the standard hours for that one product only.

To revert a product back to the standard hours later, clear the fields and save.



### **“Time restrictions” must stay on Unrestricted**



The **Time restrictions** dropdown directly above the four time fields must stay on **Unrestricted** — both globally and on any per-product override.

If it gets switched to **Restricted**, every hire product page will display “In person pick up/return is unavailable” and the booking form will not accept dates, even though times are configured correctly. The Restricted mode is built for self-service lockers where the math of pickup-vs-return times prevents overlap; it does not fit a staffed desk that is open the same hours both ends. The booking form already enforces appointment-only bookings through the slot list itself — customers cannot pick midnight because midnight is not in the list.

---



## **Important Notes**



- Hire Store products have different pickup/return logistics than regular products
- Revenue from the Hire Store goes to TUSA
- The Hire Store has its own location settings (Launceston and/or Hobart)
- Be aware of the mixed-location cart warning — if a customer adds items from different pickup locations, they will see a notice

  
