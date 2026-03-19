# MCO Spellcheck Starter Package

This starter package is aligned with the project brief for the Filipino spell-checking MCO.

## Contents

- `rules/filipino_spelling_rules.xml`: LanguageTool-compatible XML starter with 3 rule slots.
- `docs/Documentation_Template.md`: Main documentation template to convert to PDF.
- `docs/Evidence_Log_Template.csv`: Log for incorrect spelling evidence links.
- `docs/Contribution_Table_Template.md`: Group workload table template.
- `docs/AI_Declaration_Template.md`: Per-member AI usage declaration template.
- `docs/Video_Demo_Outline.md`: Suggested flow for your demo presentation.
- `docs/Submission_Checklist.md`: Final pre-submission checklist.
- `docs/Test_Sentences.md`: Ready sentence set for precision demo.

## How to use

1. Research OP and MMP and identify 3 misspelling patterns with documented incorrect forms.
2. Edit `rules/filipino_spelling_rules.xml`:
   - Replace placeholder regex patterns and suggestions.
   - Add exception handling (`<exception>` and/or regex safeguards).
   - Add 3 incorrect and 3 correct examples per rule in XML.
3. Fill all `docs/*` templates using your final rules and evidence.
4. Validate the XML in LanguageTool standalone.
5. Convert completed documentation to PDF.

## Important

- The file is intentionally safe by default and does not flag real words yet.
- Do not submit placeholder content.
- Verify every rule against OP/MMP and actual corpus evidence.
