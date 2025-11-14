# Papers in this repository

This Papers.md indexes curated papers and notes stored in the papers/ directory of this repository. The goals are:

- Provide a clear inventory of available PDFs with direct links.
- Give concise one-paragraph summaries and tags for quick discovery.
- Suggest a recommended reading order and topical grouping.
- Explain how to use these files, contribution guidelines, and citation guidance.

---

Table of contents
- Files in this folder (with links)
- Summaries and tags
- Recommended reading order and topics
- How to use these files
- How to contribute
- Citation & license notes
- TODOs / suggested follow-ups

---

Files in this folder

- Continual Learning - 14062025.pdf  
  https://github.com/PenguAKAuseless/Continual-Learning-Research/blob/8c56b0dc4302d7a1c0cda8d0d434be24746a3e4e/papers/Continual%20Learning%20-%2014062025.pdf

- DINOv3.pdf  
  https://github.com/PenguAKAuseless/Continual-Learning-Research/blob/8c56b0dc4302d7a1c0cda8d0d434be24746a3e4e/papers/DINOv3.pdf

- Energy-based OOD Detection.pdf  
  https://github.com/PenguAKAuseless/Continual-Learning-Research/blob/8c56b0dc4302d7a1c0cda8d0d434be24746a3e4e/papers/Energy-based%20OOD%20Detection.pdf

- Mahalanobis Distance based OOD Detection.pdf  
  https://github.com/PenguAKAuseless/Continual-Learning-Research/blob/8c56b0dc4302d7a1c0cda8d0d434be24746a3e4e/papers/Mahalanobis%20Distance%20based%20OOD%20Detection.pdf

- NL.pdf  
  https://github.com/PenguAKAuseless/Continual-Learning-Research/blob/8c56b0dc4302d7a1c0cda8d0d434be24746a3e4e/papers/NL.pdf

- NeurIPS-2019-gradient-based-sample-selection-for-online-continual-learning-Paper.pdf  
  https://github.com/PenguAKAuseless/Continual-Learning-Research/blob/8c56b0dc4302d7a1c0cda8d0d434be24746a3e4e/papers/NeurIPS-2019-gradient-based-sample-selection-for-online-continual-learning-Paper.pdf

- Online-LoRA.pdf  
  https://github.com/PenguAKAuseless/Continual-Learning-Research/blob/8c56b0dc4302d7a1c0cda8d0d434be24746a3e4e/papers/Online-LoRA.pdf

- Softmax-based OOD Detection.pdf  
  https://github.com/PenguAKAuseless/Continual-Learning-Research/blob/8c56b0dc4302d7a1c0cda8d0d434be24746a3e4e/papers/Softmax-based%20OOD%20Detection.pdf

- Tiwari_GCR_Gradient_Coreset_Based_Replay_Buffer_Selection_for_Continual_Learning_CVPR_2022_paper.pdf  
  https://github.com/PenguAKAuseless/Continual-Learning-Research/blob/8c56b0dc4302d7a1c0cda8d0d434be24746a3e4e/papers/Tiwari_GCR_Gradient_Coreset_Based_Replay_Buffer_Selection_for_Continual_Learning_CVPR_2022_paper.pdf

---

Summaries and tags

- Continual Learning - 14062025.pdf  
  Summary: A dated set of overview notes or a primer on continual learning (likely lecture notes or a survey-style writeup). Good starting point for terminology, evaluation protocol, and taxonomy.  
  Tags: overview, primer, survey, evaluation

- DINOv3.pdf  
  Summary: Latest DINO family self-supervised visual representation learning work. Not a continual-learning method, but highly relevant as a modern, robust backbone used in continual learning experiments (feature quality matters for forgetting).  
  Tags: self-supervised, representation learning, backbone

- Energy-based OOD Detection.pdf  
  Summary: Energy-based scoring for out-of-distribution detection. Presents how energy from model logits (or logits-derived functions) can be used to detect OOD inputs and distribution shifts — useful for continual-learning systems that must detect novel classes or domain shifts.  
  Tags: OOD, detection, robustness, energy score

- Mahalanobis Distance based OOD Detection.pdf  
  Summary: OOD detection via Mahalanobis distance in feature space using class-conditional Gaussian approximations. A strong classical baseline for distinguishing in-distribution vs out-of-distribution samples in many vision settings.  
  Tags: OOD, classical baseline, statistical distance

- NL.pdf  
  Summary: Filename is not descriptive. Please open the PDF to extract the real title and authors. It may be notes or a paper; update this entry with a proper title and summary after inspection.  
  Tags: needs-review, ambiguous-filename

- NeurIPS-2019-gradient-based-sample-selection-for-online-continual-learning-Paper.pdf  
  Summary: Gradient-based Sample Selection (GSS) for online continual learning. Proposes selecting representative samples for the replay buffer based on gradient diversity/coverage to improve online continual learners. Useful when building replay strategies that must be memory-efficient.  
  Tags: replay buffer, sample selection, online continual learning, gradient-based

- Online-LoRA.pdf  
  Summary: Online adaptations of LoRA-style parameter-efficient updates for large models. Explains how to update compact adapter parameters in an online fashion, which is directly applicable to parameter-efficient continual adaptation and on-device continual learning scenarios.  
  Tags: LoRA, parameter-efficient tuning, online adaptation

- Softmax-based OOD Detection.pdf  
  Summary: Classic softmax-confidence-based OOD detection analysis (maximum softmax probability and related calibration issues). Useful as baseline comparisons against energy/Mahalanobis-based detectors.  
  Tags: OOD, softmax, calibration, baseline

- Tiwari_GCR_Gradient_Coreset_Based_Replay_Buffer_Selection_for_Continual_Learning_CVPR_2022_paper.pdf  
  Summary: Gradient Coreset Reduction (GCR) — uses gradient-space coreset selection to choose a compact, informative replay buffer for continual learning. Demonstrates coreset-based approaches that directly optimize for gradient coverage or representativeness.  
  Tags: coreset, replay buffer, gradient-based, CVPR 2022

---

Recommended reading order and topical grouping

1. Primer & evaluation
   - Continual Learning - 14062025.pdf (overview, protocols)

2. Core replay & sample selection techniques
   - NeurIPS 2019 GSS (gradient-based sample selection)
   - Tiwari CVPR 2022 GCR (gradient-coreset replay selection)

3. Parameter-efficient and online adaptation
   - Online-LoRA.pdf

4. Representation/backbone considerations (helps reduce forgetting)
   - DINOv3.pdf

5. Out-of-distribution detection (robustness / novelty detection in continual settings)
   - Softmax-based OOD Detection.pdf
   - Mahalanobis Distance based OOD Detection.pdf
   - Energy-based OOD Detection.pdf

6. Repository-specific notes and ambiguous files
   - NL.pdf (inspect and rename/update)

This order is intended to first establish foundational concepts (what forgetting is and how we measure it), then dive into practical mechanisms (replay selection and parameter-efficient adaptation), and finally consider supporting tools like robust representations and OOD detectors.

---

How to use these files

- Local reading: clone the repository and open the PDF files in the papers/ directory.
- Reproducing experiments: consult the paper PDF for algorithmic details and check the repository for corresponding code or scripts (if present).
- Quick lookup: use the tags to find papers relevant to replay, OOD, or representation learning.
- When adding notes or code that implements a paper, reference the file name exactly and add a link back to the corresponding PDF in this folder.

---

How to contribute

To add a new paper or note:
1. Add the PDF to the papers/ directory (prefer a descriptive filename: Title_Year_Author.pdf).
2. Update Papers.md with:
   - The file link (use the repository blob link if the PDF is in-repo).
   - A one-paragraph summary with key contributions and why it's relevant to continual learning.
   - Tags (comma-separated): e.g., replay, OOD, backbone, coreset.
3. Open a pull request and include why the paper belongs in the collection (short justification).
4. If you cannot add the PDF due to copyright, add an external link (arXiv/DOI) and a short summary instead.

Filename/metadata suggestions:
- Use human-readable filenames, avoid cryptic abbreviations (e.g., rename NL.pdf → Author_Title_Year.pdf).
- Optionally add a small metadata YAML at the top of each PDF (in a .yml or README) for automated tooling in the future (authors, year, DOI/arXiv, tags).

---

Citation & license notes

- The PDFs here are copies of original research papers. Respect the original licenses and citation norms of each paper. When using or reproducing results, cite the original work directly.
- This Papers.md is intended as an organizational aid. If you’d like to license this document explicitly, add a license header (e.g., CC BY or CC0) at the top and include a LICENSE file in the repo.

---

TODOs / suggested follow-ups

- Inspect NL.pdf and update its filename, summary and tags.
- Expand summaries to include authors, publication venue, year, and citation snippet (BibTeX) for each paper.
- Add short “Key equations / algorithms” or a 3-line summary for implementers for each paper.
- (Optional) Add a small index file (papers/index.yml) with structured metadata to support automated generation of Papers.md in the future.

---

If you'd like, I can:
- Generate BibTeX entries for each paper (requires extracting metadata from the PDFs or arXiv).
- Propose a branch and a PR that adds this file to the repo (I'll prepare the commit message and diff for you to push).
- Inspect NL.pdf and produce an updated descriptive filename and summary.
