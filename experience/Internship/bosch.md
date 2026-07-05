---
company: Bosch Global Software Technologies
role: Computer Vision Intern
description: Developed a self-supervised image recommendation and retrieval system for ADAS drive logs, integrating VGG, RNN, and BLIP-2 architectures to accelerate dataset curation.
employmentType: Internship
location: Bengaluru, India
startDate: 2024-01
endDate: 2024-06
current: false
published: true
featured: true
order: 100
website: https://www.bosch-softwaretechnologies.com/en/
technologies: [Computer Vision, Self-Supervised Learning, Deep Learning, Image Recommendation, BLIP-2, VGG, RNN, Active Learning]
---

# Internship at Bosch Global Software Technologies

During my internship at Bosch Global Software Technologies, I worked on the **Automotive Self-Driving (ADAS)** project. My primary objective was to build and optimize an intelligent, scalable **Image Recommendation System** to curate high-quality training datasets from millions of unlabeled road images.

By utilizing self-supervised learning, deep vision backbones, sequence modeling, and state-of-the-art vision-language models, I developed pipelines that drastically reduced the manual effort required for data labeling and model fine-tuning.

---

## Overview

In autonomous driving systems (ADAS), vehicles capture millions of frames of driving logs daily. Finding relevant scenarios (e.g., specific weather conditions, corner cases, or road signs) within these massive, unlabeled datasets is a major challenge. 

This project focused on building an image-to-image and text-to-image recommendation system that allows engineers to query millions of unlabeled images and retrieve relevant frames for model training and fine-tuning.

---

## Responsibilities

* **Pipeline Design:** Architected a self-supervised vision pipeline to process and index massive volumes of unlabeled road-scene imagery.
* **Feature Extraction & Classification:** Fine-tuned deep learning models to generate robust embeddings and classify frame content.
* **Multimodal Retrieval:** Integrated vision-language models to support natural language queries for semantic image search.
* **Human-in-the-Loop Integration:** Built feedback mechanisms to dynamically refine recommendation results based on user interactions.

---

## Impact

* **High-Accuracy Retrieval:** Achieved **92% accuracy** in real-time image recommendation across specified road and environmental classes.
* **Multimodal Search:** Improved retrieval accuracy to **~95%** by leveraging advanced vision-language models for natural language queries.
* **Dataset Curation Efficiency:** Significantly reduced dataset preparation time for ADAS downstream models by automating the discovery of relevant, edge-case road frames.

---

## Notable Work

### 1. Self-Supervised Feature Generation & Classification
To extract meaningful representations from unlabeled driving logs, I implemented a self-supervised pipeline:
* **Feature Extraction:** Fine-tuned a **VGG** backbone to generate dense, low-dimensional feature embeddings representing the spatial layout and objects within each frame.
* **Sequence Modeling:** Integrated an **RNN** model to process sequential frames, capturing temporal context and transitions in driving logs to improve scenario classification.

### 2. Multimodal Query-Based Search with BLIP-2
To allow engineers to query the dataset using natural language (e.g., *"wet asphalt at sunset with pedestrians"*), I integrated the **BLIP-2** (Bootstrapping Language-Image Pre-training) model:
* Mapped visual and textual features into a shared embedding space.
* Achieved an impressive **~95% accuracy** on zero-shot semantic queries.

### 3. Active Learning & Human Feedback Loop
To continually improve retrieval performance:
* Developed an active learning interface where human feedback at query time directly influences the retrieval algorithms.
* Readjusted similarity weights based on positive/negative user confirmations, leading to higher precision in successive retrieval rounds.

---

## Tools and Systems

* **Frameworks & Models:** PyTorch, VGG, RNNs, BLIP-2
* **Domains:** Computer Vision, Self-Supervised Learning, Multimodal Retrieval
* **Methods:** Active Learning, Embedding Vector Search, Feature Engineering

---

## Lessons

* **Self-Supervised Power:** Standard supervised learning is bottlenecked by manual labeling. Self-supervised learning is crucial for unlocking the value of massive, raw driving datasets.
* **Multimodal Alignment:** Zero-shot models like BLIP-2 bridge the gap between human intuition and raw pixel data, making datasets highly searchable.
* **Active Learning Loops:** Human feedback is a powerful catalyst for refining models in production without needing full retraining cycles.
