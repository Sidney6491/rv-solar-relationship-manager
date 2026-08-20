# Relationship Manager

A one-page app that tells me who needs me today, in a sentence I don't have to decode.

I spent my working years as a water operator. The job was never about knowing everything — it was about the system telling you what needed attention before it turned into a problem. Most contact managers don't do that. They store people and wait for you to remember. This one does the remembering.

Live: https://sidney6491.github.io/rv-solar-relationship-manager/

---

## What it actually does

It writes sentences, not rows.

> Renogy still hasn't come back to you about the 9% kit rate after Sept 30. You asked 3 weeks ago.

> You haven't spoken to Ray Nolan in 4 months. Worth giving Ray a call.

> Danielle's birthday is in 15 days. Time to get a card made and sent.

Four things push a person to the top of the page: a follow-up that's due, a birthday inside 30 days, an anniversary inside 21 days, and drift — nobody asked for anything, it's just been too long. Everything else stays in the rolodex until it matters.

Personal and business sit in separate zones on purpose. Business noise piles up fast and it would bury "you haven't called your sister," which is the stuff with no deadline forcing it.

## First run

Open the link and sign in. The page is empty, which is correct — it starts with nobody in it.

Hit **+ Add** and put someone in. First name is the only thing it really needs. The field marked *What's outstanding?* is the one worth getting right — write a fragment, not a heading. Type `the 9% kit rate` and the card reads properly. Type `Rates` and you get a card that says nothing.

Set a channel — call, text, or email — and the buttons and links follow it.

## Day to day

A person shows up in a zone when they need you. Do the thing, then tick it off, and the app logs the date, the channel, and what it was about on that person's record. If you're not doing it today, hit **Not today** and they go quiet for three days. That button exists because the alternative was lying to the app or staring at a wall of guilt, and an app that makes you feel bad stops getting opened.

## Back it up

The contacts live in your browser on your machine. Not on a server, not in the repo, not anywhere I can reach. That's deliberate — a public repo with people's names and birthdays in it is a problem waiting to happen.

The tradeoff is that clearing your browser data wipes the lot.

So: **⚙ → Download a backup** gives you a JSON file. **⚙ → Restore from a backup** reads it back — it tells you how many contacts are coming in and how many it's about to replace before it does anything. There's a line at the bottom of the page that goes amber when it's been more than 30 days.

Back it up before you change computers. That one's from experience.

## Updating it

One file. `index.html`. Replace it in the repo and GitHub Pages picks it up in a minute or two.

Your contacts survive that, because they were never in the file.

## What it doesn't do

The email button opens a pre-filled draft. It doesn't send — sending needs a server, and this doesn't have one.

Nothing runs while the page is closed. No daily email, no notifications. It works when you open it, which means it only works if you open it. That's the honest weak spot and I know it.

There's no sync. One browser, one machine.

---

Built for RV Solar Hub — affiliate managers, brand contacts, backlink people, and the ones I'd feel bad about forgetting.
