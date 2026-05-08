# Latest Visual / Legal Output Issues (2026-05-08)

These notes capture the newest problems found after deploying `MCAContracts_Netlify_Deploy_Current_2026-05-08.zip` and generating a fresh packet.

The corresponding screenshots are also preserved inside the pickup bundle under:

- `MCA_Tomorrow_Pickup_2026-05-07/latest_user_screenshots_2026-05-08/`

## Overall rule for the next session

Do not keep trying to rescue these sections with tiny overlay patches.

If a section is unstable, rebuild that page region cleanly as a deliberate layout while preserving the exact legal meaning. The user explicitly approved redesigning ugly sections as long as the legal content stays correct.

## Problems visible in the latest screenshots

1. Broker-addendum initials page still looks sloppy.
   - File: `Screenshot 2026-05-08 at 2.29.44 PM.png`
   - The initials checklist at the top is acceptable, but the page has huge dead space and then a lonely `Seller #1` signature block dropped far down the page.
   - This needs a full page composition pass so the signature area is intentionally placed and balanced.

2. Addendum execution page still has orphaned overlay artifacts.
   - File: `Screenshot 2026-05-08 at 2.29.59 PM.png`
   - Stray `SELLER #1` and `SELLER #2` labels are floating above the real execution blocks.
   - This means older overlay behavior is still leaking through.
   - The execution area should be rebuilt as a single clean custom block.

3. Written Consent page 2 still wastes space and looks unfinished.
   - File: `Screenshot 2026-05-08 at 2.30.09 PM.png`
   - The body text ends high on the page and the owner/guarantor block sits far too low with large empty space between them.
   - This is visually weak even if the text is technically present.

4. ICC disclosure page shows a likely entity-metadata mismatch.
   - File: `Screenshot 2026-05-08 at 2.30.26 PM.png`
   - `Provider's Address` shows `Iron Crown Capital, LLC`, but `Provider's E-Mail Address` shows `submissions@EastShoreEquities.com`.
   - Treat this as a substantive configuration bug until proven otherwise.
   - The next session must verify that every entity uses the correct phone/email/address package everywhere.

5. Declaration execution page still looks under-designed.
   - File: `Screenshot 2026-05-08 at 2.30.35 PM.png`
   - The signature line exists, but the lower execution block still reads like a rough overlay rather than a polished final legal page.

6. NOA / Assignment page is improved versus older catastrophic versions, but still not professional enough.
   - File: `Screenshot 2026-05-08 at 2.30.46 PM.png`
   - The top summary block is cleaner, but the bottom signature block still dumps extra entity text under the signature area and the composition is not court-quality.
   - This section still should be treated as a deliberate redesign candidate.

7. ACH authorization / collection page still has footer/signature collision problems.
   - File: `Screenshot 2026-05-08 at 2.30.55 PM.png`
   - The `Initials:` marker is colliding with text near the bottom.
   - The seller signature region still looks cramped and mechanically overlaid.

8. Power of Attorney page still uses text that is too tiny and too dense.
   - File: `Screenshot 2026-05-08 at 2.31.05 PM.png`
   - The opening block is readable but not polished.
   - There is also an ugly broken transition before item `6`, which makes the page look like text was forced into place rather than designed.

9. Security Agreement top block still overlaps the body text below.
   - File: `Screenshot 2026-05-08 at 2.31.16 PM.png`
   - The top summary fields and the first paragraph are colliding.
   - This page is still unsafe and needs a real custom top-of-page composition.

10. Guaranty opening page still has overlapping text in the intro area.
    - File: `Screenshot 2026-05-08 at 2.31.27 PM.png`
    - Address/party text is crossing into the two-column body below.
    - This section should be rebuilt, not micro-patched.

11. Another signature-heavy page still has extreme empty space and weak composition.
    - File: `Screenshot 2026-05-08 at 2.31.41 PM.png`
    - The page is mostly blank with signature blocks floating in the lower half.
    - This is not acceptable as a world-class legal output.

12. Agreement opening / seller table is improved but still not premium.
    - File: `Screenshot 2026-05-08 at 2.31.47 PM.png`
    - The table is more stable than some other sections, but the top paragraph and table composition still feel like a patched PDF instead of a polished document.
    - This may be acceptable later, but only after the higher-risk pages are solved.

## High-priority next-session targets

These sections should be treated as the first redesign candidates:

1. `securityTop`
2. `guarantyOpening`
3. `powerOfAttorneyOpening`
4. `noaAssignment`
5. addendum execution / signature pages
6. written-consent page 2 layout
7. ACH footer/signature page

## Business-rule reminders that must stay intact

1. The legal meaning must remain exact.
2. The user does not care if the page looks different from the older sample, as long as the content is legally correct and the page looks excellent.
3. If a one-owner clause legally requires the trailing conjunction, keep it.
   - Example reminder from the user: `TULIO DAVID GONZALEZ CASTANEDA and`
4. Do not silently substitute the wrong entity metadata.
   - The ICC disclosure email mismatch must be investigated.
