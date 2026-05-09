Superseded by `PROMPT_FOR_NEXT_CODEX_CHAT_2026-05-09.md`.

Open the GitHub repo first and work only from that handoff:

- Repo: `https://github.com/BlueStoneRG-2026/MCAContracts`

Start by reading:

1. `GITHUB_START_HERE_2026-05-08.md`
2. `LATEST_VISUAL_ISSUES_2026-05-08.md`

Then download and unpack:

- `MCA_Tomorrow_Pickup_2026-05-08_final_for_laptop.zip`

Inside that bundle, the working source of truth is:

- `MCA_Tomorrow_Pickup_2026-05-07/working_deploy/`

Main files:

- `MCA_Tomorrow_Pickup_2026-05-07/working_deploy/js/app.js`
- `MCA_Tomorrow_Pickup_2026-05-07/working_deploy/js/template-config.js`

Important instructions for this session:

1. Do not continue the old patch-test-patch loop.
2. Do not hand back another deploy zip without real visual verification.
3. Preserve the exact legal meaning of every page.
4. You are allowed to redesign ugly/unstable page regions completely if needed, as long as the legal language and legal effect stay the same.
5. The output should look like a world-class professional legal packet, not a patched PDF with random overlays.
6. If a section keeps breaking because of placeholder geometry, clear the unstable region and rebuild it as a clean page-specific composition.
7. Test everything in the browser and generate real PDFs before claiming anything is fixed.

Current known priorities from the latest screenshots:

1. `securityTop` still overlaps body text.
2. `guarantyOpening` still overlaps body text.
3. `powerOfAttorneyOpening` still looks too dense and broken.
4. `noaAssignment` still is not professional enough.
5. Addendum execution pages still show sloppy/orphaned overlay artifacts.
6. Signature-heavy pages still have huge blank spaces and weak composition.
7. ICC disclosure may have a real entity-metadata bug:
   - `Provider's Address` says `Iron Crown Capital, LLC`
   - but the email shown is `submissions@EastShoreEquities.com`
   - verify all entity metadata everywhere.

Required workflow:

1. Unpack the final pickup bundle.
2. Read `notes/REPO_HANDOFF_2026-05-08.md`.
3. Read `notes/LATEST_VISUAL_ISSUES_2026-05-08.md`.
4. Use the latest screenshots in `latest_user_screenshots_2026-05-08/` as the current visual defect list.
5. Fix the worst unstable sections by deliberate redesign, not by piling on more tiny overrides.
6. Generate at least:
   - one short normal sample
   - one long-name stress sample
   - one multi-owner sample
   - one Schedule A sample
   - one example for each funder/entity if touched by the changes
7. Visually inspect the generated PDFs page by page.
8. Only then package the next deploy zip.

Success standard:

- exact legal meaning preserved
- correct entity-specific content everywhere
- no sloppy overlaps
- no orphan labels
- no random blank deserts on signature pages
- pages look polished enough that a court, merchant, broker, or account debtor would see them as professional final documents
