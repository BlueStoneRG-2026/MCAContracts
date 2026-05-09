# MCA Contracts — Start Here (2026-05-09)

This is the current handoff after the 2026-05-09 visual/legal QA pass.

## Current deploy file

- `MCAContracts_Netlify_Deploy_Current_2026-05-09.zip`
  - Deploy this package to Netlify.
  - It contains only the app files needed for production: `index.html`, `netlify.toml`, `_redirects`, `js/`, and `master/`.

## Current recovery bundle

- `MCA_Tomorrow_Pickup_2026-05-09_final_verified.zip`
  - Contains the clean `working_deploy/` source of truth, the deploy zip, final notes, QA logs, high-risk visual review sheets, and generated sample PDFs.

Inside that bundle, the source of truth remains:

- `MCA_Tomorrow_Pickup_2026-05-07/working_deploy/`

Main files:

- `MCA_Tomorrow_Pickup_2026-05-07/working_deploy/js/app.js`
- `MCA_Tomorrow_Pickup_2026-05-07/working_deploy/js/template-config.js`

## What changed in the final pass

- Rebuilt the Agreement Seller / D/B/A / entity information block as a clean custom table so placeholder boxes no longer cover rules.
- Redesigned the NOA into a more formal notice page while preserving the operative assignment language.
- Fixed the Security Agreement opening overlap.
- Tightened POA, Authorization, Schedule A, pre-funding questionnaire, disclosure, and signature-heavy page compositions.
- Clarified EIN entry: primary Seller EIN goes in the primary Seller EIN field; additional entity EINs go in their own Schedule A rows.
- Verified ICC metadata: ICC disclosure intentionally uses `submissions@EastShoreEquities.com`, matching the real sample contracts provided.

## QA status

Generated and reviewed real PDFs in browser automation across 9 scenarios:

- one owner / no Schedule A
- two owners / long names / Schedule A
- duplicate-owner stress case
- one Schedule A entity
- three Schedule A entities
- multi-EIN Schedule A
- ESE, ICC, and SMB funder packets

The final acceptance matrix reported `problems: []` for every scenario.

