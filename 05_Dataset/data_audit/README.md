# Dataset audit checklist

- [ ] Verify source, version, license, and permitted use.
- [ ] Record actual image/annotation counts for the downloaded release.
- [ ] Inspect dimensions, channels, bit depth, compression, and corrupt files.
- [ ] Determine whether each image contains full-swath context or only crops.
- [ ] Record range, altitude, beam, platform, survey, and acquisition metadata availability.
- [ ] Identify group/survey IDs for leakage-safe splits.
- [ ] Inspect annotation format and consistency.
- [ ] Sample easy, weak, ambiguous, displaced, and apparently shadowless cases.
- [ ] Decide whether proposed shadow labels are feasible.
- [ ] Document exclusions before training.

Do not infer physical geometry from crop position alone.
