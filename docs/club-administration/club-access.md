---
title: How Access Works
---
# **How access works: groups, roles, and who sees what**

Most “why can’t I see this?” or “can this person do X but not Y?” questions come down to one idea: on this site, **membership decides visibility, and roles decide what people can do.** Once that clicks, the rest of the access model follows from it. None of this is a bespoke choice; it’s how access control works in systems like this. What’s been tailored to TUSA is the setup built on top of it.

This builds on [Club Groups vs TUSA Groups](https://tusa-dev.its.utas.edu.au/docs/tusa-operations-guide/club-administration/how-access-works-groups-roles-and-who-sees-what/#club-groups-vs-tusa-groups). Read that first if you haven’t; it covers the two group types and how people get into them.

## **The core rule: you see a group only if you’re in it**

When you log in and go to your profile, you don’t see every group on the site. You see the groups **you belong to**, and nothing else. The clubs you’re not in, other teams, the staff areas: none of it shows for you.

That isn’t the site hiding things by accident. It’s how we control who sees what. Group membership *is* the permission. There’s no separate “who can see this” setting to keep in step: being in the group grants the view, and not being in it withholds it.

## **Why this is a feature, not a limitation**

Because visibility follows membership, the boundaries look after themselves:

- **TUSA Internal is staff-only.** All the behind-the-scenes work (affiliations, grants, incident reports, profile checks) lives inside the TUSA Internal group. Students and club admins never see any of it, because they’re not in that group.
- **Each club’s things stay with that club.** A club’s deals, resources and members sit inside its group, visible to that club’s members and no one else.
- **Put something in a group, and you’ve scoped it.** Where a thing lives decides who sees it.

So when something isn’t showing up, the first question is nearly always: **am I a member of the group it lives in?** If not, that’s usually the system working exactly as intended.

## **Access comes in whole containers**

There’s no “just their part” inside a group or a store. Whatever someone is given, they get all of it:

- **A group:** anyone in it sees everything in it: every post, member, document, and every risk assessment or event application lodged there.
- **A store:** anyone with access to a store has the whole store, every order and every customer’s details, not only the items they set up themselves.

So “can this person do this one thing” is really “am I happy for this person to see everything in that container.” Delegation is fine; it just isn’t free: someone can lodge a risk assessment on a team’s behalf, but only by being in that team’s group, and at that point they see all of it.

## **A group has only two levels: admin or member**

Within any group, there are exactly two levels. Admins run the group; members take part. There is no “member who sees less” and no half-membership, so you can’t give someone a partial view of a group by adjusting their level inside it. If they need a narrower view, that’s a group of their own, which is what an entity is.

## **Controlling what someone sees: that’s what entities are for**

Because membership is permission and a group is all-or-nothing, the way you give someone a specific, scoped view is by choosing which groups they belong to. If a team needs to see and run its own things without seeing everyone else’s, you give it its own group: its own entity. You don’t hand out one all-access pass and then try to hide parts of it. So whenever the question is “we want this person to do X but not see Y,” the answer is almost always their group or entity setup, not a per-person permission.

## **Build for the role, not the person**

The system deliberately grants and routes by **role**, not by naming individuals. A form’s approvals go to a role (say, Clubs Super Admin), not to a named person. This is on purpose: you don’t want a person built in as a lynchpin, because the day they move on, the thing they were holding together goes with them. Roles stay put as people come and go, so the setup survives the turnover that’s normal here. When you’re deciding access, the useful question is never “what should this person be able to do”, it’s “what does this role need”, so that whoever holds it next simply inherits it.

## **Seeing something is not the same as working on it**

Some things have two surfaces:

- A **view** is for visibility: an overview list showing what exists and its status. The Affiliations tab, for instance, lists every application and whether it’s pending or approved, by name.
- A **workflow inbox** is for action: it holds the full detail and the actual step to do (approve, assign), and only surfaces to the people who can act on it, whoever’s assigned or stands to be.

So you might see that something exists in a view while the working detail, and the ability to act on it, live only in the right person’s inbox.

Work is assigned to a **role**, not a named person, so an item usually shows in the inbox of everyone who holds that role, and whoever is free can pick it up. On some forms a person can then claim it as their own, at which point it drops off everyone else’s inbox; on others it stays visible to the whole role until it’s actioned. Which of those happens depends on the form. Either way it lands on the role first, so the work never depends on one named person being in that day.

One practical note: the workflow inbox lists items by form name, date and id, not by the club or entity name. To find a specific one, take its date from the view and match it in your inbox.

## **Adding yourself to a group is not the same as full membership**

As a clubs super admin, if you can’t see a group you need, you can add yourself to it. For TUSA groups (Food Hub, TUSA Internal, and the like) that manual add is the right method: they’re run without automation on purpose, so people are added by hand. Club groups work differently: adding yourself gets you into the group, but it does not give you the club membership tags a real member gets when they buy a membership. Those tags are what make someone a full club member.

## **The short version**

- You see a group only if you’re a **member** of it. Membership is the permission.
- Access is **whole-container**: in a group or store you get all of it, not a corner.
- A group has only **two levels, admin or member**. No “member who sees less”.
- To give someone a scoped view, give them their own group: an **entity**. Not a per-person setting.
- **Build for the role, not the person**, so the setup survives people coming and going.
- **Views show, inboxes act.** You can see that something exists, but you only get the detail and the ability to act if it’s assigned to you.

