# Scoring rubric

Score each listed check **Pass (1)** or **Fail (0)** for each approach, using the same input and the same check. Judge only what the output says and the supplied transcript/visual evidence. Record the reason for every failure in `scorecard.csv`.

| Code | What passes |
|---|---|
| **A** | Documented actions, sequence, and final state match the available evidence. |
| **I** | Explicit purpose and constraints are preserved; intended outcomes are not presented as observed facts. |
| **H** | The failure/recovery or later correction is captured, including which state/action is final. |
| **G** | Material claims are tied to a timestamp/screenshot or transcript evidence; missing confirmation is stated; unsupported claims are absent. |

## Report these results
1. For each category, report `passed checks / applicable checks` and the percentage. Denominators are derived from the checks in `evaluation_set.json`: **A 7, I 4, H 3, G 5** (19 total checks).
2. Report the overall result as `passed checks / 19`. Also list every failed check and any extra unsupported claim not explicitly covered by a check. Treat a single unsupported completion/delivery claim in IT-04 as a failure of IT-04-G2, even if other checks pass.
3. Compare the two approaches on the exact same four cases. Include the raw counts, not percentages alone. This tiny synthetic set supports case-level observations only, not statistical significance or general claims about real users/product performance.

## Fairness and handling ambiguity
- Freeze this rubric before running either approach.
- Score both outputs independently against the same checks.
- A check fails if a required fact is materially wrong or missing. Minor wording differences do not fail a check.
- If an output adds a material claim not supported by the transcript or visual evidence, mark the relevant **G** check failed and note the claim.
- Do not give credit for facts that appear only in the expected outcome; the runtime input is the transcript and recorded visual evidence. Expected outcomes are evaluator-only references.
- No scores or results have been produced yet.
