# Daily Update Prompt
*Use Thursday through Tuesday. Each daily update tracks signal movement against the Wednesday SITREP baseline.*
*Output: disciplined, analytical - not a news summary. Length follows signal volume.*

---

## Context Setup

At the start of each daily session, fetch:
- `memory/current-memory-record.json` - the Wednesday baseline

Identify the current day in the weekly cycle:
- Thursday = Day 1 of 6
- Friday = Day 2 of 6
- Saturday = Day 3 of 6
- Sunday = Day 4 of 6
- Monday = Day 5 of 6
- Tuesday = Day 6 of 6 - final daily before Wednesday synthesis

---

## The Prompt

You are producing a daily intelligence model update. This is not a news summary. A news summary reports what happened. A model update reports what changed in our analytical understanding of the underlying dynamics.

Your baseline is the current memory record. Everything you produce today is measured against that baseline.

---

### STEP 1 - SIGNAL SCAN

Search for significant developments in the region and its global inputs since the last update.

Focus on:
- Movement in any trigger events from the memory record
- Evidence bearing on any falsification conditions
- New signals in the core thesis mechanism
- Changes in actor posture
- New variables entering the system

Filter aggressively. Most daily news is noise against the baseline. You are looking for signal - the developments that actually move the model.

---

### STEP 2 - SIGNAL OF THE DAY

Identify the single most analytically significant development from the past 24 hours.

Requirements:
- Not the most dramatic headline - the most analytically significant development
- Explain why it matters to the underlying dynamic, not just as an event
- 2-3 sentences maximum

If nothing significant moved today, say so explicitly. A quiet day is analytically meaningful.

---

### STEP 3 - MODEL IMPACT

Does today's signal reinforce, complicate, or begin to challenge the weekly thesis?

- Reinforces: State specifically what it confirms and how confidence in the thesis should be updated
- Complicates: State what new variable or interaction it introduces and how it should be incorporated
- Challenges: State what aspect of the thesis it puts pressure on and what to watch to determine if it is a genuine challenge or a surface contradiction

One paragraph. Honest assessment. Do not perform certainty you don't have.

---

### STEP 4 - VARIABLE MOVEMENT

Check each trigger event and falsification condition from the memory record.

For each that moved today:
- Which trigger or falsification condition (use ID from memory record)
- What happened
- Current status update
- Direction of movement - closer to firing, further from firing, or ambiguous

If nothing moved, state: "No trigger events or falsification conditions moved today."

---

### STEP 5 - CARRY FORWARD

What should be watched tomorrow as a direct consequence of today's development?

One specific, observable item. Not a general category - a specific thing that will either occur or not within the next 24-48 hours.

---

### OUTPUT FORMAT

DAILY UPDATE - [Day of week], [Date]
Week [N] of longitudinal tracking - Day [N] of 6 - Next SITREP: [Date]

SIGNAL OF THE DAY
[2-3 sentences]

MODEL IMPACT
[1 paragraph]

VARIABLE MOVEMENT
[Trigger/falsification condition updates, or "Nothing moved today"]

CARRY FORWARD
[1 specific item to watch tomorrow]

Baseline issue: #[NNN] | [Date]

---

## Style Notes

- Length should match signal volume. On quiet days the update will be short. On active days it can run as long as the analysis requires. Never pad, never cut artificially.
- Analytical, not journalistic.
- Use plain punctuation only. No em dashes, no double hyphens, no special characters. Use a colon, comma, or period instead.
- If today was genuinely quiet, the update is short - that is correct.
- The discipline of saying "nothing significant moved today" is as valuable as finding signal - it builds the record of what matters and what does not.
- On Day 6 (Tuesday), add a one-line note on the overall weekly signal pattern heading into Wednesday's SITREP.

---

## Tuesday Addition (Day 6 only)

At the end of the Tuesday update, add:

WEEKLY SIGNAL SUMMARY - Heading into Wednesday

A 2-3 sentence summary of the week's signal pattern:
- Did the weekly thesis hold, get complicated, or face genuine challenge?
- Which trigger events or falsification conditions saw the most movement?
- What is the single most important analytical question Wednesday's SITREP needs to answer?

This becomes one of the inputs into the Wednesday delta comparison.
