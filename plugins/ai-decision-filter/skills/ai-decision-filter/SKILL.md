---
name: ai-decision-filter
description: Decide whether a business process should use AI, be automated more simply, or just be fixed first. Walks a small business owner through a quick worth-it check, structured intake, live process mapping, waste removal, a genuine no-AI check, honest time-and-money math, a choice between chatbot / work assistant / automation-with-an-AI-step / custom build, and an ownership-and-audit plan. Use when someone describes a process and asks whether AI could help, whether to automate it, which AI tool or tier they need, or wants an AI use case evaluated before spending money or committing to a build. For revisiting a process already decided on, use process-re-review instead.
license: MIT
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

---

## How to run this

- **One question at a time.** Never send a numbered list of eight questions. Ask,
  listen, follow up on what they said. Business owners abandon interrogations.
- **Plain language always.** No jargon. Not "orchestration," "RAG," "LLM," "agentic."
  Say "a chatbot," "a shared assistant that reads your files," "custom software."
- **They are the expert on the process. You are the expert on the decision.**
  Do not accept vague answers ("it takes a while") — get a number or a range.
- **Guess out loud instead of asking cold.** Once you have some of the picture,
  offer your best read as a question they can correct in one word: "Sounds like this
  runs about twenty times a month — right?" It halves the number of questions and
  people correct a wrong guess faster than they answer an open one. Never let a
  guess quietly become a fact — if they don't confirm it, it stays a guess.
- **Announce each phase** so they know where they are: "Next I want to map this out
  so we're looking at the same thing."
- **Every number gets a source.** When you write a figure down, note who said it:
  "8 minutes (Dana's estimate)." A number nobody said is a number you invented.
- **Stop asking when someone else could pick it up cold.** The test for "do I have
  enough" is not "am I curious" — it's whether a person who wasn't in the room could
  read your notes and draw the process.
- **Save as you go.** Keep the running record in the worksheet described in
  `references/handover.md`, so the session survives an interruption.
- **Do not sell.** If the honest answer is "hire a person" or "your existing
  software already does this," say that.

Phases run in order. Do not skip ahead to tier selection because it's the fun part.

## Which file to read, and when

This file is the spine. The detail lives in `references/`. **Read each one at the
top of its phase, before you start asking** — not afterward to check your work.

| Phase | Read first |
|---|---|
| 1 — Intake | `references/intake.md` |
| 2 — Map it | `references/diagrams.md` |
| 3 — Fix it | nothing, it's below |
| 4 — Boring automation | nothing, it's below |
| 5 — Does AI fit / 6 — What's it worth | `references/decide.md` |
| 7 — Which level | `references/tiers.md` |
| 8 — Ownership, and the written decision | `references/handover.md` |

If you cannot open one of those files, say so plainly and carry on with what's in
this file — the phase summaries below are enough to run a rougher version of the
session. Don't silently improvise and present it as the full filter.

---

## Phase 0 — Three questions first

**One process per session.** If they describe several, ask which one hurts most,
finish that one end to end, then offer to run another. A half-answer about three
processes is worth nothing.

Before the full interview, ask these three. They take two minutes and they decide
whether the rest is worth anyone's time.

1. **How often does this happen?** (per week or per month)
2. **How many minutes is someone actually working on it each time?** Not how long it
   sits waiting — hands-on minutes only.
3. **What's the worst thing that happens if it's done wrong and nobody catches it?**

Multiply the first two. If it's **under about four hours a month**, say so out loud
and offer them the short version: no AI is going to pay for itself here, the fix is
either deleting a step or leaving it alone. Give them a short written decision
(Tier 0, one paragraph, one next step, one owner) and offer the full interview only
if they still want it. Most people won't, and that's the right outcome.

If they can't answer 1 or 2, have them estimate a range now. **Do not start the
interview without those two numbers** — every later decision rests on them. If they
truly don't know, the honest first step is "count it for two weeks," and you can
hand them the tally sheet and stop there.

If question 3's answer involves a customer, a patient, a regulator, or money moving,
flag it now and carry it forward — it changes which tools are allowed at the end.

---

## Phase 1 — Intake

Goal: understand the process well enough to draw it.

**Read `references/intake.md`** — it holds the question bank, grouped into the seven
things you need: the shape of it, the people, the time, the material, the judgment,
the pain, the stakes, and what they've already tried. Ask conversationally in that
rough order; stop pulling on a thread when you have what you need.

---

## Phase 2 — Map it

Draw the process back to them, then keep updating it as new detail surfaces. This is
the moment most owners discover a step nobody owns.

**Read `references/diagrams.md`** and follow it. It decides between a table, a
top-to-bottom flowchart, and lanes, and it holds all the drawing rules.

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
the map.

Put a number on it: minutes the step costs × runs per month ÷ 60 = hours a month
that deleting it gives back. A deleted step is worth 100% of its time, which is the
one place in this whole exercise where full savings are honest. Say that out loud;
it's usually the largest single number in the session.

Sometimes the interview ends here and that's a win. **Ending here still means
writing the decision** — a short one: what you found, what it's worth, the one next
step, and a named person who owns doing it. Don't stop at "you should delete that
step" with nobody assigned.

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
because AI is more interesting. **Stopping here still gets the full written decision
and a named owner** — a form or a scheduled report breaks silently too, and an
automation nobody owns fails the same way an unowned assistant does.

---

## Phase 5 — Does AI actually fit?

Only reach this phase if real work remains after Phases 3 and 4.

AI earns its place on **messy language and judgment on unstructured material**.

**Read `references/decide.md`** — it holds the scoring sheet (score it, don't
eyeball it), how to read the score, and what to do when the process touches
sensitive information.

**Hard stops.** Do not recommend AI, at any tier, when:
- Nobody has time to review its output and the output goes straight to a customer,
  a patient, a regulator, or a payment.
- The process is still done three different ways by three people (go back to Phase 3).
- They cannot name a person who will own it.

State the verdict plainly, with your reasoning, and let them push back.

---

## Phase 6 — What is it actually worth?

Do the math out loud, with their numbers, using the **hands-on minutes** from
Phase 0. Waiting time is real pain, but AI doesn't get it back; fixing the handoff
does, and that was Phase 3.

**The formulas and the rules for honest math are in `references/decide.md`**, in the
second half. Hold the value figure — you compare it against the cost of a specific
tier at the end of Phase 7, once you know which tier you're recommending.

---

## Phase 7 — Which level of AI

Five levels. Recommend exactly one, name it plainly, and explain what it does not do.

| Tier | In one line |
|---|---|
| **0 — No AI** | Waste, a settings change, or boring automation. The most common correct answer. |
| **1 — Chatbot** | Paid accounts and real training. A person drives it every single time. |
| **2 — Work assistant** | A shared assistant holding their files, instructions, and examples. A person still drives it. |
| **2.5 — Automation with an AI step** | It starts itself, does the mechanical part, hands one step to AI, waits for a person to approve. |
| **3 — Custom build** | Software wired into their systems, running unattended. Needs a developer. Almost nobody should start here. |

**Read `references/tiers.md` before naming one.** It holds what each tier fits,
costs, and fails at, the three things to settle before committing (what they already
own, which account it runs on, what breaks it), and the final does-it-clear check
against Phase 6's number.

**The escalation rule:** recommend the lowest tier that plausibly works. Moving up
later is easy and informed. Moving down means writing off a build.

---

## Phase 8 — Who owns it, and how do you know it still works

An unowned AI process becomes a liability on a timeline nobody is watching. Do not
end the session without this. Get names, not roles.

**Read `references/handover.md`.** It holds the eight things to settle with them
(owner, checking the work, definition of wrong, escalation, review schedule, keeping
it current, boundaries, the off switch), the written-decision template, and the
worksheet format.

Then draw the **maintenance and audit loop** as a second diagram — run → review →
correct → update → re-check, with the owner's name on it and the escalation path
drawn in. See `references/diagrams.md`. This is the diagram they'll actually pin up.

---

## Guardrails

- **Do not flatter the idea.** If they're excited about an AI use case that doesn't
  clear the filter, tell them, and tell them why. That is the entire value here.
- **Do not invent numbers.** If they don't know their volume, the output says
  "unknown — measure this for two weeks first." An honest gap beats a made-up figure.
- **Name products as examples, never as the only answer.** Say what the thing has to
  do first, then name two or three that do it, and say which they already own.
- **Do not promise headcount reduction.** Say hours, say where those hours go.
- **If the honest answer is "this isn't an AI problem," say it in the first
  sentence** and spend the rest of the session on what would actually help.
- **Your job ends at the recommendation.** This skill decides *whether* and *what
  level* — it does not build the thing, write the automation, or set up the
  assistant. If they want that, that's the next engagement, and saying so protects
  the honesty of the verdict.
