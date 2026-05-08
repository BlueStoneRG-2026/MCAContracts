# MCA Contracts — Start Here (2026-05-08)

This repo is being used as the cross-computer handoff point for the MCA contract tool project.

## Start with these files

- `MCA_Tomorrow_Pickup_2026-05-08_final_for_laptop.zip`
  - Full recovery bundle.
  - Contains the current `working_deploy/`, historical artifacts, latest screenshots from 2026-05-08, updated handoff notes, and the next-session prompt.
- `MCAContracts_Netlify_Deploy_Current_2026-05-08.zip`
  - The current deployable Netlify package as of 2026-05-08.
- `LATEST_VISUAL_ISSUES_2026-05-08.md`
  - The newest visual/substantive defect list from the latest generated packet.
- `PROMPT_FOR_NEXT_CODEX_CHAT_2026-05-08.md`
  - Copy-paste this into the next Codex chat on the laptop.

## What is the actual working source?

Inside `MCA_Tomorrow_Pickup_2026-05-08_final_for_laptop.zip`, the source of truth is:

- `MCA_Tomorrow_Pickup_2026-05-07/working_deploy/`

Main file:

- `MCA_Tomorrow_Pickup_2026-05-07/working_deploy/js/app.js`

## Important status

This project is **not signed off**.

The tool improved in some places, but several redesign / overlay attempts also made specific pages worse. The next session should not continue with random patching. The correct next move is to open the pickup bundle, read the handoff note, review the newest screenshots/issues note, and then deliberately rebuild the worst unstable sections with full visual verification.

## Most important note to read first

Inside the pickup bundle, read:

- `MCA_Tomorrow_Pickup_2026-05-07/notes/REPO_HANDOFF_2026-05-08.md`
- `MCA_Tomorrow_Pickup_2026-05-07/notes/LATEST_VISUAL_ISSUES_2026-05-08.md`
- `MCA_Tomorrow_Pickup_2026-05-07/notes/PROMPT_FOR_NEXT_CODEX_CHAT_2026-05-08.md`

That note explains:

- what changed after the older pickup bundle
- what sections are still unsafe
- what not to repeat
- what the next session should do first

## Core instruction for the next Codex session

Do **not** assume the latest deploy is good.

Do **not** trust old screenshots without checking newer generated PDFs.

Do **not** keep stacking custom overrides blindly.

Instead:

1. unpack the pickup bundle
2. open the updated handoff note
3. work from `working_deploy/`
4. regenerate sample PDFs
5. visually verify every bad section before calling anything fixed
6. do not be afraid to fully redesign ugly page regions if the legal meaning stays exact
