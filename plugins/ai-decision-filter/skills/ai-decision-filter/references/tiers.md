# Phase 7 — Which level of AI

Five levels. Recommend exactly one, name it plainly, and explain what it does not
do.

---

## Before you name a tier, show them what each one looks like in their process

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

---

## Tier 0 — No AI

The work was waste, a settings change, or boring automation. Or the volume is too
low to matter. **This is the most common correct answer.**

## Tier 1 — People need a chatbot

Give the staff a paid ChatGPT/Claude/Copilot account and real training.

- **Fits:** varied one-off thinking work — drafting, rewriting, brainstorming,
  explaining, "help me word this."
- **Person is in the loop every single time.** Nothing runs unattended.
- **Cost:** per-person subscription, plus training time.
- **Setup:** days.
- **Biggest risk:** everyone uses it differently and nobody learns anything. Fix
  with training and a few shared example prompts.
- **Tell them:** results vary person to person. That's expected at this tier.

## Tier 2 — A work assistant with your material in it

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

## Tier 2.5 — An automation tool with one AI step and an approval step

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

## Tier 3 — A custom build

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

---

## Three things to settle before you commit to the tier

**1. What they already own.** If Phase 1 turned up a tool they've already bought,
say plainly whether it fits this tier. Three honest answers: it fits, use it; it
fits but needs setting up properly, here's what's missing; it doesn't fit this
process, here's what it *is* good for. Money already spent doesn't earn a tool a
pass, and it doesn't disqualify it either.

**2. The account it runs on.** If Phase 5 flagged sensitive information, the tier
you name has to run on a business plan with the right contract signed and training
switched off. Write that into the recommendation as a requirement, not a footnote —
"Tier 2, on a business plan with a BAA" is the recommendation, not "Tier 2." See
`decide.md`.

**3. What breaks this.** Before you write it down, spend five lines on how it fails.
Say them out loud:
- The person who set it up leaves. Who can run it in a month?
- The volume doubles. Does the cost or the review time still work?
- The vendor changes its pricing or its rules.
- The reference files go stale and it confidently quotes last year's prices.
- Nobody reviews the output after week three.

If you can't answer one of these, that's the real first step, not the build.

---

## Does it clear?

Now compare Phase 6's value per month against what this specific tier costs — the
subscriptions, the setup hours, and the standing review time. Give them payback in
months.

If it doesn't clear, say so and drop a tier, or say the honest answer is Tier 0
after all. Reversing yourself here is the filter working, not a mistake.
