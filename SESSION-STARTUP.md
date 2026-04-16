Session Startup Instructions
Copy this into every new Claude session to orient the model immediately.
---
For Wednesday SITREP Sessions
Paste this at the start of the session:
---
> You are producing the weekly Middle East SITREP for a longitudinal geopolitical intelligence system. This is Issue #[NNN].
>
> Please fetch the following files from the repository:
>
> **Memory record (previous week's baseline):**
> `[raw GitHub URL to memory/current-memory-record.json]`
>
> **Daily updates from this week (if available):**
> `[raw GitHub URLs to each daily update from this week]`
>
> Once you have fetched and read those files, run the delta comparison prompt against current signals, then produce the full SITREP using the Triad synthesis prompt.
>
> The prompts are available at:
> - Delta comparison: `[raw GitHub URL to prompts/delta-comparison-prompt.md]`
> - Triad synthesis: `[raw GitHub URL to prompts/triad-synthesis-prompt.md]`
>
> After producing the SITREP, extract the memory record in JSON format so I can commit it to the repository.
---
For Daily Update Sessions (Thursday–Tuesday)
Paste this at the start of the session:
---
> You are producing a daily intelligence model update for a longitudinal geopolitical intelligence system. Today is [Day of week], [Date] — Day [N] of 6 in the current weekly cycle.
>
> Please fetch the current baseline:
>
> **Memory record:**
> `[raw GitHub URL to memory/current-memory-record.json]`
>
> The daily update prompt is at:
> `[raw GitHub URL to prompts/daily-update-prompt.md]`
>
> Fetch the memory record, then scan for today's signals and produce the daily update. Track all trigger events and falsification conditions from the memory record.
---
GitHub Raw URL Format
To get a raw file URL from GitHub:
Navigate to the file in the repository
Click "Raw" button
Copy the URL — it will look like:
`https://raw.githubusercontent.com/[username]/[repo]/main/[filepath]`
Or construct it manually:
`https://raw.githubusercontent.com/[username]/[repo]/main/memory/current-memory-record.json`
---
After Each Wednesday Session — Commit Checklist
[ ] Save SITREP output to `/sitreps/YYYY-MM-DD-issue-NNN.md`
[ ] Copy new memory record JSON into `/memory/current-memory-record.json` (overwrite)
[ ] Append previous week's memory record to `/memory/memory-archive.json`
[ ] Commit all changes with message: `Issue NNN — YYYY-MM-DD`
After Each Daily Session — Commit Checklist
[ ] Save daily update to `/daily-updates/YYYY-MM-DD-[weekday].md`
[ ] Commit with message: `Daily update — YYYY-MM-DD [Weekday]`
