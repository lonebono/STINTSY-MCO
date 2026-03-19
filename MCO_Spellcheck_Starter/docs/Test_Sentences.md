# Precision Test Sentences

Use these in LanguageTool to demonstrate that incorrect forms are flagged and standard forms are not flagged.

## Should be flagged

1. Hinde ako makakasama mamaya.
2. Uuwi na ako kase gabi na.
3. Pede po bang humingi ng extension?
4. Hinde pa raw tapos ang report.
5. Kase umulan, hindi kami natuloy.
6. Pede na ba kaming pumasok?

## Should not be flagged

1. Hindi ako makakasama mamaya.
2. Uuwi na ako kasi gabi na.
3. Puwede po bang humingi ng extension?
4. Hindi pa raw tapos ang report.
5. Kasi umulan, hindi kami natuloy.
6. Puwede na ba kaming pumasok?

## Mixed paragraph for demo

Hinde raw siya sasama kase pagod pa siya. Pede pa rin naman siyang humabol mamaya.

Expected: 3 flags (`Hinde`, `kase`, `Pede`) and suggestions (`hindi`, `kasi`, `puwede`).
