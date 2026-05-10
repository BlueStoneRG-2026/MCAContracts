# MCA Contracts — Start Here (2026-05-10)

This is the current handoff after the legal-content parity pass against the JLD original contract.

## Current deploy files

- `MCAContracts_Netlify_Deploy_LegalParity_2026-05-10.zip`
  - Preferred deploy package.
  - Contains only the production files Netlify needs: `index.html`, `netlify.toml`, `_redirects`, `js/`, and `master/`.

- `MCAContracts_Netlify_Deploy_Final_2026-05-10.zip`
  - Same deploy contents under the existing final deploy filename.

## Source of truth

The working source remains:

- `MCA_Tomorrow_Pickup_2026-05-07/working_deploy/`

Main changed file:

- `MCA_Tomorrow_Pickup_2026-05-07/working_deploy/js/app.js`

## Legal-content parity fixes in this pass

- Preserved the original Seller Acknowledgment closing sentence exactly, including the source typo `paged`.
- Restored two-column execution architecture for blank second Seller and Owner/Guarantor slots.
- Corrected PSFRA entity checkbox association so the selected entity’s `X` is visually and textually tied to the selected entity.
- Matched the Power of Attorney punctuation and `''ESE"` text pattern.
- Restored the final Broker/Addendum Seller #1 / Seller #2 execution block.
- Made Schedule A adaptive: when additional-entity EINs are blank, the table omits the EIN column and only renders populated rows, matching the JLD source structure; when EINs are supplied, the EIN-capable table is preserved.
- Kept literal extracted initials text as `Initials: _____`.

## Verification

Generated the JLD SMB sample locally and verified:

- 58-page contract packet.
- `paged of this document` present and `pages of this document` absent.
- LLC checkbox association present; no false `Corp X Limited Liability` association.
- `OWNER/GUARANTOR #2` present.
- final `Seller: #2` block present.
- Power of Attorney punctuation pattern present.
- Schedule A no-EIN table shape present when the Schedule A row has no EIN.

Also regenerated the full 9-case acceptance matrix across ESE, ICC, and SMB packets:

- one owner / no Schedule A
- two owner / Schedule A
- duplicate-owner stress case
- multi-entity Schedule A
- multi-EIN Schedule A
- long-name stress cases

All matrix cases reported:

- `problems: []`

