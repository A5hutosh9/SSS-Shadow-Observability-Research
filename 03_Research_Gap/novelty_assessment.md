# Novelty assessment — living document

## Candidate gap
The candidate distinction is not simply detecting or segmenting shadows. It is estimating whether shadow evidence is assessable under local imaging conditions and conditioning target verification on that estimate.

## Evidence required
1. A reproducible operational definition of shadow observability.
2. Observable cues measurable from available image/context information.
3. Evidence that observability predicts when shadow evidence is informative.
4. Improvement over detector-only, unconditional shadow evidence, and hard-rejection baselines.
5. A documented distinction from object–shadow annotation, geometry-informed detection, shadow segmentation, and illumination-aware methods.

## Mandatory rejection tests
- If SE-OBB already estimates observability or does equivalent condition-aware verification, redefine the contribution.
- If Li et al. or Yu et al. cover the proposed question, narrow or abandon the claim.
- If dataset context/metadata are inadequate, change dataset or question.
- If observability labels cannot be annotated consistently, redesign the label definition.
- If the proposed method does not beat simpler baselines, report that honestly.

**Status: not established.** Do not claim first/novel/unprecedented until supported by a complete prior-art comparison.
