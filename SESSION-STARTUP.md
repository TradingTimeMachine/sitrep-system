# Session Startup Instructions
Copy this into every new Claude session to orient the model immediately.

---

## URL Construction Logic

All repository URLs follow a predictable pattern. Claude can construct them automatically from the current date without any human input.

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

**Missing day handling:** If a daily update URL returns a 404 or error, skip it silently and note "no update filed for [weekday]" in the session log. Do not halt the session.

**SITREP URLs (constructed from date and issue number):**
`https://raw.githubusercontent.com/TradingTimeMachine/sitrep-system/refs/heads/main/sitreps/YYYY-MM-DD-issue-NNN.md`

---

## Automated Session Trigger (Minimum Input Required)

For a fully automated or near-automated session, Claude only needs:
- The current date
- The session type: "daily" or "sitrep"

From those two inputs Claude constructs all URLs, fetches all files, and proceeds without further human input. Missing files are skipped automatically.

---

## Manual Session Startup

### For Wednesday SITREP Sessions

Say: "run the SITREP" and paste the weekly daily update URLs if not auto-constructing.

Claude will automatically fetch:
- Memory record
- Delta comparison prompt
- Triad synthesis prompt
- Source library
- Any daily update URLs provided or constructed

Then run delta comparison first, then full Triad synthesis.

### For Daily Update Sessions (Thursday through Tuesday)

Say: "run the daily" and Claude will automatically fetch:
- Memory record
- Daily update prompt

Then scan for signals and produce the daily update.

---

## After Each Wednesday Session — Commit Checklist

- [ ] Save SITREP output to `/sitreps/YYYY-MM-DD-issue-NNN.md`
- [ ] Copy new memory record JSON into `/memory/current-memory-record.json` (overwrite)
- [ ] Append previous week's memory record to `/memory/memory-archive.json`
- [ ] Commit all changes with message: `Issue NNN - YYYY-MM-DD`

## After Each Daily Session — Commit Checklist

- [ ] Save daily update to `/daily-updates/YYYY-MM-DD-[weekday].md`
- [ ] Commit with message: `Daily update - YYYY-MM-DD [Weekday]`
