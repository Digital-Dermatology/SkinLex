# SkinLex: Multi-Dataset Diagnostic Utility of Clinical Visual Concepts in AI Systems for Dermatology

[![MICCAI ISIC 2026](https://img.shields.io/badge/MICCAI_ISIC_2026-Spotlight-blue.svg)](https://isic-archive.com/) [![Paper PDF](https://img.shields.io/badge/Poster-PDF-red.svg)](./poster.pdf)

This repository contains the poster and upcoming code release for the paper **"Multi-Dataset Diagnostic Utility of Clinical Visual Concepts in AI Systems for Dermatology"** (Accepted as Spotlight to the 11th ISIC Workshop @ MICCAI 2026).

The full code base, dataset preprocessing scripts, and LLM prompt templates are currently being prepared and will be made available here shortly.

## Abstract & Overview

The clinical integration of AI decision-support systems in digital dermatology relies heavily on human trust. Clinical visual concepts act as an intermediate representation layer that can enhance human trust, corroborate model reliability, and enable intuitive auditing by medical staff.

**SkinLex** harmonizes **48 clinical morphological attributes** across four public datasets (*SkinCon*, *DermaCon-IN*, *MM-Skin*, and *PASSION*) to create a unified benchmark of **20,411 records**. Using this dataset, we evaluate how machine learning models utilize structured clinical concepts to predict 9-partition dermatological disease categories.

## Key Insights

* **Concept Complementarity:** Restricting inputs to specific concept groups (e.g., colors or shapes alone) causes accuracy drops, showing that coarse diagnosis requires a varied combination of visual features.
* **Concept Redundancy:** Bootstrapped backward elimination reveals feature redundancy for algorithmic classification, allowing the omission of 8 concepts (for AP) and up to 18 concepts (for ROC-AUC) without significant performance loss.
* **Clinical Utility:** Identifying and removing redundant concepts could guide future concept set selection, potentially reducing annotation effort, improving modeling efficiency, and enhancing clinical trust.

## Repository Contents

* [`poster.pdf`](./poster.pdf): PDF version of the poster presentation.
* `code/`: *(Coming soon)* Data harmonization pipelines, baseline models (LightGBM, Logistic Regression), and evaluation scripts.
* `prompts/`: *(Coming soon)* Qwen3.6 prompt templates used for diagnostic label mapping and concept extraction from text captions.