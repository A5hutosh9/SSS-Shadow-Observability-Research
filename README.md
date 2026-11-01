# Observability-Conditioned Acoustic-Shadow Evidence for Side-Scan Sonar Target Verification

> **Status:** provisional research direction. Novelty and feasibility are not yet established; complete the critical prior-art and dataset audits before making a novelty claim.

## Research question

Can a side-scan sonar (SSS) system estimate whether a target's acoustic shadow should be observable under current imaging conditions, then distinguish an unobservable shadow from genuinely inconsistent or absent shadow evidence?

## Proposed investigation

Study target detection, local image-quality/context cues, shadow candidate extraction, shadow-observability estimation, target–shadow association, and observability-conditioned verification.

The hypothesis is that a weak or missing shadow should not automatically count as negative evidence when local conditions make that shadow difficult to assess. Compare against detector-only, unconditional shadow matching, and hard shadow rejection. This is a hypothesis, not a proven contribution.

## Provisional notation

For detection i: detector confidence p_i; observability estimate O_i; signed shadow-association evidence M_i; local quality/context features Q_i; correctness label Y_i. A candidate evidence term is E_i = O_i × M_i. This formulation is provisional. Define O_i operationally, justify all inputs, and test whether it predicts when shadow evidence is informative. Do not claim calibrated probabilities or formal guarantees without validation.

## Candidate dataset

MILCO/NOMBO: Santos et al. (2024), *Data in Brief*, DOI [10.1016/j.dib.2024.110132](https://doi.org/10.1016/j.dib.2024.110132); dataset DOI [10.6084/m9.figshare.24574879](https://doi.org/10.6084/m9.figshare.24574879). Reported collection: 1,170 real SSS images and 668 annotated objects. Published labels are object boxes, not shadow-observability annotations. Audit license, image context, image quality, metadata, and survey grouping before training. Do not infer physical range or geometry from crop position alone.

## Critical prior-art checks

- Li et al. (2025), “Side-scan sonar mine-like target detection considering acoustic illumination and shadow characteristics,” *Ocean Engineering*. [DOI](https://doi.org/10.1016/j.oceaneng.2025.121711)
- Yu et al. (2026), “Physics-Informed Side-Scan Sonar Perception: Tackling Weak Targets and Sparse Debris via Geometric and Frequency Decoupling,” *Sensors*. [DOI](https://doi.org/10.3390/s26061938)
- Lee et al. (2026), “SE-OBB: Structure-Aware Object-Shadow Annotation for Robust Object Detection in Side-Scan Sonar Imagery.” [DOI](https://doi.org/10.22761/GD.2026.0049)
- Si et al. (2025), “An Unsupervised Method for Detecting and Segmenting Shadow Areas of Sunken Targets in Sonar Images,” *IEEE Transactions on Instrumentation and Measurement*. [DOI](https://doi.org/10.1109/TIM.2025.3527611)
- Lei et al. (2026), “PhysDNet: Physics-Guided Decomposition Network of Side-Scan Sonar Imagery,” *IEEE Geoscience and Remote Sensing Letters*. [DOI](https://doi.org/10.1109/LGRS.2026.3704815)
- Park and Bae (2025), *Journal of Marine Science and Engineering*. [DOI](https://doi.org/10.3390/jmse13020242)
- Grządziel (2023), *Remote Sensing*. [DOI](https://doi.org/10.3390/rs15235599)

Generic shadow detection, segmentation, object–shadow association, and geometry-informed shadow use already exist. Specifically test whether SE-OBB, Li et al., and Yu et al. already cover observability-conditioned verification. If so, narrow or change the question.

## Comparisons and evaluation

Compare (A) detector only, (B) detector plus unconditional shadow score, (C) detector with hard shadow rejection, and (D) proposed observability-conditioned evidence. Evaluate precision, recall, mAP@0.5, mAP@0.5:0.95, false positives per image/swath, difficult-subset recall, Brier score, ECE, reliability diagrams, and risk–coverage. Use group-aware train/validation/calibration/test splits where metadata supports them. Report uncertainty intervals and multiple seeds where feasible. Pilot annotations should distinguish visible, weak, ambiguous, displaced, unobservable, not-assessable, and no-shadow-evidence cases; assess inter-annotator agreement.

## Two-person workflow

Person A leads SSS fundamentals, dataset audit, split proposal, detector-only baseline, and conventional shadow extraction. Person B leads full-text prior-art matrix, annotation protocol, observability/reliability design, metrics, and statistics. Both independently annotate a shared pilot subset and challenge the novelty claim.

## Research integrity

- A title/abstract is not a substitute for full-text review.
- Do not claim “first,” “novel,” or “unprecedented” until a documented prior-art comparison supports it.
- Do not redistribute copyrighted PDFs without permission; use DOI/official links when needed.
- Do not commit raw dataset files unless the license permits redistribution.
- Keep data splits, seeds, configurations, preprocessing, and negative results documented.

## Immediate next actions

1. Obtain and review the critical papers in full text.
2. Audit MILCO/NOMBO source, license, metadata, image context, and survey grouping.
3. Pilot the annotation scheme and measure agreement.
4. Decide whether observability is measurable and distinct before substantial model training.
5. Establish reproducible baseline comparisons.

## Repository structure

The repository is organized into research papers (split between two researchers), literature review, research gap, sonar fundamentals, dataset audit, annotations, baseline models, proposed method, experiments, results, manuscript, presentations, project management, and reproducibility. See the folders for checklists and templates.
