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
- **Save as you go.** Keep the running record in the worksheet (see *The worksheet*
  below) so the session survives an interruption.
- **Do not sell.** If the honest answer is "hire a person" or "your existing
  software already does this," say that.

Phases run in order. Do not skip ahead to tier selection because it's the fun part.

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

**The time** (you have the two headline numbers from Phase 0 — fill in around them)
- How long does one run take, start to finish, including the waiting?
- Where does the waiting happen, and what is it waiting on?
- Is the volume steady, or does it spike? (month-end, tax season, Mondays)

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

**What they've already tried**
- Have you already bought, signed up for, or tried something for this?
- What happened? Where did it stop being useful?

Ask this before you form a verdict, not after. If they've already bought a tool,
that money is spent either way — it does not earn the tool a passing grade, and it
does not disqualify it. You'll come back to it in Phase 7 and say plainly whether
what they own fits the tier they actually need, and what it would take to make it
fit. Finding this out at the end, after you've recommended something else, wastes
the session.

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
the map.

Put a number on it the same way Phase 6 does — minutes the step costs × runs per
month ÷ 60 = hours a month that deleting it gives back. A deleted step is worth
100% of its time, which is the one place in this whole exercise where full savings
are honest. Say that out loud; it's usually the largest single number in the
session.

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
Score it, don't eyeball it. Give each line **0, 1, or 2** and show them the sheet —
a verdict they can see the arithmetic behind is a verdict they can argue with, which
is the point.

**Points toward AI** (0 = no, 1 = partly, 2 = strongly)

| | Score |
|---|---|
| The input is messy — emails, notes, PDFs, recordings, free text | |
| Every instance looks a little different | |
| The work is reading, summarizing, drafting, sorting, or pulling facts out | |
| A capable person could do it right from written instructions, no special training | |
| There is a lot of it | |
| Roughly right is useful — a person polishes it | |
| **Toward total (0–12)** | |

**Points against AI** (0 = not true, 1 = somewhat, 2 = very true)

| | Score |
|---|---|
| The rule is exact and the information is already tidy (that's Phase 4) | |
| A wrong answer causes real harm before a person could catch it | |
| There is no practical way to tell whether the output is right | |
| It's low volume — a few times a month, a few minutes each | |
| Nobody has been named to own it after launch | |
| The people doing it don't want it and won't use it | |
| **Against total (0–12)** | |

**Reading the score:**
- **Toward 8+ and Against 4 or less** → AI fits. Continue to the tiers.
- **Toward 5–7, or Against 5–7** → borderline. Say "borderline" out loud, name the
  one thing that would tip it, and recommend the smallest possible trial rather than
  a build.
- **Toward 4 or less, or Against 8+** → no AI. Say so and explain which lines drove
  it.

Any single **Against** line scored a 2 is worth stopping on by itself. Talk about it
before you total anything.

**Hard stops.** Do not recommend AI, at any tier, when:
- Nobody has time to review its output and the output goes straight to a customer,
  a patient, a regulator, or a payment.
- The process is still done three different ways by three people (go back to Phase 3).
- They cannot name a person who will own it.

### Sensitive information changes the tool, not the answer

If the process touches patient records, customer financial details, employee files,
or payment data, that is **not a reason to refuse.** It's a reason to be specific
about where the work is allowed to happen. Never say "you can't use AI for this."
Say which kind of tool it has to be.

The rule: **the information may only go into a tool that has signed a contract
promising to protect it.** In practice that means:

- **Health or patient information** — a business or enterprise plan with a signed
  BAA (a Business Associate Agreement — the contract a vendor signs promising to
  handle patient data under health-privacy law). The major AI vendors offer this on
  their business tiers. A personal account does not have one, no matter how much it
  costs.
- **Customer financial, payment, or personal records** — a business or enterprise
  plan with a signed data-processing agreement, and the vendor's SOC 2 report on
  file. SOC 2 is an independent audit of how a vendor guards data; ask for it and
  they will send it.
- **Either way, training must be switched off** on the account, so their material
  isn't used to improve the vendor's model. This is a setting on business plans and
  often not available on personal ones.
- **A short written "never paste this" list** for staff, in their words, naming the
  specific fields that stay out — social security numbers, full card numbers,
  whatever applies here.

Carry this into Phase 7 as a constraint on the tier: **the tier is unchanged, the
account it runs on is not.** A clinic that lands on Tier 1 gets Tier 1 on a business
plan with a BAA, not Tier 0. If they will not pay for the business plan, then say
plainly that the answer is no AI for this particular process until they do — and
that a different, non-sensitive process might be a better first project.

State the verdict plainly, with your reasoning, and let them push back.

---

## Phase 6 — What is it actually worth?

Do this math out loud, with their numbers. Use the **hands-on minutes** from
Phase 0 — the time someone is actually working, not the time it sits in an inbox.
Waiting time is real pain, but AI doesn't get it back; fixing the handoff does, and
that was Phase 3.

```
Hours spent now   = hands-on minutes per run × runs per month ÷ 60
Realistic capture = 30–60% of that if AI does it   (NOT 100%)
                    up to 100% if the step is DELETED (Phase 3)
                    70–90% if boring automation does it (Phase 4)
Review time added = minutes reviewing × runs per month ÷ 60
Net hours saved   = (hours × capture) − review time
Value per month   = net hours × loaded hourly cost of whoever does it
Payback in months = one-time setup cost ÷ value per month
```

**Loaded hourly cost** means what the person really costs per hour — their wage plus
payroll taxes and benefits. Rule of thumb: wage × 1.3. Use the wage of whoever
actually does the work, not the owner's.

Rules for honest math:
- **Never claim 100% savings from AI.** Someone still checks, fixes, and handles the
  odd ones. 30–60% of the hands-on time is the realistic first-year range because
  the exceptions — the weird invoice, the angry customer, the one that doesn't fit
  the pattern — stay human, and they are a bigger share of the work than anyone
  expects. Say that, in those words.
- **Always subtract review time.** AI that nobody checks is a liability, so review
  time is a permanent cost, not a startup cost.
- **Count setup honestly** — build time, training the staff, cleaning up the files,
  and the weeks it runs badly before it runs well.
- **Give them payback in months.** It's the only number most owners feel
  immediately. "Nine hours a month back, pays for itself in four months" lands where
  a percentage does not.
- **Saved time is only real if it goes somewhere.** Ask: "If this gives Dana six
  hours a month back, what does Dana do with them?" If the answer is nothing
  specific, the savings are theoretical. Say that.
- **Small numbers are a valid stop.** Two hours a month does not justify a build.
- **Mark every figure as measured or estimated.** An estimate isn't a problem; an
  estimate presented as a measurement is. If the whole case rests on estimates, say
  the first step is to count it for two weeks.

Hold the value figure. You'll compare it against the cost of a specific tier at the
end of Phase 7, once you know which tier you're recommending.

---

## Phase 7 — Which level of AI

Five levels. Recommend exactly one, name it plainly, and explain what it does not do.

**Before you name a tier, show them what each one looks like *in their process*.**
People cannot picture "a work assistant." They can instantly react to a sentence
about their own job. Write three or four one-liners using their real names and their
real steps, and ask which one they were imagining:

> - Dana opens a chatbot, pastes the email in, and fixes up the draft it gives back.
> - Dana opens a shared assistant that already has your price list and your last
>   fifty quotes in it. It drafts the quote in your format. Dana checks it and sends.
> - The quote drafts itself when the email arrives and waits in a queue. Dana
>   approves or edits it, then it sends.
> - It runs on its own overnight. Dana reads a summary of what it did in the morning.

This takes thirty seconds and it surfaces the gap between what they've been
picturing and what they can afford, before you deliver a verdict they'll resist.

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

### Tier 2.5 — An automation tool with one AI step and an approval step
An off-the-shelf automation tool — Zapier, Make, n8n, Power Automate, or whatever
their existing software already connects to — wired so the process starts itself. It
picks up the trigger, does the mechanical moving of information, hands the one messy
part to AI, and then **stops and waits for a person to approve** before anything
leaves the building.

This is where most small businesses actually land, and Tier 2 and Tier 3 both get
recommended in its place by people who don't know it exists.

- **Fits:** the work should start on its own — an email arrives, a form is
  submitted, it's Monday — and it has to move information between two systems, but
  there is exactly one step that needs judgment. Volume is steady. Tier 2 works but
  somebody is tired of remembering to go do it.
- **Person approves each run, or each batch.** Nothing goes to a customer, a
  patient, or a payment without a human clicking yes. That approval step is what
  makes this tier safe, and it is not optional.
- **Cost:** a monthly subscription for the automation tool (usually tens of dollars,
  priced by how many times it runs), plus whatever the AI step costs, plus setup.
- **Setup:** a few days to a few weeks. No developer strictly required, but somebody
  has to be willing to learn the tool — and that somebody is a real, named person
  spending real hours, not a weekend.
- **Biggest risk:** it's built by one enthusiastic person, it lives in their
  account, and nobody else knows how it works. Put it in a company account from day
  one and write down what it does in plain English.
- **Tell them:** the approval step feels like it defeats the purpose. It doesn't —
  it's the difference between a tool and a liability, and it still saves most of the
  time because approving is far faster than doing.

**Between 2 and 2.5:** if a person is happy to sit down and drive it, that's Tier 2
and it's cheaper. Go to 2.5 when the problem is that nobody remembers to sit down.

### Tier 3 — A custom build
Software connecting AI to their systems, running on a trigger or a schedule,
usually without a person watching each run. Needs a developer.

- **Fits:** high volume, needs to touch other systems, needs to run unattended, and
  Tier 2.5 has been tried and genuinely hit a wall — the off-the-shelf tool can't
  reach their system, or the run volume makes its pricing absurd.
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

### Three things to settle before you commit to the tier

**1. What they already own.** If Phase 1 turned up a tool they've already bought,
say plainly whether it fits this tier. Three honest answers: it fits, use it; it
fits but needs setting up properly, here's what's missing; it doesn't fit this
process, here's what it *is* good for. Money already spent doesn't earn a tool a
pass, and it doesn't disqualify it either.

**2. The account it runs on.** If Phase 5 flagged sensitive information, the tier
you name has to run on a business plan with the right contract signed and training
switched off. Write that into the recommendation as a requirement, not a footnote —
"Tier 2, on a business plan with a BAA" is the recommendation, not "Tier 2."

**3. What breaks this.** Before you write it down, spend five lines on how it fails.
Say them out loud:
- The person who set it up leaves. Who can run it in a month?
- The volume doubles. Does the cost or the review time still work?
- The vendor changes its pricing or its rules.
- The reference files go stale and it confidently quotes last year's prices.
- Nobody reviews the output after week three.

If you can't answer one of these, that's the real first step, not the build.

### Does it clear?

Now compare Phase 6's value per month against what this specific tier costs — the
subscriptions, the setup hours, and the standing review time. Give them payback in
months. If it doesn't clear, say so and drop a tier, or say the honest answer is
Tier 0 after all. Reversing yourself here is the filter working, not a mistake.

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

Show them the draft before you finalize it, the same way you showed the map: **"What
did I get wrong?"** Then hand over a one-page summary they can keep and show someone
else:

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

Give them the two HTML diagram files alongside it.

---

## The worksheet

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
