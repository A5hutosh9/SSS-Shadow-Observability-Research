# Researcher 2 — Observability, uncertainty, calibration, and evaluation

**Role:** Statistical and method lead.

## Primary reading order
1. **Andéol et al. (2023)** — *Confident Object Detection via Conformal Prediction and Conformal Risk Control: an Application to Railway Signaling*. Transferable conformal object-detection setup; note assumptions and calibration split.
2. **Angelopoulos et al. (2025 version)** — *Conformal Risk Control*. Understand bounded monotone loss requirements and finite-sample guarantee assumptions.
3. **Mallick et al. (2021)** — *Forward-Looking Sonar Patch Matching: Modern CNNs, Ensembling, and Uncertainty*. Sonar-specific uncertainty, but FLS rather than SSS.
4. **Basha et al. (2026)** — *An Explainable Context-Adaptive Fusion and Expert-in-the-Loop Evaluation Framework for Underwater Sonar Image Classification*. Strong prior art for context-adaptive shadow/highlight fusion; classification rather than target verification.
5. **Natarajan & Nambiar (2024)** — *Underwater SONAR Image Classification and Analysis using LIME-based Explainable Artificial Intelligence*. XAI context; classification rather than detection.
6. **Xiao et al. (2025)** — *CKAN-YOLOv8: A Lightweight Multi-Task Network for Underwater Target Detection and Segmentation in Side-Scan Sonar Images*.
7. **Xie et al. (2026)** — *Ultra-Fast Object Detection for Side-Scan Sonar Images via Target Presence Awareness*.
8. **Zou et al. (2025)** — *Side-Scan Sonar Small Objects Detection Based on Improved YOLOv11*.
9. **Wen et al. (2024)** — *Underwater Side-Scan Sonar Target Detection: YOLOv7 Model Combined with Attention Mechanism and ...* (large PDF; verify full title on first page).
10. **Yu (2022)** — *Sonar Image Target Detection Based on Deep Learning* (broad sonar; check modality).
11. **Zhu et al. (2024)** — *Side-Scan Sonar Image Augmentation Method Based on CC-WGAN*.
12. **Yang & Zhang (2026)** — *Diffusion-Model-Based Data Augmentation for Target Detection in Side-Scan Sonar Images*.
13. **2608.24756v1** — weakly supervised seafloor segmentation for seagrass habitat mapping in SSS (verify final title/authors and preprint status).
14. **Palomeras et al. (2022)** — *Automatic Target Recognition for Mine Countermeasure Missions Using Forward-Looking Sonar Data* (FLS; contextual only).

## Shared mandatory reading (both researchers)
- Li et al. (2025), *Side-scan sonar mine-like target detection considering acoustic illumination and shadow characteristics*.
- Yu et al. (2026), *Physics-Informed Side-Scan Sonar Perception*.
- Lee et al. (2026), *SE-OBB*.
- Si et al. (2025), shadow segmentation.
- Park & Bae (2025), DOI 10.3390/jmse13020242.

## Deliverables
- Formal definition of shadow observability, target-level labels, and the distinction between unobservable and absent/inconsistent.
- Candidate observability estimator and ablation plan; no arbitrary multiplier without validation.
- Reliability evaluation plan: Brier score, ECE, reliability diagrams, risk–coverage, review fraction, subgroup results.
- Group-aware train/calibration/test split proposal to prevent survey leakage.
- Statistical protocol: confidence intervals, multiple seeds, annotation agreement, and limitations of exchangeability under domain shift.

For every method, state precise assumptions and whether it has a theorem, an empirical result, or only a proposed design. Do not claim conformal guarantees unless calibration and exchangeability assumptions are satisfied.
