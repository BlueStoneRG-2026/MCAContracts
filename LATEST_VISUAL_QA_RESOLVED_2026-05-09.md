# Latest Visual QA Status — Resolved Build (2026-05-09)

The latest verified deploy package is:

- `MCAContracts_Netlify_Deploy_Current_2026-05-09.zip`

## Resolved priority issues

1. `securityTop` overlap: resolved.
2. `guarantyOpening` overlap / dense opening: improved and verified in stress packets.
3. `powerOfAttorneyOpening` density: rebuilt to fit more cleanly while preserving legal content.
4. `noaAssignment` professionalism: redesigned as a formal Notice of Assignment record and letter.
5. Addendum execution artifacts: custom signature compositions verified on high-risk pages.
6. Signature-heavy blank-space pages: tightened and rebalanced where controlled by custom rendering.
7. ICC entity metadata: verified against supplied real-life samples. ICC uses Iron Crown Capital, LLC with `submissions@EastShoreEquities.com`.
8. Agreement first table white-box artifacts: replaced with a clean custom information grid.
9. Multiple EIN handling: primary Seller EIN remains separate; Schedule A entity EINs are entered one per entity row.
10. Sales-Based Financing Disclosure value alignment: rebuilt the first disclosure page as a clean table so Provider E-Mail, Total Amount, Fees Deducted, Disbursement Amount, Finance Charge, Total Repayment Amount, Total Cost, Estimated Number of Payments, and Payment Schedule values all render in their own cells without overlay artifacts.

## Final QA matrix

The final browser-generated PDF matrix covered:

- ESE one owner, no Schedule A
- ESE two owners, long legal names, three Schedule A entities, multi-EIN
- ESE duplicate owner, three Schedule A entities
- ICC one owner, no Schedule A
- ICC two owners, one Schedule A entity with blank additional-entity EIN
- ICC three Schedule A entities, multi-EIN
- SMB one owner, sole prop, no Schedule A
- SMB two owners, partnership, Schedule A
- SMB LLP stress case, two owners, three Schedule A entities

All nine scenarios produced `problems: []` in the QA log and were visually reviewed through generated page PNGs / high-risk review sheets.

After the disclosure-table rebuild, the same nine-scenario matrix was generated again locally from the patched deploy source. All nine scenarios again produced `problems: []`, and the ESE/ICC/SMB high-risk sheets were re-reviewed.
