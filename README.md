Global Intelligence SITREP System
A structured, longitudinal intelligence analysis framework producing weekly situation reports and daily model updates on global geopolitical, economic, and security dynamics.
Built on the Triad Analytical Model — thesis formation, interaction mapping, red team challenge, risk forecast, pattern recognition, and final synthesis — with full falsification condition tracking and compounding memory architecture.
---
What This Is
This is not a news aggregation system. It is an analytical intelligence model that:
Sets a thesis each Wednesday based on current signals
Tracks that thesis daily against new developments
Updates the model explicitly when evidence confirms, complicates, or falsifies the thesis
Accumulates a documented history of analytical reasoning, forecast accuracy, and model evolution
Gets smarter over time because every previous assessment is available as context
The product is a weekly SITREP (Wednesday) fed by six daily model updates (Thursday–Tuesday). The weekly synthesis closes the loop on the daily signals and resets the baseline for the next cycle.
---
Repository Structure
```
/intelligence-repo
  /sitreps                    # Full weekly SITREP outputs
  /daily-updates              # Daily model update outputs  
  /memory                     # The analytical memory system
  /prompts                    # Production-ready prompt templates
  /templates                  # Output format templates
  /source-library             # Tracked sources by region
  README.md                   # This file
```
---
The Weekly Cycle
Wednesday — SITREP Day
Open new Claude session in the Intelligence Project
Provide the raw URL to `/memory/current-memory-record.json`
Claude fetches the memory record and runs delta comparison against fresh signals
Full SITREP produced using the Triad Model
Save output to `/sitreps/YYYY-MM-DD-issue-NNN.md`
Copy the new memory record block into `/memory/current-memory-record.json`
Append previous week's memory record to `/memory/memory-archive.json`
Cycle resets
Thursday through Tuesday — Daily Update Days
Open Claude session
Provide the raw URL to `/memory/current-memory-record.json`
Claude fetches baseline and scans for signal movement
Short daily update produced — signal of the day, model impact, variable movement, carry forward
Save to `/daily-updates/YYYY-MM-DD-[day].md`
The Following Wednesday
Provide memory record URL plus URLs of the week's daily updates
Claude fetches all, runs full delta comparison
New SITREP produced with explicit continuity from previous week
Analytical delta documented — what changed, what held, what was wrong and why
---
Memory Architecture
The memory system is the spine of the entire product. It converts a series of individual outputs into a compounding analytical model.
`current-memory-record.json`
Overwritten every Wednesday with the new week's distilled memory record. Contains:
Core thesis
30/60/90-day forecasts with probability ranges
Active trigger events being watched
Falsification conditions
Key uncertainties
Pattern match
Confidence levels
`memory-archive.json`
Never overwritten — only appended. Every previous week's memory record accumulates here. This is the longitudinal analytical history. Over time it becomes a documented record of:
How the model evolved
Which forecasts proved accurate
Which falsification conditions fired
Which variables proved most predictive
Where the analytical blind spots consistently appeared
---
The Triad Analytical Framework
Every SITREP follows this six-step process:
Step 1 — Core Thesis
Identify the single most important system-level dynamic. Causal, not chronological. Cross-domain. Committed — no hedging overload.
Step 2 — Interaction Pathways
2–4 key pathways where signals reinforce or contradict each other. Each labeled: stabilizing, destabilizing, or mixed.
Step 3 — Red Team Challenge
Critically assess the core thesis. Alternative explanations. What may be overestimated. What missing information would change the assessment.
Step 4 — Risk Forecast
30, 60, and 90-day forward assessment with explicit probability ranges. Trigger events that would accelerate change. No vague language.
Step 5 — Pattern Recognition
Historical analog matching. What does this situation most resemble structurally and why.
Step 6 — Final Intelligence Brief
600–1000 words. Prose only. Leads with underlying dynamic not events. Shows how signals combine into a single risk pattern. Ends with why this matters beyond the immediate region.
Falsification Conditions
Explicit statements of what would invalidate the current thesis. Tracked weekly against outcomes.
Memory Record
Distilled output of the above for longitudinal tracking. Feeds the following week's delta comparison.
---
Daily Update Framework
Short. Disciplined. 300–400 words maximum.
Signal of the Day — the single most analytically significant development
Model Impact — does this reinforce, complicate, or challenge the weekly thesis? Honest assessment.
Variable Movement — which weekly trigger events or falsification conditions moved, and in which direction
Carry Forward — what to watch tomorrow as a direct consequence of today
---
Global Input Framework
Middle East SITREPs are not purely regional. The following global inputs are tracked as active variables in every assessment:
China — energy exposure, diplomatic positioning, leverage over Iran
Russia — energy windfall incentive structure, Ukraine war funding implications
Pakistan — mediation access and limits
United States — strategic bandwidth, military stock depletion, domestic political constraints
India — energy exposure, hedging strategy
Europe — inflationary shock, energy security, political cohesion
Global South — normative opposition accumulation, multilateral framework erosion
---
Regional Framework (Middle East)
Five standing sub-regional nodes:
Persian Axis — Iran, Iraq, proxy network
Hormuz / Chokepoint — the strait as its own analytical unit
The Levant — Israel, Lebanon, West Bank, Syria
The Gulf — GCC, Saudi, UAE, Qatar, Bahrain
Red Sea / Yemen — Houthis, STC, Bab el-Mandeb
---
How Claude Accesses This Repo
In each session, provide raw GitHub file URLs:
```
Current memory record:
https://raw.githubusercontent.com/[username]/[repo]/main/memory/current-memory-record.json

Memory archive:
https://raw.githubusercontent.com/[username]/[repo]/main/memory/memory-archive.json

Specific SITREP:
https://raw.githubusercontent.com/[username]/[repo]/main/sitreps/2026-04-15-issue-001.md
```
Claude fetches these directly using web tools. No copy-paste required beyond the URL.
---
Analytical Principles
Causality over chronology — explain mechanisms, not sequences of events
Committed thesis — form a view, then attack it, then refine it
Falsification discipline — always state what would prove you wrong
Probability ranges — express uncertainty numerically, not with vague language
Delta awareness — the change in state is often more significant than the current state
Global inputs — regional analysis without external power inputs is incomplete
Compounding value — each week builds on the last; the product gets better over time
---
Output Naming Convention
```
SITREPs:        YYYY-MM-DD-issue-NNN.md          e.g. 2026-04-15-issue-001.md
Daily updates:  YYYY-MM-DD-[weekday].md           e.g. 2026-04-16-thursday.md
Memory records: current-memory-record.json         (always current week)
                memory-archive.json                (all previous weeks)
```
---
System designed and built in collaboration with Claude (Anthropic) — April 2026
