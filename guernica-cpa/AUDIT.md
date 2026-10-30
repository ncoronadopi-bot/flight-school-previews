# Guernica & Associates, CPA: design audit and redesign

Audited: https://www.guernicacpa.com/ (homepage plus the Accounting & Auditing, Taxation, Payroll and About pages), 30 Oct 2026.

Tool: tasteskill v2, installed with `npx skills add Leonxlnx/taste-skill` (skill `design-taste-frontend`), using its browser inspector at 1440, 768 and 390px, its lint, its direction draw and its juror critique.

## Verdict

The current site hides an accounting and audit practice behind a stock tax-form photo, an off-topic headline ("Business Advisory Solutions") and a layout that does not work on phones. The redesign leads with what the firm actually signs (compilations, reviews and audits) and uses only the firm's own published content.

| | Before | After |
| --- | --- | --- |
| Inspector result | 8 FAIL, 5 WARN | 0 FAIL, 1 WARN |
| Juror score (of 10) | 4.3 | 7.5 |
| Phone layout | Desktop page shrunk to 980px; tablet scrolls sideways 212px | Own phone composition, no sideways scroll |
| First-screen title | "Business Advisory Solutions" under a "Taxation Specialists" label | "Accounting & audit since 1998" |
| Primary action on first screen | None | "Book a consultation" button and phone number |
| Typefaces | 3 (Open Sans, Raleway, Georgia) | 1 (Archivo) |
| Text shadows | 23 | 0 |
| Unreadable text (measured) | 4 blocks at 1:1 contrast | 0 |
| Peer review "Pass" | A bare "Peer Review Report:" label on an inner page | On the first screen, the services panel and the credentials |

![Before, desktop](audit/before-desktop.jpg) ![After, desktop](audit/after-desktop.jpg)

## What is wrong today (ranked)

1. **Not mobile-ready.** The page renders at 980px on a 390px phone. At tablet width it scrolls sideways and the "CPA" title is half covered.
2. **The wrong story.** The hero is a 2007 IRS Form 1040 with a calculator and says "Taxation Specialists". The firm's own pages say its core is accounting and audit.
3. **No clear next step.** No button above the fold. The only actions are three identical "More Info" buttons.
4. **Best proof is buried.** The firm passed its most recent peer review (System Review, year ended Dec 31, 2022) and is an IRS Certifying Acceptance Agent. Neither appears on the homepage.
5. **Team page errors.** On the About page, bios sit under the wrong names (the "Anita" bio is under Loreli Mendez, Loreli's bio is under Esmeralda Valdes), and "Certified Puplic Accountant" is misspelled. For an audit firm, that undercuts trust.
6. **Template look and legibility.** Identical navy cards with centred small text, 23 text shadows, three typefaces, body text at 1.2 line height.

## The redesign

- **Idea:** the three levels of assurance the firm signs (compilation, review, audit) become a working engagement picker on the first screen.
- **Live thing:** "Who is asking for your financial statements?" Pick bank, investors, captive insurance regulator, board, or just you. It shows the engagement, the assurance level, what the CPA does, the report wording, and a link to ask. One tap switches it to Spanish.
- **Signature move:** "Accounting & auditing" pins the firm's own 14-item service list and highlights it in three groups as you scroll: statements for lenders, controls for boards, starting or buying a business.
- **All content from the firm:** the 14 accounting and audit services, six tax services, 12 payroll items, six team members and titles, the peer review rating with a link to the report, and the IRS acceptance agent status.
- **Brand kept:** navy and logo blue; the notched chevron from the door sign and logo is the one shape used across the page.
- **Direction dealt:** "The product performs" (seed 1757103226), palette kept from the brand. The hero follows the direction's composition (headline left, working fragment right) instead of the dealt "sentence split by a frame" hero, because the direction outranks the hero blueprint.

## Critique, final round

```
ROUND 3
Seen in one second: "Accounting & audit since 1998" beside a working report picker
Idea (one sentence): the three levels of assurance become a picker that answers "which report do I need?"
Live thing: bilingual engagement picker (5 situations, EN/ES)
Layout words by section: hero=split+fragment / accounting=pinned list / tax=shaped photo+points / people=two lists / place=full-bleed photo / about=letter on ledger / proof=tiles / contact=band / footer=strip
Scores: design 7 · usability 8 · creativity 7 · content 8.5 → overall 7.5
Caps applied: creativity capped at 7 (another audit firm could use a similar picker; bilingual and captive content make it specific, not unique)
```

Still short: no video (no honest footage of the firm's work exists), and there is no photo of the team. A real team photo would lift the "Who we work with" section most.

## Confirm with the firm before launch

- **Picker wording.** The report excerpts follow standard AICPA report language. The firm should approve each situation's advice (especially loan covenants and captive insurers) and the Spanish text.
- **Team titles.** Names and titles are copied from the About page, which has the mismatched bios noted above. Confirm each title.
- **Concept banner.** The top bar says this is a redesign concept, not the official site. Remove it only when the firm adopts the design.
- **Credits.** Two photos are CC BY-SA 4.0 and are credited in the footer. Keep the credit line if they stay.

## Files

- `index.html`: the redesigned homepage (single file, no build step)
- `img/`: the firm's own logo, office photos and credential badges, taken from the current site
- `assets/`: open-licence photos with `credits.json`
- `audit/`: before and after screenshots
