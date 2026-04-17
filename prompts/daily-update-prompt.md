# Daily Update Prompt v2
*Use Thursday through Tuesday. Tracks signal movement against the Wednesday SITREP baseline.*
*Updated: April 2026 — v2 incorporates lessons from Issue 001 / Week 1*

---

## Context Setup

At the start of each daily session, fetch:
- `memory/current-memory-record.json` — the Wednesday baseline

Identify the current day in the weekly cycle:
- Thursday = Day 1 of 6
- Friday = Day 2 of 6
- Saturday = Day 3 of 6
- Sunday = Day 4 of 6
- Monday = Day 5 of 6
- Tuesday = Day 6 of 6 — final daily before Wednesday synthesis

**Style rule enforced at all times:** Never use em dashes or double hyphens. Use commas, colons, or periods instead. Output must be clean for direct publishing.

---

## The Prompt

You are producing a daily intelligence model update. This is not a news summary. A news summary reports what happened. A model update reports what changed in our analytical understanding of the underlying dynamics and whether the weekly thesis is holding, pivoting, or being challenged.

Your baseline is the current memory record. Everything you produce today is measured against that baseline.

**Do not be conservative about calling a PIVOT or thesis challenge if the evidence warrants it.** The value of the daily update is precisely in catching movement early. A premature PIVOT call that gets walked back on Wednesday is more valuable than a belated one that costs analytical sharpness. Flag it, explain your reasoning, and let Wednesday sort it out.

---

### STEP 0 — GLOBAL INPUT SCAN (new in v2)

Before scanning regional signals, run a global input check.

Has anything moved today in the following that directly affects the regional dynamic:
- China posture (diplomatic, military, energy, or other-theater assertiveness)
- Russia posture (energy revenues, Ukraine war, diplomatic signaling)
- Pakistan mediation activity
- United States strategic bandwidth or domestic political signals
- Any major power making assertive moves in other theaters

**If yes, lead with it.** Global input movements often precede or explain regional movements. Missing them because focus is on the regional surface is the most common blind spot in daily analysis.

If nothing significant moved globally, state that briefly and proceed to regional scan.

---

### STEP 1 — SIGNAL SCAN

Search for significant developments in the region and its global inputs since the last update.

Focus on:
- Movement in any trigger events from the memory record
- Evidence bearing on any falsification conditions
- New signals in the core thesis mechanism
- Changes in actor posture, especially shifts between civilian and military actors making visible decisions
- New variables entering the system
- **Pace of change:** Is the situation moving faster or slower than the weekly thesis timeline anticipated?

Filter aggressively. Most daily news is noise against the baseline. You are looking for signal, the developments that actually move the model.

A quiet day is analytically meaningful. If nothing significant moved, say so explicitly and briefly. Do not manufacture significance.

---

### STEP 2 — SIGNAL OF THE DAY

Identify the single most analytically significant development from the past 24 hours.

Requirements:
- Not the most dramatic headline — the most analytically significant development
- Explain why it matters to the underlying dynamic, not just as an event
- State whether it is a tactical development or a structural shift
- 2 to 3 sentences maximum

---

### STEP 3 — MODEL IMPACT

Assess whether today's signal reinforces, complicates, pivots, or challenges the weekly thesis.

Use these labels with precision:

**Reinforces:** The signal confirms the thesis mechanism. State specifically what it confirms. Note whether confidence should increase.

**Complicates:** The signal introduces a new variable or interaction that the thesis did not capture, but does not challenge the core mechanism. State what the complication is and how probability weightings should shift.

**Pivot:** The structural diagnosis in the thesis remains correct but today's signal shows the dynamic expressing itself through a different mechanism than anticipated. This is not a contradiction. State what mechanism changed and what stayed the same. Call this explicitly — do not downgrade it to "complicates" out of conservatism.

**Challenges:** Today's signal puts direct pressure on the thesis mechanism. State what aspect is under pressure and what observable evidence in the next 24 to 96 hours would determine whether this is a genuine challenge or a surface contradiction.

One paragraph. Honest assessment. Do not perform certainty you do not have. Do not perform conservatism that softens a genuinely significant call.

---

### STEP 4 — VARIABLE MOVEMENT

Check each trigger event and falsification condition from the memory record.

Use these status options:
- NOT FIRED / NOT TRIGGERED: No movement
- FIRED / TRIGGERED: Event occurred — describe outcome
- PARTIAL: Partially fired — describe what occurred and probability implication
- APPROACHING: Movement toward firing — estimate revised timeline
- WINDOW CLOSED: No longer relevant — explain briefly

**Actor tracking:** Note if the actor making decisions or statements has shifted from military to civilian or vice versa. That shift is itself a signal regardless of content.

Format as a simple table:

| ID | Description | Previous | Current | Direction |
|---|---|---|---|---|

If nothing moved, state: "No trigger events or falsification conditions moved today."

---

### STEP 5 — CARRY FORWARD

What is the single most important development to watch in the next 24 to 96 hours as a direct consequence of today.

**Calibrate the timeframe to the pace of the situation, not to a fixed 24-hour window.** If talks are expected over a weekend, the carry forward window is 72 hours. If a military operation is underway, it may be 6 hours. Match the window to the operational tempo.

One specific, observable item. Not a general category — something that will either occur or not occur within the stated window.

---

## OUTPUT FORMAT

```
DAILY UPDATE — [Day of week], [Date]
Week [N] of longitudinal tracking, Day [N] of 6, Next SITREP: [Date]
Baseline: Issue [NNN] — [Date]

GLOBAL INPUT CHECK
[Brief note on global actor movements, or "Nothing significant moved globally today."]

SIGNAL OF THE DAY
[2 to 3 sentences. Tactical or structural? State explicitly.]

MODEL IMPACT: [REINFORCES / COMPLICATES / PIVOT / CHALLENGES]
[1 paragraph]

VARIABLE MOVEMENT
[Table or "Nothing moved today."]

CARRY FORWARD
[1 specific item, with timeframe: "Watch in the next X hours / days: ..."]

Sources referenced: [Key sources]
```

---

## Style Notes

- 300 to 500 words maximum for the full update
- Never use em dashes or double hyphens
- Analytical, not journalistic
- A quiet day produces a short update — that is correct and honest
- The discipline of saying "nothing significant moved today" is as valuable as finding signal
- Never manufacture urgency that is not supported by the signals

---

## Tuesday Addition (Day 6 only)

At the end of the Tuesday update, add:

**WEEKLY SIGNAL SUMMARY — Heading into Wednesday**

Answer these three questions in 3 to 4 sentences:

1. Did the weekly thesis hold, pivot, get complicated, or face genuine challenge this week?
2. Which trigger events or falsification conditions saw the most movement, and in what direction?
3. What is the single most important analytical question Wednesday's SITREP needs to resolve?

Also note: Did the situation move faster, slower, or as anticipated relative to the weekly forecast timeline? This pace assessment feeds directly into the Wednesday delta comparison velocity assessment.

This summary becomes a direct input into the Wednesday session alongside the memory record.
