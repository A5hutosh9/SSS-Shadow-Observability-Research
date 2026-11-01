# Researcher 1 — Sonar physics, shadow structure, and SSS evidence

**Role:** Domain and signal-processing lead.

## Primary reading order
1. **Grządziel (2023)** — *The Impact of Side-Scan Sonar Resolution and Acoustic Shadow Phenomenon on the Quality of Sonar Images*. Resolution-dependent shadow interpretation.
2. **Si et al. (2025)** — *An Unsupervised Method for Detecting and Segmenting Shadow Areas of Sunken Targets in Sonar Images*. Critical direct prior art for shadow segmentation.
3. **Lee et al. (2026)** — *SE-OBB: Structure-Aware Object-Shadow Annotation for Robust Object Detection in Side-Scan Sonar Imagery*. Critical novelty threat; study annotation representation and post-processing.
4. **Yu et al. (2026)** — *Physics-Informed Side-Scan Sonar Perception: Tackling Weak Targets and Sparse Debris via Geometric and Frequency Decoupling*. Critical physics-informed/shadow-geometry prior art.
5. **Wang et al. (2024)** — *A Novel Target Detection Method with Dual-Domain Multi-Frequency Feature in Side-Scan Sonar Images*.
6. **Tang et al. (2023)** — *AUV-Based Side-Scan Sonar Real-Time Method for Underwater-Target Detection*.
7. **Yang et al. (2022)** — *Semantic Segmentation of Side-Scan Sonar Images with Few Samples*.
8. **Yang et al. (2022)** — *Side-Scan Sonar Image Segmentation Based on Multi-Channel CNN for AUV Navigation*.
9. **Sethuraman et al. (2025)** — *Machine Learning for Shipwreck Segmentation from Side Scan Sonar Imagery: Dataset and Benchmark*.
10. **Yang et al. (2024)** — *Side-Scan Sonar Image Matching Method Based on Topology Representation*.
11. **Liu et al. (2023)** — *An Image Quality Improvement Method in Side-Scan Sonar Based on Deconvolution*.
12. **Motylinski et al. (2025)** — *Computer Vision Methods for Side Scan Sonar Imagery* (review).
13. **Qiao et al. (2026)** — *AUVs for Seabed Surveying: A Comprehensive Review of Side-Scan Sonar-Based Target Detection* (review).

## Shared mandatory reading (both researchers)
- Li et al. (2025), *Side-scan sonar mine-like target detection considering acoustic illumination and shadow characteristics* — full text required; major novelty threat.
- Yu et al. (2026), *Physics-Informed Side-Scan Sonar Perception*.
- Lee et al. (2026), *SE-OBB*.
- Si et al. (2025), shadow segmentation.
- Park & Bae (2025), DOI 10.3390/jmse13020242 — far-range shadow visibility / beam-pattern effects; full text required.

## Deliverables
- 2–3 page SSS physics note: beam direction, slant range, grazing angle, altitude, object height, shadow formation, beam-pattern effects, resolution, speckle/reverberation.
- Dataset audit: identify image context needed to assess a shadow; do not infer physical range from crop position alone.
- Pilot annotation guide for visible / weak / ambiguous / displaced / unobservable / not-assessable shadow states.
- Annotate at least 50 difficult examples jointly with Researcher 2; report agreement and adjudication rules.
- Baseline highlight/shadow extraction and qualitative failure gallery.

For every paper record exact citation/DOI, modality (SSS/SAS/FLS/other), dataset, labels, geometry assumptions, shadow representation, limitations, and what it does **not** establish.
