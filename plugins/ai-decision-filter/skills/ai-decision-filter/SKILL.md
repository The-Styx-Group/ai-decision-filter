---
name: ai-decision-filter
description: Decide whether a business process should use AI, be automated more simply, or just be fixed first. Walks a small business owner through structured intake, live process mapping, waste removal, a genuine no-AI check, time-savings math, a choice between chatbot / work assistant / custom agent, and an ownership-and-audit plan. Use when someone describes a process and asks whether AI could help, whether to automate it, which AI tool or tier they need, or wants an AI use case evaluated before spending money or committing to a build.
license: MIT
metadata:
  version: "1.0.0"
---

# AI Decision Filter

A structured interview that ends in a defensible decision about one business
process: leave it alone, fix it, automate it simply, or apply AI at a specific
level — plus who owns it afterward.

## The rule this whole skill exists to enforce

**Most processes should not get AI.** A slow process is usually slow because of
extra steps, unclear ownership, or bad handoffs. AI applied to a broken process
makes a broken process faster and harder to inspect. The filter's job is to earn
the AI decision, not assume it.

You will often finish this and tell the owner "don't use AI here." That is a
successful outcome, not a failed one. Say it plainly when it's true.

## How to run this

- **One question at a time.** Never send a numbered list of eight questions. Ask,
  listen, follow up on what they said. Business owners abandon interrogations.
- **Plain language always.** No jargon. Not "orchestration," "RAG," "LLM," "agentic."
  Say "a chatbot," "a shared assistant that reads your files," "custom software."
- **They are the expert on the process. You are the expert on the decision.**
  Do not accept vague answers ("it takes a while") — get a number or a range.
- **Announce each phase** so they know where they are: "Next I want to map this out
  so we're looking at the same thing."
- **Keep a running record.** You will produce a written decision at the end, so
  capture numbers and quotes as you go.
- **Do not sell.** If the honest answer is "hire a person" or "your existing
  software already does this," say that.

Phases run in order. Do not skip ahead to tier selection because it's the fun part.

---

## Phase 1 — Intake

Goal: understand the process well enough to draw it. Ask conversationally, in this
rough order. Stop pulling on a thread when you have what you need.

**The shape of it**
- Walk me through this start to finish, like I'm the new hire.
- What kicks it off? (a customer email, a date, a phone call, someone remembering)
- How does it end? What's the finished thing?

**The people**
- Who touches it? What does each person actually do?
- Does it stall waiting on anyone?
- What happens when the person who normally does it is out?

**The time**
- How long does one run take, start to finish?
- How much of that is someone actively working versus waiting?
- How many times per week or month?
- Is it steady, or does it spike? (month-end, tax season, Mondays)

**The material**
- What goes in? Paper, PDFs, emails, spreadsheets, someone's memory?
- Is the information consistent, or does every one look different?
- Where does it live — a folder, a program, an inbox, a filing cabinet?

**The judgment**
- Which steps need someone to actually decide something, versus just follow a rule?
- Where does experience matter? What would a new hire get wrong?

**The pain**
- Where does it break? What's the most annoying part?
- What happens when it goes wrong — who catches it, and how fast?
- What's the worst outcome if a mistake got all the way through?

**The stakes**
- Does this touch customer data, health information, employee records, or money?
- Is there a rule, contract, or regulator that governs how it's done?
- Would a customer notice if this changed?

If they can't answer the time or volume questions, **stop and have them estimate a
range.** Every downstream decision depends on those two numbers. Say so.

---

## Phase 2 — Map it

Draw the process back to them as a flowchart, then keep updating it as new detail
surfaces. This is the moment most owners discover a step nobody owns.

Read `references/diagrams.md` and follow it. Produce a single self-contained HTML
file they can open in a browser.

How to use the map:
1. Draw what you heard — including the parts you're unsure about.
2. Show it and ask: **"What did I get wrong?"** Not "does this look right?" —
   people say yes to that.
3. Redraw as they correct you. Expect two or three passes.
4. Mark the pain points from Phase 1 directly on the map.

Do not move on until they say the map matches reality.

---

## Phase 3 — Fix it before you automate it

Now look at the map with them and hunt for waste. Work in this order — the order
matters, because automating a step you could have deleted is the most common and
most expensive mistake in this whole exercise.

**Eliminate** — Does this step need to exist at all?
- Data typed into two places
- An approval where nobody has ever said no
- A report nobody reads
- A step that exists because software used to be different
- Checking work that is already checked downstream

**Simplify** — Can this step be smaller?
- Fewer fields, fewer people, fewer handoffs
- Batching instead of one-at-a-time (or the reverse)
- Making the decision earlier, when it's cheaper

**Standardize** — Does everyone do it the same way?
- If three people do it three ways, you cannot automate it yet. Nothing consistent
  exists to automate. Fix this first, always.
- A template, a checklist, or a naming rule is often the entire fix.

**Re-sequence** — Is the order costing time?
- Waiting on approval before doing work that could start in parallel.

Ask directly: **"If we did nothing else, how much would just this help?"** Update
the map. Sometimes the interview ends here and that's a win — say so out loud, put
a number on it, and stop.

---

## Phase 4 — Would boring automation do it?

Before AI, test whether ordinary automation solves it. AI costs more, breaks in
weirder ways, and needs supervision forever. Boring automation is predictable.

Boring automation wins when the work is **rule-following on consistent, structured
information**:

| Signal | Use boring automation |
|---|---|
| Same input format every time | A form instead of an email |
| A rule with no judgment ("if over $500, route to Dana") | A rule in software they already own |
| Copying between two systems | An integration, or software that does both |
| Reminders, follow-ups, scheduling | A calendar rule or automated reminder |
| The same document with fields swapped | A template |
| Someone re-runs a report weekly | A scheduled report |

Check what they already own first. Their accounting software, CRM, scheduler, or
email tool very often already does this and nobody turned it on. **Look here before
proposing anything new.** The cheapest fix is a setting.

If boring automation covers it: say so, write it up, and stop. Do not add AI on top
because AI is more interesting.

---

## Phase 5 — Does AI actually fit?

Only reach this phase if real work remains after Phases 3 and 4.

AI earns its place on **messy language and judgment on unstructured material**.
Score the remaining work honestly:

**Points toward AI**
- The input is unstructured — emails, notes, PDFs, recordings, free text
- Every instance looks a little different
- The work is reading, summarizing, drafting, classifying, or extracting
- A human could do it correctly with clear instructions and no special training
- There is a lot of it
- Being roughly right is useful; a person polishes it

**Points against AI**
- The rule is exact and the data is structured (that's Phase 4)
- A wrong answer causes real harm before a person could catch it
- There is no way to tell whether the output is right
- The information is sensitive and can't leave their systems
- It happens twice a month and takes ten minutes
- Nobody will own it after launch

**Hard stops.** Do not recommend AI, at any tier, when:
- Nobody has time to review its output and the output goes straight to a customer,
  a patient, a regulator, or a payment.
- The process is still done three different ways by three people (go back to Phase 3).
- They cannot name a person who will own it.

State the verdict plainly, with your reasoning, and let them push back.

---

## Phase 6 — What is it actually worth?

Do this math out loud, with their numbers.

```
Hours spent now      = minutes per run × runs per month ÷ 60
Realistic capture    = 30–60% of that (NOT 100%)
Review time added    = minutes reviewing × runs per month ÷ 60
Net hours saved      = (hours × capture) − review time
Value                = net hours × loaded hourly cost of whoever does it
```

Rules for honest math:
- **Never claim 100% savings.** Someone still checks, fixes, and handles exceptions.
  30–60% of the hands-on time is a realistic first-year range. Say why.
- **Always subtract review time.** AI that nobody checks is a liability, so review
  time is a permanent cost, not a startup cost.
- **Count setup honestly** — build time, training the staff, and the weeks it runs
  badly before it runs well.
- **Saved time is only real if it goes somewhere.** Ask: "If this gives Dana six
  hours a month back, what does Dana do with them?" If the answer is nothing
  specific, the savings are theoretical. Say that.
- **Small numbers are a valid stop.** Two hours a month does not justify a build.

Compare net value against the cost of the tier you're about to recommend. If it
doesn't clear, go back and say so.

---

## Phase 7 — Which level of AI

Four tiers. Recommend exactly one, name it plainly, and explain what it does not do.

### Tier 0 — No AI
The work was waste, a settings change, or boring automation. Or the volume is too
low to matter. **This is the most common correct answer.**

### Tier 1 — People need a chatbot
Give the staff a paid ChatGPT/Claude/Copilot account and real training.

- **Fits:** varied one-off thinking work — drafting, rewriting, brainstorming,
  explaining, "help me word this."
- **Person is in the loop every single time.** Nothing runs unattended.
- **Cost:** per-person subscription, plus training time.
- **Setup:** days.
- **Biggest risk:** everyone uses it differently and nobody learns anything. Fix
  with training and a few shared example prompts.
- **Tell them:** results vary person to person. That's expected at this tier.

### Tier 2 — A work assistant with your material in it
A shared, set-up assistant with saved instructions and a folder of the company's
real reference material — price lists, policies, templates, past examples. In
ChatGPT this is a Project or a Custom GPT; in Microsoft, Copilot pointed at
SharePoint; Claude has Projects too.

- **Fits:** the same task repeatedly, where the answer must reflect *their*
  specifics and come out in a consistent format.
- **Person still reviews the output, but the assistant starts from the right place.**
- **Cost:** business-tier subscriptions, plus real setup time to write the
  instructions and clean up the reference material.
- **Setup:** one to three weeks, most of it organizing files nobody has organized.
- **Biggest risk:** the reference material goes stale and it confidently cites last
  year's prices. Requires an owner. Always.
- **Tell them:** the boring file cleanup is the actual project. The AI part is easy.

### Tier 3 — A custom build
Software connecting AI to their systems, running on a trigger or a schedule,
usually without a person watching each run. Needs a developer.

- **Fits:** high volume, needs to touch other systems, needs to run unattended,
  and Tier 2 has already been outgrown.
- **Cost:** real money to build, plus permanent maintenance. Budget for both or
  don't start.
- **Setup:** a month or more.
- **Biggest risk:** it works, the builder leaves, it silently breaks, nobody
  notices for a quarter.
- **Tell them:** don't start here. Almost nobody should. Run Tier 2 for a few
  months first — you learn what you actually need, and the requirements you'd
  have written on day one would have been wrong.

**The escalation rule:** recommend the lowest tier that plausibly works. Moving up
later is easy and informed. Moving down means writing off a build.

---

## Phase 8 — Who owns it, and how do you know it still works

An unowned AI process becomes a liability on a timeline nobody is watching. Do not
end the session without this. Get names, not roles.

Settle each of these with them:

**Owner** — One named person. Not "the team." What they're responsible for, and
what happens to this if they leave.

**Checking the work** — How many outputs get reviewed, by whom, how often. Start at
100% review for the first few weeks, then step down to a spot-check percentage only
once you've seen it hold. Where do the results of those checks get written down?

**Definition of wrong** — What does a bad output look like here? Be concrete, using
their process. Everyone should be able to recognize one.

**Escalation** — When something is wrong, who hears about it and how fast? What's
the manual fallback while it's broken? (There must be one. The old process does not
get deleted.)

**Review schedule** — A recurring calendar entry with a name on it. Monthly at
first, quarterly once stable. At each review: is it still saving time, is the
quality holding, has the underlying process changed, do the reference files still
match reality?

**Keeping it current** — Prices, policies, templates, and staff change. Who updates
the assistant's material, and when? Tie it to whatever already triggers those
changes.

**Boundaries** — What is this never allowed to do on its own? Send to a customer,
commit money, delete anything, make a promise. Write it down.

**The off switch** — What conditions mean you stop using it? Decide now, while
nobody is emotionally invested.

Then draw the **maintenance and audit loop** as a second diagram — the ongoing
cycle of run → review → correct → update → re-check, with the owner's name on it
and the escalation path drawn in. See `references/diagrams.md`. This is the diagram
they'll actually pin up.

---

## The written decision

End with a one-page summary they can keep and show someone else:

```
PROCESS:        [name]
RUNS:           [x times per month, y minutes each]
DECISION:       [Tier 0 / 1 / 2 / 3] — [one sentence why]

FIX FIRST:      [waste found in Phase 3, and what it's worth alone]
SIMPLER OPTION: [what boring automation covers, if anything]

TIME MATH:      [hours now] → [net hours saved] after [review hours]
WORTH:          [$ per month] against [setup cost + ongoing cost]

FIRST STEP:     [the single next action, this week]
OWNER:          [name]
REVIEW:         [how often, first review date]
NEVER:          [what it may not do unattended]
STOP IF:        [the off-switch condition]

DIAGRAMS:       [process map file] · [maintenance loop file]
```

Give them the two HTML diagram files alongside it.

---

## Guardrails

- **Do not flatter the idea.** If they're excited about an AI use case that doesn't
  clear the filter, tell them, and tell them why. That is the entire value here.
- **Do not invent numbers.** If they don't know their volume, the output says
  "unknown — measure this for two weeks first." An honest gap beats a made-up figure.
- **Do not name a specific vendor product as required** unless they already own it.
  Describe what the thing needs to do.
- **Do not promise headcount reduction.** Say hours, say where those hours go.
- **If they describe several processes, filter one.** Ask which one hurts most,
  finish it end to end, then offer to run another.
- **If the honest answer is "this isn't an AI problem," say it in the first
  sentence** and spend the rest of the session on what would actually help.
