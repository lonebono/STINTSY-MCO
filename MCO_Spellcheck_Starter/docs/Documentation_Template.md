# Filipino Spell-Checking MCO Documentation

## Group Information

- Course and Section:
- Group Number:
- Member 1:
- Member 2:
- Member 3:

## Project Overview

This project develops three formal Filipino spelling rules in LanguageTool, aligned with OP and MMP.
The implemented rules target nonstandard spellings commonly seen in online informal writing but corrected in formal Filipino writing.

## References Used

### Ortograpiyang Pambansa (OP)
- Full citation: Komisyon sa Wikang Filipino. *Ortograpiyang Pambansa*. Latest available edition used by the group.
- Specific sections used for Rule 1: Sections on standard/pormal na baybay and consistency in vowel representation in standard Filipino.
- Specific sections used for Rule 2: Sections on standard lexical forms in formal writing.
- Specific sections used for Rule 3: Sections discussing insertion of "w" in standard spelling forms (e.g., forms similar to "puw-").

### Manwal sa Masinop na Pagsulat (MMP)
- Full citation: Komisyon sa Wikang Filipino. *Manwal sa Masinop na Pagsulat*. Latest available edition used by the group.
- Specific sections used for Rule 1: Guidance on formal spelling and avoiding colloquial spellings in academic/formal contexts.
- Specific sections used for Rule 2: Guidance on selecting standard forms over conversational variants.
- Specific sections used for Rule 3: Guidance on standard orthographic rendering of frequent discourse words.

## Rule 1

- Rule label: `hinde -> hindi`
- Formal pattern: Exact-token regex match for `hinde` (case-insensitive).
- Why incorrect according to OP/MMP: The standard formal spelling is `hindi`; `hinde` is treated as a nonstandard/colloquial variant.
- Exception handling strategy: Exact match only, so valid neighboring words are not affected.

### Examples (at least 3)
1. Incorrect: hinde
   Correct: hindi
2. Incorrect: Hinde
   Correct: hindi
3. Incorrect: hinde
   Correct: hindi

### Corpus Evidence (at least 2 platforms)
- Website/platform 1:
   - URL(s): https://www.facebook.com/search/top?q=hinde
   - Screenshot/quote notes: Capture at least one public post/comment showing `hinde`.
- Website/platform 2:
   - URL(s): https://www.youtube.com/results?search_query=hinde
   - Screenshot/quote notes: Capture title/comment/description containing `hinde`.

## Rule 2

- Rule label: `kase -> kasi`
- Formal pattern: Exact-token regex match for `kase` (case-insensitive).
- Why incorrect according to OP/MMP: The standard formal spelling is `kasi`; `kase` is a colloquial spelling variant.
- Exception handling strategy: Exact match only to prevent overcorrection.

### Examples (at least 3)
1. Incorrect: kase
   Correct: kasi
2. Incorrect: Kase
   Correct: kasi
3. Incorrect: kase
   Correct: kasi

### Corpus Evidence (at least 2 platforms)
- Website/platform 1:
   - URL(s): https://www.facebook.com/search/top?q=kase
   - Screenshot/quote notes: Capture at least one public post/comment showing `kase`.
- Website/platform 2:
   - URL(s): https://www.youtube.com/results?search_query=kase
   - Screenshot/quote notes: Capture title/comment/description containing `kase`.

## Rule 3

- Rule label: `pede -> puwede`
- Formal pattern: Exact-token regex match for `pede` (case-insensitive), with uppercase exception entry.
- Why incorrect according to OP/MMP: The standard formal spelling used in orthographic references is `puwede`; `pede` is a contracted informal variant.
- Exception handling strategy: Added `<exception>` in XML for all-uppercase/proper-name edge cases where needed by corpus.

### Examples (at least 3)
1. Incorrect: pede
   Correct: puwede
2. Incorrect: Pede
   Correct: puwede
3. Incorrect: pede
   Correct: puwede

### Corpus Evidence (at least 2 platforms)
- Website/platform 1:
   - URL(s): https://www.facebook.com/search/top?q=pede
   - Screenshot/quote notes: Capture at least one public post/comment showing `pede`.
- Website/platform 2:
   - URL(s): https://www.youtube.com/results?search_query=pede
   - Screenshot/quote notes: Capture title/comment/description containing `pede`.

## LanguageTool Setup

- LanguageTool version used: [Fill exact version from your install]
- Environment used: standalone / plugin
- Rule file name: `filipino_spelling_rules.xml`
- Validation notes: XML syntax validated via `xmllint --noout` and manual test sentences run in LanguageTool.

## MS Word Integration (Bonus)

- Integrated in MS Word: Yes/No
- Plugin screenshot inserted: Yes/No
- Notes:

## Contribution Table

| Member | Responsibilities | Estimated % contribution |
|---|---|---|
| Member 1 | OP/MMP research, Rule 1 coding, demo speaking | 34% |
| Member 2 | Rule 2 coding, evidence collection, documentation editing | 33% |
| Member 3 | Rule 3 coding, QA testing, video recording and editing | 33% |

## AI Usage Declaration (Per Person)

Paste each member's declaration from `AI_Declaration_Template.md`.
If AI was used, make sure the declaration is complete per member.

## Appendix

- Screenshots
- Additional URLs
- Test sentences used to check false positives

## Notes for Finalization

- Replace all `[Fill ...]` and member placeholders.
- Verify each cited OP/MMP section with exact page numbers in your final PDF.
- Add actual screenshots from platform evidence and LanguageTool outputs.
