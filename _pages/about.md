---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>

Hi! I am a first-year Ph.D. student in Computer Science at Texas A&M University, working in the [OptMAI Lab](https://people.tamu.edu/~tianbao-yang/) advised by [Dr. Tianbao Yang](https://people.tamu.edu/~tianbao-yang/). My research focuses on **large-scale multimodal foundation models**, in particular **pretraining methods**, **optimization**, and **scalable distributed training pipelines**. I have experience pretraining foundation models on **highly multimodal data** with diverse distributions spanning **14+ medical imaging modalities**.

# 🔥 News
- *2026.11*: A US patent application for RADEO, our unified multi-modality foundation model for medical imaging, is now pending.
- *2026.10*: Received the NeurIPS 2026 Travel Award.
- *2026.09*: Our paper, "Tune-Up Open-Weight CLIP: Optimization Framework for Self-Supervised Fine-tuning of CLIP" (TuneCLIP), was accepted at NeurIPS 2026 as a <span style="color:red">Spotlight</span> (top 3%)! [[paper]](https://arxiv.org/abs/2601.09859) [[code]](https://github.com/Optimization-AI/TuneCLIP)
- *2026.08*: Started my Ph.D. in Computer Science at Texas A&M University under [Prof. Tianbao Yang](https://people.tamu.edu/~tianbao-yang/).
- *2025.01*: Our paper, "HFMF: Hierarchical Fusion Meets Multi-Stream Models for Deepfake Detection", was accepted at the WACV 2025 Workshop on AI for Multimedia Forensics & Disinformation Detection as an <span style="color:green">Oral</span>!
- *2024*: Our work, "Calibrating Machine Learning Models For Accurate Stroke Type Prediction In Low-resource Settings", was accepted at the 16th World Stroke Congress (WSC 2024), an opportunity to collaborate with AIIMS Delhi, India!
- *2024.01*: Our paper, "A Feature Extraction and Time Warping Based Neural Expansion Architecture for Cloud Resource Usage Forecasting", was published in Cluster Computing.
- *2023.10*: Our paper, "An Automated Diagnosis Model for Classifying Cardiac Abnormality Utilizing Deep Neural Networks", was published in Multimedia Tools and Applications.

# 📝 Publications 

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">Preprint Soon</div><img src='images/teaser-radeo-v2.jpg' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

RADEO: A Unified Self-supervised Foundation Model Across Diverse Medical Imaging Modalities

**Anant Mehta**, Vicente Balmaseda, Xiyuan Wei, Ryan King, Varsha Goalla, Girish Bathla, Sadeer G. Al-Kindi, Kyle J. Myers, Tianbao Yang

<span style="color:green">**US Patent Pending**</span> · To be submitted to *Nature*
- Led the development and pretraining of **RADEO**, a single **multi-modality foundation model** self-supervised pretrained on **millions of images** spanning **14+ medical imaging modalities**.
- RADEO beats Google Research's **MedSigLIP**, the image encoder used in [MedGemma](https://deepmind.google/models/gemma/medgemma/), and achieves a **mean rank of 1** across various tasks.
- Scaled RADEO to a larger model with **700+ GPUs** in a heroic run on [**VISION**](https://vision.tamus.edu/), the Texas A&M System's NVIDIA DGX SuperPOD (**#66** on the June 2026 TOP500 list), achieving state-of-the-art performance among medical foundation models.
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">NeurIPS 2026 Spotlight (Top 3%)</div><img src='images/teaser-tuneclip.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[Tune-Up Open-Weight CLIP: Optimization Framework for Self-Supervised Fine-tuning of CLIP](https://arxiv.org/abs/2601.09859)

**Anant Mehta**, Xingyu Chen, Xiyuan Wei, Tianbao Yang

[**Paper**](https://arxiv.org/abs/2601.09859) [**Code**](https://github.com/Optimization-AI/TuneCLIP)
- We show that simply applying standard training protocols to an open-weight CLIP model often *degrades* performance, and ask whether such models can be improved using only existing self-supervised data.
- We propose **TuneCLIP**: a warm-up stage that recovers optimization statistics to reduce cold-start bias, followed by fine-tuning with a new contrastive loss that reduces the penalization of false-negative pairs.
- TuneCLIP yields consistent gains across architectures and scales, e.g., up to **+2.5%** on ImageNet and related OOD benchmarks and **+1.2%** on DataComp for SigLIP (ViT-B/16).
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">WACV 2025 Workshop (Oral)</div><img src='images/teaser-hfmf.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[HFMF: Hierarchical Fusion Meets Multi-Stream Models for Deepfake Detection](https://ieeexplore.ieee.org/abstract/document/10972529)

**Anant Mehta**, Bryant McArthur, Nagarjuna Kolloju, Zhengzhong Tu

[**Paper**](https://ieeexplore.ieee.org/abstract/document/10972529) [**Code**](https://github.com/taco-group/HFMF)
- We propose HFMF, a two-stage deepfake detection framework: the first stage fuses vision Transformers and convolutional networks via hierarchical feature fusion; the second combines object-level information with a fine-tuned CNN.
- An ensemble deep neural network merges both streams, achieving strong performance across multiple benchmarks while remaining well calibrated.
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">MTAP 2024</div><img src='images/teaser-cardiac.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[An Automated Diagnosis Model for Classifying Cardiac Abnormality Utilizing Deep Neural Networks](https://link.springer.com/article/10.1007/s11042-023-16930-5)

Gurjot Singh, Abhinav Verma, Lavanya Gupta, **Anant Mehta**, Vinay Arora

*Multimedia Tools and Applications*, 83(13), 2024

[**Paper**](https://link.springer.com/article/10.1007/s11042-023-16930-5)
- We develop a deep neural network–based model for automated classification of cardiac abnormalities.
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">Cluster Computing 2024</div><img src='images/teaser-cloud_forecasting.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[A Feature Extraction and Time Warping Based Neural Expansion Architecture for Cloud Resource Usage Forecasting](https://link.springer.com/article/10.1007/s10586-023-04224-2)

Gurjot Singh, Prajit Sengupta, **Anant Mehta**, Jatin Bedi

*Cluster Computing*, 27(4), 2024

[**Paper**](https://link.springer.com/article/10.1007/s10586-023-04224-2)
- We propose a neural expansion architecture combining feature extraction and time warping to forecast cloud resource usage.
</div>
</div>

# 🎖 Honors and Awards
- *2026*: **Travel Award** — Annual Conference on Neural Information Processing Systems (**NeurIPS**)
- *2026*: **Spotlight Paper (top 3%)** — NeurIPS 2026 (TuneCLIP)
- *2025*: **Travel Award** — IEEE/CVF Winter Conference on Applications of Computer Vision (**WACV**)
- *2025*: **Oral Presentation** — WACV 2025 Workshop on AI for Multimedia Forensics & Disinformation Detection
- *2024*: **Scholarship (USD 30,000)** — [Center for Curiosity](https://www.centerforcuriosity.com/research)
- *2024*: **Oxford Machine Learning Summer School (OxML)** — Selected participant, sponsored by Google DeepMind
- *2024*: **University Medal and Cash Prize** — Thapar Institute of Engineering & Technology, for excellence in academics *(ranked in top 1%)*
- *2023*: **Best Research Paper Award** — HeartBeatNet: Unleashing the Power of Attention in Cardiology, CINS 2023
- *2020 - 2024*: **Academic Merit Scholarship (USD 15,600 total)** — Thapar Institute of Engineering & Technology (4 consecutive years)

# 📖 Education
- *2026.08 - Present*, Ph.D. in Computer Science, Texas A&M University, College Station, Texas
- *2024.08 - 2026.05*, M.S. in Computer Science, Texas A&M University, College Station, Texas
- *2020.09 - 2024.06*, B.E. in Computer Engineering, Thapar Institute of Engineering & Technology, Patiala, India

# 💻 Experience
- *2024.01 - 2024.06*, **Research Intern**, **Indian Institute of Technology Delhi**, New Delhi, India, with [Prof. Rahul Garg](https://www.cse.iitd.ac.in/~rahulgarg/)
- *2023.06 - 2023.07*, **Machine Learning Engineer Intern**, Metacube Software, Jaipur, India
- *2022.06 - 2022.07*, **Deep Learning Research Engineer Intern**, NPBridge, Bengaluru, India

# 📚 Service
- *Spring 2026*: Graduate Teaching Assistant, CSCE 482: Senior Capstone Design (undergraduate), Texas A&M University. Mentored 6 projects with 30 students.
- *Fall 2025*: Graduate Teaching Assistant, CSCE 703 / CYBR 603: Cybersecurity Risk (graduate), Texas A&M University. Mentored 5 students on a research project, one of which led to the **Best Student Paper Award** at GAISS 2026, UT Austin.
