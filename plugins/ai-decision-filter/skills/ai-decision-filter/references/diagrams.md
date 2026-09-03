# Drawing the diagrams

Two diagrams get produced in a session: the **process map** (Phase 2, redrawn
several times as detail surfaces) and the **maintenance loop** (Phase 8, drawn once
at the end).

Both are a single self-contained HTML file the owner can open in a browser. No
build step, no image files, no external assets except the Google Fonts stylesheet.
Copy `example-flowchart.html`, replace the contents of the `<svg>`, keep everything
else.

---

## First: does this need a diagram at all?

- **Five steps or fewer, one person, no branches** — use a table, not a diagram. Two
  columns: step, who does it. A five-box flowchart is decoration.
- **Three or more people touching it** — draw it in lanes, one horizontal lane per
  person, boxes placed in the lane of whoever does them. The lanes are the point: a
  step nobody can place, or a lane that's empty in the middle of the process, is the
  ownership gap the owner has been living with. Nothing else in this exercise shows
  it as fast.
- **Otherwise** — the ordinary top-to-bottom flowchart below.

---

## Non-negotiable rules

1. **Shape carries meaning, not color.**
   - Oval (`rx="24"`) — start and end
   - Rectangle (`rx="6"`) — a step someone performs
   - Diamond — a decision, maximum 3 exits
   - Small filled dot (`r="4"`) — where branches rejoin
2. **Flow runs top to bottom.** From a diamond, Yes goes down, No goes right.
   Label every outgoing arrow anyway.
3. **Draw arrows first, then boxes.** SVG paints in document order, so boxes
   drawn last cover the arrow ends cleanly.
4. **Connectors are straight or right-angled.** Never diagonal. Use two straight
   segments to turn a corner.
5. **Arrow labels sit on a small background rectangle** the same color as the
   canvas, so the line doesn't run through the text.
6. **Accent color appears once or twice, never more.** Use it for the main path
   through the process, or the single most consequential decision — not both.
7. **Every diagram needs `<title>` and `<desc>`** inside the SVG, with matching
   `aria-labelledby` ids, so a screen reader can announce it.
8. **No drop shadows, no gradients, no glow.** Flat, thin strokes, plenty of space.

---

## Colors and type

```
paper   #f5f5f5   canvas background
ink     #2d3142   text and step outlines
muted   #4f5d75   connectors, labels, secondary text
accent  #eb6c36   the main path — sparingly
white   #ffffff   step fill
```

Fonts: `Geist` for labels, `Geist Mono` for small caps labels and legends,
`Instrument Serif` for the page heading above the diagram.

If the business has its own brand colors and they want them used, swap `accent`
for their brand color and leave everything else alone. Do not swap `ink` for a
brand color — readability first.

---

## Sizing and spacing

- Canvas `viewBox="0 0 1000 600"`. Grow the height for longer processes; keep the
  width at 1000.
- Step boxes: 160 wide × 48 tall. Decision diamonds: 200 wide × 96 tall.
- At least 32px of vertical gap between rows.
- Snap coordinates to multiples of 4.
- **If it needs more than about 12 boxes, the diagram is too dense.** Split it, or
  collapse a stretch of steps into one box named for what that stretch accomplishes.
  A crowded map is worse than no map.

---

## The process map (Phase 2)

Draw what actually happens today, not the tidy version:

- Include the waiting. A step that sits in someone's inbox for two days is a real
  step — draw it and label the delay.
- Include the rework loops. The arrow that goes backward when something is wrong is
  usually where the pain lives.
- Name each box with a verb: "Enter invoice," not "Invoice entry."
- Put the person's name or role under the box in small muted text.
- Once Phase 1's pain points are known, mark them: a short accent-colored label
  beside the box, e.g. `2 DAY WAIT` or `DONE 3 WAYS`.
- Redraw the whole file each time they correct you. Don't patch — it drifts.

Add a legend strip at the bottom explaining the shapes. The example file shows the
pattern.

**Lanes, when three or more people are involved.** Divide the canvas into horizontal
bands, one per person, name each band on the left in muted small caps, and separate
them with a thin `muted` rule. Steps sit in the band of whoever performs them. Flow
still runs generally left to right across the lanes; an arrow crossing a lane
boundary is a handoff, and handoffs are where the delay lives — label the wait on
those arrows specifically. Keep the same shapes, colors, and spacing rules.

**Saving it.** Name the file `<process-name>-process-map.html` and save it next to
the worksheet, so a later review can open both. If you can't save files, put the
full HTML in a code block and tell them to paste it into a text file and rename it
to end in `.html`.

---

## The maintenance loop (Phase 8)

A cycle, not a top-to-bottom flow. Four to six boxes arranged in a ring with arrows
running clockwise, returning to the start.

Typical ring:

```
Run  →  Review the output  →  Correct what's wrong  →  Update the instructions
     →  Log what changed  →  (back to Run)
```

Then hang two things off the ring:

- **The owner**, in a box beside the ring with a line to it, showing their name and
  their review schedule.
- **The escalation path**, branching off "Review the output" — an accent-colored
  arrow to a box reading what happens when something is wrong and who hears about
  it, ending in the manual fallback.

To place a ring of boxes, put them at the compass points of the canvas — top center,
right, bottom right, bottom left, left — and connect with right-angled arrows.
Don't attempt curved arcs; straight segments read fine.

This is the diagram the owner keeps. Put the review date and owner name in it, in
text, so a printed copy is self-explanatory. Name the file
`<process-name>-maintenance-loop.html`.

---

## Before handing over a diagram

- Every arrow leaving a diamond is labeled.
- No line passes through a box or through text.
- Accent color used once or twice.
- Title and description filled in, no `[placeholder]` text left anywhere.
- Every box name would mean something to someone who wasn't in the conversation.
- The file opens in a browser and needs nothing else.
