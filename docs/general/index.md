# Reporting an Issue
When something on the TUSA site isn’t working the way you expect, don’t try to debug it yourself — send Sarah the five things below and she’ll take it from there.

This applies to anything on the site: a page that’s blank, a button that does nothing, a form that won’t submit, an email that didn’t arrive, a club that won’t save, an order that didn’t show up, a member who can’t log in.

# What to send
Reply with these five things — a screenshot covers most of them in one go:

#### What were you doing?
e.g. “I was setting up a new deal for Hobart Surf Club.”

#### What did you see?
e.g. “The page loaded blank — just the header and footer, nothing in the middle.”

#### What did you expect to see?
e.g. “I was expecting a form like the one I use for adding products.”

#### Where were you?
The page address (URL) at the top of the browser, or the menu path you took.
e.g. “tusa.com.au/clubs/hobart-surf-club/manage/deals/add-new”

#### A screenshot, please.
– Windows: press Windows key + Shift + S, drag a box around the page, then paste into your message (Ctrl+V).
– Mac: press Cmd + Shift + 4, drag a box, then drag the screenshot file into your message.
– Phone: use your usual screenshot shortcut and attach the image.

Capture the whole browser window if you can — the address bar and any error messages need to be visible too.

That’s it. Send it through and Sarah will diagnose.

Please don’t try to fix it yourself
Even if you think you know what’s wrong — please leave the diagnosis and the fix to your web person.

Issues can surface for entirely different reasons to what you’re seeing. A blank page might not be a “blank page problem.” A missing button might not be a “missing button problem.” The cause is often something connected behind the scenes — a permission rule, a recent change to a related system, an automated process running in the background, or a plugin that interacts with three other things. What looks like the obvious cause is usually a symptom, not the source.

When you act on what appears to be wrong:

The real fault keeps doing damage elsewhere, hidden behind your “fix”
Working automation can break because it depended on the thing you changed
The original error state is gone — which means the web person has to diagnose from a baseline that no longer reflects the actual problem
Changes you make affect every user of the site, not just you
So even if you feel confident about the cause: stop, send the five things above, and wait for a reply.

If something is genuinely time-sensitive (the site is down, money is involved), say so in your message — see When it’s urgent at the bottom of this page.

What NOT to do
You may have seen technical instructions floating around about editing config files, turning on “debug logging,” or installing diagnostic plugins. Those are developer-only tasks. Please don’t try them.

Specifically, please don’t:

Edit wp-config.php — this file holds the site’s security keys and database credentials. Editing it incorrectly can take the entire site offline or expose sensitive data.
Open or read debug.log — debug logging is already on; Sarah checks it. The file isn’t meant for human reading.
Install, activate, or deactivate plugins to “test” something — even a quick toggle can break automation that runs in the background.
Edit code snippets in WPCode — these are part of the site’s automation and changing one can cascade.
Use FTP/SFTP to look at site files.
If a guide somewhere asks you to do any of the above and you’re not sure, send Sarah the five things instead — that’s always the right move.

Common situations
“The page is blank”
Refresh once (Ctrl+R / Cmd+R) — sometimes it’s a momentary load issue.
If it’s still blank: send the five things. Don’t clear caches, don’t disable plugins.
“I got an error message”
Take a screenshot of the whole error, including any red banner, popup, or text on the page.
Send the five things plus the screenshot.
“It worked yesterday and doesn’t today”
Note what’s different if anything — different browser, different device, different login, new release.
Send the five things and mention “this worked [when].”
“Email didn’t arrive”
Check your spam/junk folder first.
If not there: send the five things plus which email address you were expecting it at and roughly when it should have arrived.
“I followed the instructions but got stuck at step X”
Tell Sarah which guide and which step. e.g. “Setting up Club Stripe, step 3 — the button isn’t there.”
Send the five things and a screenshot of where you got stuck.
Feedback on the guides
The guides are written by one person and the only way they improve is when you flag what tripped you up. Please send that feedback — but be specific, because “the instructions are confusing” doesn’t tell Sarah which paragraph to rewrite.

Useful feedback names the specific point of failure:

Which guide. e.g. “Managing TUSA Locations.”
Which step or section. e.g. “The Sharing Link bit.”
What you tried. e.g. “I opened Google Maps and searched for the address but couldn’t find a Share button.”
What you expected to happen. e.g. “I thought I’d be filling something in on the location edit screen itself.”
That kind of feedback gets a fix in the next version of the doc — often the same day.

Vague feedback like “steps are missing” or “it was too complicated” reads as honest frustration, but Sarah can’t act on it. She doesn’t know which step felt missing, so she can’t add it. If a guide isn’t working for you, take 30 seconds to note the specific point you got stuck and send that.

If a message comes back as “this is all too hard” or “I don’t understand,” Sarah will keep coming back to you with the same questions — which guide, which step, what you tried, what you expected — until there’s enough to act on. She isn’t trying to be difficult, and she isn’t ignoring you. She just genuinely can’t do anything for you without it.

A half-finished attempt is fine to send too. “I made it to step 4 and then I wasn’t sure what to click” is more useful than no message at all — that clears the bar.

When it’s urgent
If the site is down for everyone (not just you) or money is involved (a payment failed, an order is wrong, refunds), flag that explicitly in your message — start with “URGENT — site down” or “URGENT — payment issue” so Sarah sees it first.

For everything else, a normal message is fine. Sarah will reply once she’s diagnosed.

