# Netlify Live Deploy Verification - 2026-05-10B

Production site: https://esedocs.tryangleai.com/
Netlify deploy ID: 6a00aa5f5e9ce4e2161d52b7
Deploy time: May 10, 2026 at 11:55 AM America/New_York

## Result

PASS - the live production site regenerated the JLD contract and passed the hard legal-content audit against:

`/Users/juanreyes/Downloads/JLD Original to compare to .pdf`

## Audit Summary

- Checks passed: 45/45
- Failed checks: 0
- Original page count: 58
- Generated page count: 58
- Generated MCA PDF: `live_jld_parity_audit_2026_05_10b/generated/JL_D_Electric_LLC_MCA_Contract_SMB.pdf`
- Generated written consent PDF: `live_jld_parity_audit_2026_05_10b/generated/JL_D_Electric_LLC_Written_Consent_SMB.pdf`
- Audit report: `live_jld_parity_audit_2026_05_10b/audit_result_2026-05-10B.md`

## Critical Checks Confirmed

- No raw template placeholders.
- No duplicate blank/populated PSFRA pass.
- No assignment notice record artifact.
- No security agreement numbering glitch.
- Seller acknowledgment mirrors source wording, including the original `paged` wording.
- PSFRA page 8 block order mirrors the original source.
- Purchase grid text and order match the source extraction.
- Seller and D/B/A Schedule A suffix text matches the source extraction.
- Entity selection row matches the source extraction.
- Account/routing text matches source extraction.
- Seller #2 and Owner/Guarantor #2 labels are present with count parity.
- Page 20 arbitration appears once and NO UCC-3 appears once.
- Guaranty continuation, arbitration, and notices are populated.
- ACH, RapidRuling, Schedule A, Broker Addendum, and final initials sections are present.

## Repo Note

The deploy zip used for this live production pass is:

`MCAContracts_Netlify_Deploy_LegalParity_2026-05-10_FINAL_VERIFIED_20260510b.zip`

GitHub was updated with the verified deploy bundle and supporting audit artifacts.
