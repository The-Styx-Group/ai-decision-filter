# AI Decision Filter

**Should this process use AI at all?**

Most small business processes should not. They're slow because of extra steps,
unclear ownership, or bad handoffs — and AI applied to a broken process just makes
a broken process faster and harder to inspect.

This is a plugin for ChatGPT and Codex that walks a business owner through
answering that question honestly. It interviews you about one process, maps it out,
hunts for waste, checks whether ordinary automation would do the job, does the time
and money math without inflating it, and only then picks a level of AI — if any.

It is designed to talk you out of AI when AI is the wrong answer.

---

## What it actually does

**0. Checks it's worth doing first.** Three questions — how often, how many hands-on
minutes, what happens if it goes wrong. Under about four hours a month and it tells
you so in two minutes instead of interviewing you for forty.

**1. Interviews you.** One question at a time, in plain language — who touches the
process, how long it takes, how often it runs, where it breaks, what happens when
it goes wrong.

**2. Draws it.** Produces a process map you can open in your browser, then redraws
it as you correct it. Most people find a step nobody owns at this stage.

**3. Looks for waste first.** Steps that could be deleted, work done twice,
approvals nobody has ever refused. Sometimes this is the whole fix and the session
ends here.

**4. Checks the boring option.** A form, a template, a rule in software you already
pay for. Ordinary automation is cheaper, more predictable, and needs less
babysitting than AI. Often it's already sitting unused in a tool you own.

**5. Does honest math.** Hours spent now, realistic hours saved (never 100%),
review time subtracted, compared against what the fix costs.

**6. Picks a level — or none.**

| Tier | What it means |
|---|---|
| **0 — No AI** | Fix the process, or use ordinary automation. The most common correct answer. |
| **1 — Chatbot** | Staff need paid AI accounts and real training. A person is in the loop every time. |
| **2 — Work assistant** | A shared assistant set up with your files, policies, and templates so answers are consistent and specific to you. |
| **2.5 — Automation with an AI step** | An off-the-shelf automation tool starts the process on its own, hands the messy part to AI, and waits for a person to approve. Where most small businesses actually land. |
| **3 — Custom build** | Software connecting AI to your systems, running unattended. Needs a developer and permanent maintenance. Almost nobody should start here. |

If the process touches patient records, customer financial details, or payments, it
doesn't refuse — it tells you which kind of account the work is allowed to happen
on, and what the vendor has to have signed.

**7. Decides who owns it.** A named person, a review schedule, what counts as a bad
output, what it's never allowed to do alone, and the conditions under which you turn
it off. Ends with a second diagram of that maintenance loop, which is the one you
pin up.

You finish with a one-page written decision, two diagram files, and a worksheet
holding everything the session captured.

---

## Coming back to it later

The plugin includes a second skill, **Process Re-Review**. Hand it the worksheet or
the written decision and it picks the process back up — checks what changed, compares
what actually happened against what was predicted, redraws the map, and lands on one
of five answers: holding, adjust, move up a tier, move down or stop, or the process
changed enough to start over.

Use it when your review date comes up, when the process changes, or to finish a
session that got interrupted.

---

## Install it

You need the ChatGPT desktop app or the Codex command line tool.

```
codex plugin marketplace add The-Styx-Group/ai-decision-filter
```

Then open the plugin browser, install **AI Decision Filter**, and start a new
conversation. In Codex CLI, `/plugins` opens the browser.

To pick up later updates:

```
codex plugin marketplace upgrade ai-decision-filter
```

**Note on availability:** tested working on a personal ChatGPT Pro account. If you
don't see a Skills tab under Plugins, your account doesn't have them yet — on a
workspace plan an admin can switch them off.

## Use it

Start a conversation and describe one process:

> Every time a customer emails an invoice, my bookkeeper enters it, and anything
> over $500 waits on me to approve it. It's slow and I want to know if AI helps.

It takes it from there. Do one process at a time — if you have several, it'll ask
which one hurts most.

---

## What's inside

```
plugins/ai-decision-filter/
├── .codex-plugin/plugin.json
└── skills/
    ├── ai-decision-filter/
    │   ├── SKILL.md                    the spine — the phases, in order
    │   └── references/
    │       ├── intake.md               the interview questions
    │       ├── diagrams.md             how the diagrams get drawn
    │       ├── decide.md               the scoring sheet and the money math
    │       ├── tiers.md                the five levels, and picking one
    │       ├── handover.md             ownership, the decision, the worksheet
    │       └── example-flowchart.html  a worked process map
    └── process-re-review/
        └── SKILL.md                    revisiting a decision later
```

`SKILL.md` runs the session and pulls in each reference file at the phase that
needs it.

The diagrams are self-contained HTML files — open them in any browser, no software
needed. They use Google Fonts, so they look best online.

## License

MIT. Take it, change it, use it with your own clients.
