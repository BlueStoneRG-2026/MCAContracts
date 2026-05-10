# MCA Contracts — Start Here (2026-05-10)

This is the current handoff after the legal-content parity pass against the JLD original contract.

## Current deploy files

- `MCAContracts_Netlify_Deploy_LegalParity_2026-05-10_FINAL_VERIFIED.zip`
  - Final verified deploy package from the last JLD live/regression pass.
  - This package preserves the original legal text while removing the remaining extra generated artifacts.

- `MCAContracts_Netlify_Deploy_LegalParity_2026-05-10.zip`
  - Preferred deploy package, overwritten with the same final verified contents.
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
- Restored the pre-funding questionnaire to the original source form instead of the cleaner regenerated form.
- Corrected the pre-funding/declaration page mapping so declaration text no longer overlays the pre-funding page.
- Restored Consent and Acknowledgement of Liquidated Damages and Fees page 1 body sections, including Section 2A.
- Removed the generated “ASSIGNMENT NOTICE RECORD” / notice-title table from the Notice of Assignment page.
- Matched the Power of Attorney punctuation and `''ESE"` text pattern.
- Restored the final Broker/Addendum Seller #1 / Seller #2 execution block.
- Made Schedule A adaptive: when additional-entity EINs are blank, the table omits the EIN column and only renders populated rows, matching the JLD source structure; when EINs are supplied, the EIN-capable table is preserved.
- Kept literal extracted initials text as `Initials: _____`.

## Verification

Generated the JLD SMB sample locally and verified:

- 58-page contract packet.
- no raw template leakage (`{{`, `}}`, `undefined`, `[object Object]`) and no blank-variable legal phrases.
- `paged of this document` present and `pages of this document` absent.
- Consent page 1 Section 1 and Section 2A present.
- pre-funding original blank Business/Contact/Email and Month 1/2/3 lines present.
- pre-funding page values match the original counts and no declaration text appears on that page.
- no generated `ASSIGNMENT NOTICE RECORD` or notice-title artifact appears in the MCA packet.
- two ACH Authorization Agreement forms present.
- Terms Section 5 UCC-3 heading present.
- security agreement Section 18 numbering glitch absent.
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
