---
title: Managing TUSA Locations
hide:
  - toc
---
# **Managing TUSA Locations**

This guide explains how the TUSA Locations system works, what the different location categories are for, and how to edit location content correctly.

---



## **Table of Contents**

- [How Locations Work](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/content-management/managing-tusa-locations/#how-locations-work)
- [Location Categories](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/content-management/managing-tusa-locations/#location-categories)
- [The Fields on Every Location](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/content-management/managing-tusa-locations/#the-fields-on-every-location)
- [Why Separate Tiles Matter](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/content-management/managing-tusa-locations/#why-separate-tiles-matter)
- [What Content Goes on Each Tile](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/content-management/managing-tusa-locations/#what-content-goes-on-each-tile)
- [How the Hire Store Connects to Locations](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/content-management/managing-tusa-locations/#how-the-hire-store-connects-to-locations)
- [The Sharing Link and Map](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/content-management/managing-tusa-locations/#the-sharing-link-and-map)
- [Current Locations Reference](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/content-management/managing-tusa-locations/#current-locations-reference)
- [Common Mistakes](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/content-management/managing-tusa-locations/#common-mistakes)

---



## **How Locations Work**

TUSA Locations appear as a top-level item labelled **TUSA Locations** in the site admin sidebar (with a map pin icon). Each location is its own page that shows as a tile on the front end of the site.

Every location is assigned to one or more **Location Categories**. These categories control what type of service the tile represents, and which region it belongs to.

There are two kinds of category:

- **Service type** — what the location does (Office, Hire Store, Food Hub)
- **Region** — where the location is (nipaluna/Hobart, palanwina lurini kanamaluka/Launceston, pataway/Burnie)

A location tile should have **one service type** and **one region**. This is what allows students to filter and find what they need.

---



## **Location Categories**

### **Service Types**


| Category | What it means | What students are looking for |
| -------------- | ------------------------------------------------------------ | ---------------------------------------------- |
| **Office** | A TUSA office where students can speak to staff in person | Office hours, building/room, contact details |
| **Hire Store** | An equipment hire pickup/return point | Pickup hours, what’s available, how to collect |
| **Food Hub** | A food distribution point, community kitchen, or food pantry | Operating days/hours, what’s offered |


### **Regions**


| Category | Covers |
| ------------------------------------------ | ------------------------------------------ |
| **nipaluna/Hobart** | Sandy Bay campus and Hobart city locations |
| **palanwina lurini kanamaluka/Launceston** | Inveresk campus and Launceston locations |
| **pataway/Burnie** | West Park / Cradle Coast campus |


### **How to assign categories**

When editing a TUSA Location, you’ll see the **TUSA Location Categories** panel in the sidebar. Tick the relevant service type and region. For example, “Sandy Bay Hire Store” should have both **Hire Store** and **nipaluna/Hobart** ticked.

---



## **The Fields on Every Location**

When you edit a TUSA Location, you’ll see these fields below the main content editor:


| Field | What to put in it |
| ------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Location address** | The human-readable address, e.g. “1 Churchill Ave, Sandy Bay, TAS 7005” |
| **Sharing link** | A Google Maps share link for the location (get this from Google Maps > Share > Copy link) |
| **Street Address** (map) | An interactive OpenStreetMap. Search for the address, then place or adjust the marker on the correct building. This powers the map that students see on the tile. |


The **post content** (the main editor area) is where you put the brief details that display on the tile itself — opening hours, building/room name, etc.

The **featured image** is the photo that appears on the tile.

---



## **Why Separate Tiles Matter**

TUSA operates different services at its campuses. An office, a hire store, and a food hub may all be on the same campus — but they serve completely different student needs.

**A student looking for food hub hours does not want to read through office contact details and hire store pickup times to find them.** And a student looking for the office doesn’t want to scroll past food hub schedules.

That’s why each service gets its own tile, even when they share a campus or a building.



### **How categories power filtering**

Categories aren’t just labels — they control how students find locations.

When location tiles are displayed on the site, students can filter by category. If a student wants to find a food hub, they filter to **Food Hub** and see only the food hub tiles. If they want to find an office to speak to someone, they filter to **Office** and see only office tiles.

This only works if each tile has the right category and only contains information about that one service. If food hub hours are written inside an office tile, they’re invisible to anyone filtering for food hubs — the tile is categorised as Office, so it won’t show up.

That’s why you create **separate tiles for each service**, even when they’re at the same campus:

- **TUSA Office Launceston** — categorised as Office
- **Inveresk Food Hub** — categorised as Food Hub
- **Launceston Hire Store** — categorised as Hire Store

Each tile has its own category, its own map marker, its own sharing link, and only the content relevant to that service.



### **A real example of the problem**

Look at the current “Northern Tasmania” office tile. Its content is:

> **TUSA Launceston Office**

> Opening hours: Monday to Friday, 9:00am to 5:00pm

> > **Inveresk Food Hub**

> Opening hours: Wednesday & Thursday, 11:00am to 2:00pm

> > **Mail**

> PO Box 4093, Invermay 7248

The Food Hub info doesn’t belong here. There is already a separate “Inveresk Food Hub” tile (categorised as Food Hub) with its own map marker and its own sharing link. Having the food hub hours duplicated inside the office tile means:

- **Students filtering for food hubs won’t see it** — this tile is categorised as Office, so when a student filters to Food Hub, this tile doesn’t appear. The food hub info crammed in here is invisible to the people actually looking for it.
- **The office tile is bigger than it needs to be** — students filtering for offices have to read past food hub info that has nothing to do with the office
- **The information can go out of date separately** — if food hub hours change, someone might update the Food Hub tile but forget to update the office tile (or vice versa), so the site shows conflicting information



### **What the office tile should look like**

> **TUSA Launceston Office**

> Opening hours: Monday to Friday, 9:00am to 5:00pm

> > **Mail**

> PO Box 4093, Invermay 7248

That’s it. Short, scannable, only office-relevant information.

---



## **What Content Goes on Each Tile**

### **Office tiles**


| Include | Don’t include |
| ------------------------------- | ----------------------------------- |
| Office name | Food hub hours or details |
| Campus and building/room | Hire store hours or details |
| Office opening hours | Mailing address from other services |
| Phone number (if applicable) | Equipment lists |
| Email (if applicable) | Volunteer info |
| Mailing address for that office | Details that belong on another tile |


### **Hire Store tiles**


| Include | Don’t include |
| -------------------------------------------------------- | ---------------------- |
| Store name | Office contact details |
| Campus and building | Food hub info |
| Pickup/return hours | Staff directories |
| Full equipment catalogue (the online store handles that) |  |


### **Food Hub tiles**


| Include | Don’t include |
| ------------------------------------- | ---------------------- |
| Hub name | Office contact details |
| Campus and building/room | Hire store info |
| Operating days and hours | Equipment lists |
| Brief description of what’s available |  |


**General rule for all tiles:** Keep it short. A tile should be scannable in a few seconds. If you’re writing more than 3-4 lines of content, you’re probably including information that belongs on a different tile.

---



## **How the Hire Store Connects to Locations**

Hire Store location tiles aren’t just informational — they are connected to the online hire system.

Every product in the hire store has a **pickup location** assigned to it (Sandy Bay, Launceston, Cradle Coast, or Rozelle). When a student rents equipment:

- The checkout shows which location they’ll pick up from
- If their cart has items from multiple locations (e.g. one item from Sandy Bay, another from Launceston), a warning appears

**What this means for you:**

- Don’t rename a Hire Store tile without checking with the dev team first — the name needs to match what’s in the product system
- The current hire store locations are **Sandy Bay** and **Launceston** (with Cradle Coast and Rozelle used in the product system too)
- If a new hire store location opens, the dev team will need to add it to the product system as well as creating the tile

---



## **The Sharing Link and Map**

### **Sharing link**

The **Sharing link** field holds a Google Maps link that students can use to get directions. To get one:

- Open Google Maps
- Search for or navigate to the location
- Click **Share**
- Copy the link
- Paste it into the Sharing link field



### **Street Address (map)**

The **Street Address** field is an interactive OpenStreetMap. When you edit it:

- Use the search box to find the address
- A marker will appear on the map
- You can drag the marker to fine-tune the position (e.g. to point at the specific building entrance)
- The marker label can be edited to show a custom name (e.g. “Social Sciences Building, UTAS Sandy Bay Campus”)

This map is what students see on the front end of the tile.

---



## **Current Locations Reference**

Here are all the TUSA Location tiles currently on the site, with their categories:

### **Offices**


| Title | Region | Address |
| ------------------- | -------------------------------------- | --------------------------------------------------- |
| Southern Tasmania | nipaluna/Hobart | Social Sciences Building, UTAS Sandy Bay Campus |
| Northern Tasmania | palanwina lurini kanamaluka/Launceston | Station “Railway” Cottage, Inveresk Campus |
| North West Tasmania | pataway/Burnie | Room 135, Floor 1, Field Building, West Park Campus |
| Rozelle, NSW | *(no region set)* | Building 101, Rozelle Campus |


### **Hire Stores**


| Title | Region | Address |
| --------------------- | -------------------------------------- | ------------------------------------------ |
| Sandy Bay Hire Store | nipaluna/Hobart | 1 Churchill Ave, Sandy Bay |
| Launceston Hire Store | palanwina lurini kanamaluka/Launceston | Station “Railway” Cottage, Inveresk Campus |


### **Food Hubs**


| Title | Region | Address |
| -------------------- | -------------------------------------- | --------------------------------------- |
| Sandy Bay Food Hub | nipaluna/Hobart | The Ref, TUSA Building, 1 Churchill Ave |
| Inveresk Food Hub | palanwina lurini kanamaluka/Launceston | Railway Cottage, Inveresk Campus |
| Hobart City Food Hub | nipaluna/Hobart | 42 Melville St, Hobart |


---



## **Common Mistakes**

### **Putting food hub or hire store details on an office tile**

This is the most common mistake. If you find yourself typing food hub hours or hire store information on an office tile, stop — that information has its own tile. Go find the Food Hub or Hire Store tile for that campus and put the information there instead.



### **Duplicating information across tiles**

If the same hours or address appear on two different tiles, one of them will eventually go out of date. Each piece of information should live on exactly one tile.



### **Leaving the Street Address map empty**

Every location needs the map field filled in. Without the map marker, the tile won’t show the interactive map and students can’t get visual directions. If you’ve filled in the Location address text field but not the Street Address map, the tile is incomplete.



### **Forgetting to set categories**

Every location needs both a **service type** (Office / Hire Store / Food Hub) and a **region** (nipaluna/Hobart / palanwina lurini kanamaluka/Launceston / pataway/Burnie). Without categories, the location won’t appear when students filter by type or region.

---

*If a student is looking for just one service, would they want to see all this other information? If no, it belongs on a different tile.*