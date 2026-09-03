---
name: process-re-review
description: Revisit a business process that has already been through the AI Decision Filter — check whether the decision still holds, whether the numbers came true, and what changed. Reads a saved decision worksheet, written decision, or process map, updates the diagram, and produces a revised one-page decision. Use when someone says a process has changed, their scheduled review date has come up, they want to check whether an AI or automation change actually worked, or they want to pick up an unfinished filter session where it left off.
license: MIT
---

# Process Re-Review

The follow-up to the AI Decision Filter. Something was decided about a process —
weeks or months ago, or halfway through a session that got interrupted. This picks
it back up without making anyone answer thirty questions again.

Two jobs, and you'll know which one from what they hand you:

- **Resume** — the filter didn't finish. Pick up at the phase it stopped at.
- **Review** — the filter finished and a decision was made. Check whether it held.

## The rule this skill exists to enforce

**A decision made once and never revisited becomes a liability nobody is watching.**
The reference files go stale, the volume changes, the person who owned it left, and
the honest answer today may be different from the honest answer in March. Changing
your mind here is the system working.

Same voice as the filter itself: one question at a time, plain language, no jargon,
no flattery, don't sell. If the honest answer is "turn it off," say it.

---

## Step 1 — Get the record

Ask for whatever they have. Any one of these is enough to start:

- the **decision worksheet** (`<process>-worksheet.md`)
- the **written decision** (the one-page summary)
- a **process map** HTML file
- nothing but a description — that's fine too, see below

If they can't find anything, ask them to paste whatever they do have, or describe
the process and what was decided. Don't refuse to start over a missing file.

**Read it back to them before anything else.** Two or three sentences: this is what
the process was, this is what was decided, this is the date. Ask: **"What did I get
wrong?"** People remember it differently, and their correction is data.

If it's an unfinished worksheet, say which phase it stopped at and what questions
were left open, then go to Step 5.

---

## Step 2 — What changed

Six questions, one at a time. Ask them plainly; don't read them as a list.

1. **Is the process still run the same way?** Any steps added, dropped, or moved?
2. **Is it the same people?** Especially — is the named owner still here, and still
   the owner?
3. **Has the volume changed?** More runs, fewer, or the same?
4. **Did you actually do the first step?** (Look it up in the record and name it.)
   If not — what stopped it? That answer matters more than the rest of this session.
5. **Has anything been bought, signed up for, or switched on since?**
6. **Anything now touch customer data, patient records, or money that didn't
   before?**

Any yes to 1, 2, 3, or 6 means the map is out of date and the decision may be too.

---

## Step 3 — Did the numbers come true?

Only if something was actually implemented. Skip it if the answer to question 4 was
no.

Pull the original figures out of the record and compare, out loud:

```
Predicted:  [hours saved per month]    Actual:  [hours saved per month]
Predicted:  [review time per month]    Actual:  [review time per month]
Predicted:  [cost per month]           Actual:  [cost per month]
Predicted:  [payback in months]        Actual:  [on track / behind / never]
```

Get the actual numbers the same way the filter got the originals — a number or a
range, never "it seems better." If nobody measured, say that plainly: the honest
answer is that the value is unknown, and the first step is to measure it for two
weeks.

Then the four review questions from the original plan:

- **Is it still saving time?**
- **Is the quality holding?** How many bad outputs in the last month, and did anyone
  notice them or did a customer?
- **Has the underlying process changed?**
- **Do the reference files still match reality?** Prices, policies, templates,
  staff names — when were they last updated?

**Being wrong in the original estimate is normal and worth saying so.** A 40%
capture that came in at 15% is useful information, not an embarrassment. Write down
which direction it missed and why; that's what makes the next estimate better.

---

## Step 4 — Update the map

Redraw the process map with whatever changed. Read `references/diagrams.md` from the
`ai-decision-filter` skill and follow the same rules — same shapes, same colors, same
sizing. If you can't reach that file, keep the new diagram in the same style as the
one they already have.

- Show it and ask **"What did I get wrong?"**, not "does this look right?"
- Mark what changed since the last version — an accent-colored `NEW` or `GONE` label
  beside the affected boxes is enough. Owners want to see the delta, not hunt for it.
- If the maintenance loop changed — new owner, new review schedule, new escalation
  path — redraw that too.
- Save both with the same names as before, so the newest version is the one they
  open. Keep the old ones if you can; a date suffix is fine.

If the process is small enough now that a table beats a diagram, say so and use a
table.

---

## Step 5 — Where does the decision land

One of five. Say which, in the first sentence, and then explain.

**Holding.** It's working, the numbers are close, the owner is in place. Confirm the
next review date and stop. This is a short session and that's fine.

**Adjust.** The tier is right but something around it isn't — reference files are
stale, review has quietly stopped, the owner changed, the boundaries need
tightening. Name the specific fix and who does it by when.

**Move up a tier.** They've genuinely outgrown it: the volume grew, or the
"somebody has to remember to do it" problem showed up. Say which tier and why now,
and re-run the money math with today's numbers before recommending it.

**Move down a tier, or stop.** Honest and underused. If the value didn't appear, if
nobody reviews the output, or if the person who owned it left and nobody replaced
them, say so and recommend turning it off. **This is a successful outcome.** The
off-switch condition was written down for exactly this moment — look it up and check
whether it's been met.

**Re-run the filter.** The process changed enough that the old decision doesn't
apply to the new process. Say so and hand it back to the `ai-decision-filter` skill,
starting from Phase 0. Don't try to patch a decision about a process that no longer
exists.

---

## The revised decision

Update the one-page summary. Keep the original visible for comparison — an owner
should be able to see what they thought last time.

```
PROCESS:        [name]
REVIEWED:       [today's date]      LAST DECIDED: [original date]
STATUS:         [holding / adjust / move up / move down / stop / re-run]

WAS:            [original tier and what was expected]
NOW:            [current tier and one sentence why it changed or held]

PREDICTED:      [hours saved, cost, payback]
ACTUAL:         [hours saved, cost, payback]   NUMBERS ARE: [measured / estimated]

WHAT CHANGED:   [process, people, volume, tools — one line each]
STILL OPEN:     [anything from the original that never got done, and why]

NEXT STEP:      [the single next action, this week]
OWNER:          [name — flag if this changed]
NEXT REVIEW:    [date]
STOP IF:        [the off-switch condition, restated or revised]

DIAGRAMS:       [updated process map] · [updated maintenance loop]
```

Save the updated worksheet alongside it, with the phase marked complete and today's
date, so the next review starts from this one.

If you can't save files, put the worksheet and the decision in the chat as code
blocks and tell them to keep both somewhere they'll find in three months.

---

## Guardrails

- **Do not defend the original recommendation.** It was made with the information
  available then. If it was wrong, say it was wrong, say what the evidence is, and
  move on. Nobody is being graded.
- **Do not accept "it's going great" as an answer.** Get a number, a count of bad
  outputs, or a date something was last checked.
- **The absence of measurement is a finding.** If nobody has been reviewing outputs
  since week two, that is the most important thing you'll learn today, and it goes
  at the top of the summary.
- **If the owner has left and nobody replaced them, that's a stop condition**, not a
  detail. Raise it first.
- **Don't build anything.** This skill re-decides and re-draws. It does not set up
  tools or write automations.
