# Method decisions

Maintain a dated decision log; every design choice needs a reason and a planned test.

## Candidate pipeline
1. Detect candidate target.
2. Extract local image/context features Q_i.
3. Generate shadow candidates and association evidence M_i.
4. Estimate observability O_i using only permitted available evidence.
5. Form conditioned evidence (initial candidate: E_i = O_i × M_i).
6. Verify/calibrate using detector confidence and evidence features.

## Open questions
- What operationally makes a shadow observable?
- Which cues exist and can be reliably measured in the dataset?
- Are separate observability labels needed?
- How will ambiguity and annotator disagreement be handled?
- Is O_i a probability, ordinal score, or binary estimate?
- How will label leakage be prevented?
- What alternatives to E_i = O_i × M_i should be tested?
- What operating point balances false positives and missed targets?

## Change log
| Date | Decision | Evidence | Owner |
|---|---|---|---|
| YYYY-MM-DD | Initial candidate pipeline | Pending audit | Both |
