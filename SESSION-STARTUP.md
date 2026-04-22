# Session Startup Instructions

---

## URL Construction Logic

All repository URLs follow a predictable pattern. Claude constructs them automatically from the current date without human input.

**Base pattern:**
`https://raw.githubusercontent.com/TradingTimeMachine/sitrep-system/refs/heads/main/[filepath]`

**Fixed URLs (never change):**
- Memory record: `https://raw.githubusercontent.com/TradingTimeMachine/sitrep-system/refs/heads/main/memory/current-memory-record.json`
- Daily update prompt: `https://raw.githubusercontent.com/TradingTimeMachine/sitrep-system/refs/heads/main/prompts/daily-update-prompt.md`
- Delta comparison prompt: `https://raw.githubusercontent.com/TradingTimeMachine/sitrep-system/refs/heads/main/prompts/delta-comparison-prompt.md`
- Triad synthesis prompt: `https://raw.githubusercontent.com/TradingTimeMachine/sitrep-system/refs/heads/main/prompts/triad-synthesis-prompt.md`
- Source library: `https://raw.githubusercontent.com/TradingTimeMachine/sitrep-system/refs/heads/main/source-library/sources-by-region.md`

**Daily update URLs (constructed from date):**
`https://raw.githubusercontent.com/TradingTimeMachine/sitrep-system/refs/heads/main/daily-updates/YYYY-MM-DD-[weekday].md`

Examples:
- `daily-updates/2026-04-16-thursday.md`
- `daily-updates/2026-04-17-friday.md`
- `daily-updates/2026-04-18-saturday.md`
- `daily-updates/2026-04-19-sunday.md`
- `daily-updates/2026-04-20-monday.md`
- `daily-updates/2026-04-21-tuesday.md`

**SITREP URLs (constructed from date and issue number):**
`https://raw.githubusercontent.com/TradingTimeMachine/sitrep-system/refs/heads/main/sitreps/YYYY-MM-DD-issue-NNN.md`

**Missing day handling:** If a daily update or SITREP URL returns a 404 or error, skip it silently and note "no file found for [date]" in the session log. Do not halt the session.

---

## Automated Session Trigger (Minimum Input Required)

For a fully automated or near-automated session, Claude only needs:
- The current date
- The session type: "daily" or "sitrep"

From those two inputs Claude constructs all URLs, fetches all files, and proceeds without further human input. Missing files are skipped automatically.

---

## Wednesday SITREP Session

Say: "run the SITREP" and Claude will automatically fetch:

1. Current memory record
2. Delta comparison prompt
3. Triad synthesis prompt
4. Source library
5. This week's daily updates (Thursday through Tuesday, constructed from date)
6. The 4 most recent prior SITREP files (constructed from issue number and date)

**Why prior SITREPs are included:** The system is longitudinal and accumulative. Each Wednesday synthesis is richer when it can see the full arc of prior issues, not just the immediately preceding memory record. The memory record contains distilled structural continuity. The prior SITREP files provide narrative depth, thesis evolution, and forecast accuracy track record. As the archive grows beyond 12 issues, the rolling window stays at 4 most recent SITREPs plus the memory record. If fewer than 4 SITREPs exist, fetch all available.

Then run delta comparison first, then full Triad synthesis.

---

## Daily Update Session (Thursday through Tuesday)

Say: "run the daily" and Claude will automatically fetch:

1. Current memory record
2. Daily update prompt

Then scan for signals and produce the daily update.

---

## After Each Wednesday Session — Commit Checklist

- [ ] Save SITREP to `sitreps/YYYY-MM-DD-issue-NNN.md`
- [ ] Overwrite `memory/current-memory-record.json` with new memory record JSON
- [ ] Append previous memory record to `memory/memory-archive.json`
- [ ] Commit message: `Issue NNN - YYYY-MM-DD`

## After Each Daily Session — Commit Checklist

- [ ] Save daily update to `daily-updates/YYYY-MM-DD-[weekday].md`
- [ ] Commit message: `Daily update - YYYY-MM-DD [Weekday]`
