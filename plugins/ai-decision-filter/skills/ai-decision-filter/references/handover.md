# Phase 8, the written decision, and the worksheet

What the owner walks away with, and what makes it survive the next six months.

---

# Phase 8 — Who owns it, and how do you know it still works

An unowned AI process becomes a liability on a timeline nobody is watching. Do not
end the session without this. **Get names, not roles.**

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

Then draw the maintenance and audit loop as the second diagram — see `diagrams.md`.

---

# The written decision

Show them the draft before you finalize it, the same way you showed the map: **"What
did I get wrong?"** Then hand over a one-page summary they can keep and show someone
else.

```
PROCESS:        [name]
DATE:           [date]
RUNS:           [x times per month, y hands-on minutes each]
NUMBERS ARE:    [measured / estimated — and by whom]

DECISION:       [Tier 0 / 1 / 2 / 2.5 / 3] — [one sentence why]
RUNS ON:        [any account requirement, e.g. business plan with a BAA]
CONSIDERED:     [the options you looked at and rejected, and why — one line each]
CONFIDENCE:     [high / medium / low] — [the one thing that would change it]

FIX FIRST:      [waste found in Phase 3, and what it's worth alone]
SIMPLER OPTION: [what boring automation covers, if anything]
ALREADY OWN:    [tool they've already bought — fits / needs setup / wrong fit]

TIME MATH:      [hours now] → [net hours saved] after [review hours]
WORTH:          [$ per month] against [setup cost + ongoing cost]
PAYBACK:        [months]

FIRST STEP:     [the single next action, this week]
OWNER:          [name]
REVIEW:         [how often, first review date]
NEVER:          [what it may not do unattended]
WATCH FOR:      [the most likely way this fails, from Phase 7]
STOP IF:        [the off-switch condition]

DIAGRAMS:       [process map file] · [maintenance loop file]
```

**`CONSIDERED:` is what makes this defensible.** A recommendation that only names
the winner reads like a sales pitch. Naming the cheaper options you rejected, and
why, is what lets them show this to a partner or an accountant.

Give them the two diagram files alongside it.

**Short version for an early exit.** If the session ended at Phase 0, 3, or 4, they
still get a decision — just a smaller one: PROCESS, DECISION (Tier 0 and why), FIX
FIRST, FIRST STEP, OWNER. Never end with a finding and nobody assigned to it.

---

# The worksheet

A session runs long. People leave for a phone call, close the tab, or come back next
week — often in a different app, with a different assistant. **Save the running
record as a file so none of that loses the work.**

Keep a plain markdown file, updated at the end of every phase, named
`<process-name>-worksheet.md`:

```
# [Process name] — decision worksheet
Started: [date]      Last updated: [date]      Phase reached: [n]

## The numbers
[runs per month, hands-on minutes, worst-case if wrong — each marked
 measured or estimated, with who said it]

## The process
[the steps, in order, with who does each and where the waiting is]

## What they said
[direct quotes worth keeping — especially about pain and about what
 they've already tried]

## Waste found (Phase 3)
## Boring automation checked (Phase 4)
## Score (Phase 5)
## Math (Phase 6)
## Open questions
[anything you asked and didn't get an answer to]

## Diagrams
[filenames]
```

**Resuming.** If someone starts a session by handing you a worksheet, do not rerun
the interview. Read it, tell them what phase it stopped at and what's still open,
confirm nothing has changed since, and pick up there.

**If you can't save files,** put the worksheet in the chat as a code block at the end
of each phase and tell them to copy it somewhere. Same content, same purpose.

Once a decision is delivered, the worksheet and the two diagrams are what the
`process-re-review` skill picks up later.
