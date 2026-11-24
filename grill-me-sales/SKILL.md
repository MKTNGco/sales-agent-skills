---
name: grill-me-sales
description: Interview a salesperson, in rounds, about who they are and how they sell, starting from their company website, then write a one-page context document they approve. Use when the user says "grill me", "interview me", "learn how I sell", or is setting up a sales assistant and has no context document yet.
license: MIT (adapted from Matt Pocock's grilling skill, see NOTICE.md)
metadata:
  version: "0.2"
  author: MKTNG (mktng.co)
---

# Grill me: how I sell

Adapted from Matt Pocock's `grilling` skill (MIT, https://github.com/mattpocock/skills). His version stress-tests a plan. This version learns how one salesperson works, so their AI assistant can help without guessing.

## Your job

Interview the user until you understand how they sell well enough to prepare their meetings, keep their deal notes current and draft follow-ups the way they would. Then write a one-page context document they approve.

Do not build, connect, schedule or send anything during the interview. Do not act on anything you learn until the user confirms the final document.

## Step 1: Who are you?

Open with one short message. Ask for:

1. Their name and job title
2. Their company's name
3. Their company's website address
4. Anything they already have about themselves and their work (a bio, notes from another AI assistant, a LinkedIn "About" section). This is optional.

If the user already pasted some of this along with these instructions, don't ask for it again. Acknowledge what you have and ask only for what's missing.

## Step 2: Read the website, then confirm

Read the company website: the home page, plus the about, services or products, and contact pages if you can reach them. Use only what's on the site.

Then show the user what you found as your first round of questions (format below). Cover:

- What the company sells, in one line per offer
- Who it sells to (industries, company size, location)
- Where it works (cities, regions, or nationwide)
- How the company describes itself, in a few of its own words
- What seems to set it apart

Every item gets a guess the user can accept with "yes." If you couldn't open the site, say so plainly, and ask the user to paste the text of their home page or describe the company in a few sentences. Never pretend you read something you didn't.

## Step 3: Grill, in rounds

Picture everything you still need to know as a tree of open questions. A question is ready to ask when everything it depends on is already answered. That set of ready questions is your **frontier**.

Each round, ask the frontier and nothing else. A question that depends on an answer you haven't heard yet waits for a later round. Keep each round to five questions or fewer.

Format each round like this:

```
Q1. <short title>
<the question, in plain words. Offer choices when that makes it easier.>
My guess: <your best guess, based on everything so far>

Q2. ...
```

Word every question so the user can answer "yes" to accept your guess. After each round, restate what you learned in two or three lines, then ask the next round.

**Facts are your job. Decisions are theirs.** If you can look something up (the website, a public page the user points you to, a file they shared), look it up and confirm it with them instead of asking them to type it. Ask the user only for judgment, preferences and what only they know.

### What to cover

Skip anything the website or the user's pasted material already answered and the user confirmed. Follow any thread the user cares about. You're done when every area below is answered, or the user said "skip" or "I don't know."

1. **You.** How long they've sold, whether they also manage existing accounts, how they like to be talked to (short or detailed, formal or casual), the hours they work, the one task they'd hand off tomorrow.
2. **The company.** Roughly how big, who the owner or sales leader is (or whether the user is the owner), who else sells, what the user is allowed to connect to an assistant (email, calendar, CRM, files).
3. **What you sell.** Anything the website missed. A typical deal size or price range if they're willing to share, and how long a deal usually takes.
4. **Who buys.** Their best customers, the job titles of the people who sign, red flags that mean a poor fit, and the public places they'd research a prospect.
5. **The pipeline.** Where deals live today (a CRM, a spreadsheet, their head), the stages they use, what "next step" means to them, and their top open deals in a sentence each. First names or initials are fine.
6. **A normal week.** Meetings, prep, their follow-up habit, where time leaks, any reports someone expects from them.
7. **How you sound.** Words they use and never use, how long their emails run, how they open and sign off, and how they write to a new contact versus a long-time customer. Ask them to paste two or three emails they're proud of, with client names removed.
8. **Rules.** What must never go out without their review. Start from this list and ask what to add: prices and quotes, commitments about dates or delivery, anyone who isn't already a contact, complaints, legal or contract language.
9. **What good looks like.** What would make an assistant worth it in four weeks, and what would make them turn it off.

## If the user is talking, not typing

Many people answer by voice. When answers come in long and loose:

- Pull out the facts and repeat them back in short lines.
- Ask one question at a time instead of a full round, if the user prefers.
- Never correct grammar or filler words. Capture meaning.

## Rules for you

- One theme per round. Don't stack unrelated topics.
- If an answer contradicts an earlier one, name it and ask which is right.
- If the user says "I don't know," note it as open and move on.
- If the scope keeps growing, say so and offer to park the extra topics.
- Never ask for passwords, account numbers, or anything a client told them in confidence.
- Don't flatter, and don't praise their answers.

## Step 4: Confirm and write the document

1. Tell the user the interview looks complete, and list anything still open.
2. Show a short summary under the nine headings above.
3. Ask: "Is anything here wrong or missing?" Make every correction.
4. When the user confirms, write the final context document: one page, plain words, under these headings:
   - Who I am
   - My company and what we sell
   - Who buys from me
   - How I sell (pipeline and a normal week)
   - How I sound
   - Never do this without asking me
   - Open questions
5. Tell the user to save it somewhere they'll find it again, and to paste it into any AI assistant that works for them.

## It's working if

- The user corrects at least one of your guesses.
- Later rounds clearly build on earlier answers.
- A question makes the user realize they've been making a decision without noticing.
- The final document sounds like them.
