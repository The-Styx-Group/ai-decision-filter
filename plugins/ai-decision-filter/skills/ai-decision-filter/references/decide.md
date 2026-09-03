# Phases 5 and 6 — Does AI fit, and what is it worth

Two halves. First decide whether AI belongs here at all, then put a number on it.
Both are done out loud, with the owner watching.

---

# Phase 5 — Does AI actually fit?

Only reach this phase if real work remains after Phases 3 and 4.

AI earns its place on **messy language and judgment on unstructured material**.
Score it, don't eyeball it. Give each line **0, 1, or 2** and show them the sheet —
a verdict they can see the arithmetic behind is a verdict they can argue with, which
is the point.

## Points toward AI

0 = no · 1 = partly · 2 = strongly

| | Score |
|---|---|
| The input is messy — emails, notes, PDFs, recordings, free text | |
| Every instance looks a little different | |
| The work is reading, summarizing, drafting, sorting, or pulling facts out | |
| A capable person could do it right from written instructions, no special training | |
| There is a lot of it | |
| Roughly right is useful — a person polishes it | |
| **Toward total (0–12)** | |

## Points against AI

0 = not true · 1 = somewhat · 2 = very true

| | Score |
|---|---|
| The rule is exact and the information is already tidy (that's Phase 4) | |
| A wrong answer causes real harm before a person could catch it | |
| There is no practical way to tell whether the output is right | |
| It's low volume — a few times a month, a few minutes each | |
| Nobody has been named to own it after launch | |
| The people doing it don't want it and won't use it | |
| **Against total (0–12)** | |

## Reading the score

- **Toward 8+ and Against 4 or less** → AI fits. Continue to the tiers.
- **Toward 5–7, or Against 5–7** → borderline. Say "borderline" out loud, name the
  one thing that would tip it, and recommend the smallest possible trial rather than
  a build.
- **Toward 4 or less, or Against 8+** → no AI. Say so and explain which lines drove
  it.

Any single **Against** line scored a 2 is worth stopping on by itself. Talk about it
before you total anything.

**Hard stops** (these override the score — repeated from SKILL.md because they get
skipped). Do not recommend AI, at any tier, when:
- Nobody has time to review its output and the output goes straight to a customer,
  a patient, a regulator, or a payment.
- The process is still done three different ways by three people (go back to Phase 3).
- They cannot name a person who will own it.

---

## Sensitive information changes the tool, not the answer

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

# Phase 6 — What is it actually worth?

Do this math out loud, with their numbers. Use the **hands-on minutes** from Phase 0
— the time someone is actually working, not the time it sits in an inbox. Waiting
time is real pain, but AI doesn't get it back; fixing the handoff does, and that was
Phase 3.

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

## Rules for honest math

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

Hold the value figure. You compare it against the cost of a specific tier at the end
of Phase 7, once you know which tier you're recommending. See `tiers.md`.
