<p align="center">
  <img src="assets/logo/origindatalab-logo.png" alt="Origin Data Lab" width="250">
</p>

<h1 align="center">Privacy Processing & Human Verification</h1>

<p align="center">
  AI-assisted face anonymization for real-world video, supported by human verification and customer-specific quality rules.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Privacy-Processing-2563EB?style=flat-square" alt="Privacy Processing">
  <img src="https://img.shields.io/badge/Human-Verification-0F766E?style=flat-square" alt="Human Verification">
  <img src="https://img.shields.io/badge/Public-Evaluation-V58-15803D?style=flat-square" alt="Public Evaluation V58">
  <img src="https://img.shields.io/badge/Pilot-Projects%20Welcome-7C3AED?style=flat-square" alt="Pilot Projects Welcome">
</p>

<p align="center">
  <a href="https://origindatalab.io"><strong>Visit Website</strong></a>
  ·
  <a href="demo/Origin%20Data%20Lab%20Face%20Anonymization%20Demo%20(V58).mp4?raw=1"><strong>Watch Demo</strong></a>
  ·
  <a href="reports/technical_report.pdf?raw=1"><strong>View Technical Report</strong></a>
</p>

> **Start with a private 1–5 minute sample evaluation before scaling to production.**

---

## Overview

Origin Data Lab provides practical privacy-processing support for video datasets that contain identifiable faces.

Our workflow combines:

- automated face detection and anonymization
- human verification for missed or uncertain cases
- customer-specific masking and acceptance rules
- delivery in video, image, and structured annotation formats

This repository presents a public V58 evaluation using dense, low-light urban traffic footage.

> **This public evaluation shows automated processing output. Commercial delivery can include the agreed level of human verification depending on project requirements.**

---

## Before / After

<p align="center">
  <img src="assets/images/before_after.jpg" alt="Origin Data Lab face anonymization before and after" width="95%">
</p>

### Additional Evaluation Frames

<table>
  <tr>
    <td width="50%" align="center">
      <img src="assets/images/before_after_003s.jpg" alt="Before and after comparison at 3 seconds" width="100%">
    </td>
    <td width="50%" align="center">
      <img src="assets/images/before_after_008s.jpg" alt="Before and after comparison at 8 seconds" width="100%">
    </td>
  </tr>
  <tr>
    <td width="50%" align="center">
      <img src="assets/images/before_after_030s.jpg" alt="Before and after comparison at 30 seconds" width="100%">
    </td>
    <td width="50%" align="center">
      <img src="assets/images/before_after_061s.jpg" alt="Before and after comparison at 61 seconds" width="100%">
    </td>
  </tr>
</table>

---

## Demo Video

<p align="center">
  <a href="demo/Origin%20Data%20Lab%20Face%20Anonymization%20Demo%20(V58).mp4?raw=1">
    <img src="assets/thumbnails/demo-thumbnail.jpg" alt="Watch Origin Data Lab V58 face anonymization demo" width="85%">
  </a>
</p>

<p align="center">
  <a href="demo/Origin%20Data%20Lab%20Face%20Anonymization%20Demo%20(V58).mp4?raw=1"><strong>▶ Watch the public V58 demonstration</strong></a>
</p>

The demo includes:

- original footage
- automated anonymized output
- side-by-side comparison
- dense urban traffic
- low-light and partially occluded faces

---

## Public Evaluation — V58

| Metric | Result |
|---|---:|
| Video duration | Approximately 1 min 29 sec |
| Processed frames | 2,661 |
| Detected face regions | 10,634 |
| Processing time | 238.3 sec |
| Processing speed | 11.169 FPS |
| Mean detection confidence | 0.637 |
| Evaluation environment | CPU processing |

These values describe this specific public evaluation and should not be interpreted as guaranteed performance for every dataset or environment.

### Detection Summary

<p align="center">
  <img src="assets/charts/detection_chart.png" alt="V58 detection summary chart" width="82%">
</p>

### Confidence Distribution

<p align="center">
  <img src="assets/charts/confidence_chart.png" alt="V58 confidence distribution chart" width="82%">
</p>

---

## Why Origin Data Lab

### AI + Human Verification

Automation handles the majority of routine detections. Human verification can then focus on low-confidence frames, missed faces, occlusion, motion blur, small targets, and other difficult cases.

### Pilot-Friendly and Direct

Small projects are welcome. Customers can begin with a short private sample and communicate directly with the people responsible for processing and quality review.

### Customer-Specific Rules

Masking strength, review scope, output format, acceptance criteria, and delivery requirements can be adjusted for each project.

---

## Workflow

```text
Customer Sample
      │
      ▼
Requirement and Privacy Rule Review
      │
      ▼
Automated Detection and Anonymization
      │
      ▼
Human Verification, if included
      │
      ▼
Quality Review
      │
      ▼
Final Delivery and Report
```

Our approach is designed to automate roughly 80–90% of routine processing where conditions allow, while assigning the remaining difficult cases to human verification. The actual automation ratio depends on footage quality, scene complexity, target size, occlusion, and customer acceptance criteria.

---

## Human Verification

Human verification is managed by our quality engineering team.

Review scope can include:

- missed-face recovery
- low-confidence frame inspection
- blur coverage checks
- temporal consistency checks
- bounding-box correction
- customer-specific exception handling
- final delivery review

Additional review capacity can be organized according to project size, schedule, security requirements, and quality targets.

---

## Pilot Process

### 1. Share a Small Private Sample

A 1–5 minute sample is usually enough for an initial quality check.

### 2. Define the Rules

We confirm the target objects, masking method, output format, human-review scope, and acceptance criteria.

### 3. Process the Sample

The sample is processed through the automated pipeline and, where agreed, additional human verification.

### 4. Review the Output

The customer receives the processed sample and can request practical adjustments.

### 5. Decide Whether to Scale

After the pilot, both sides can confirm production volume, schedule, security conditions, and pricing.

<p align="center">
  <a href="https://origindatalab.io"><strong>Request a Private Sample Evaluation</strong></a>
</p>

---

## Services

| Service | Scope | Example Outputs |
|---|---|---|
| Face anonymization | Automated privacy masking with optional human verification | MP4, MOV, image sequences |
| Human verification and GT | Missed-detection review, correction, annotation, QA | YOLO, COCO, JSON, JSONL, CSV |
| Dataset preparation | Metadata generation, restructuring, format conversion | Customer-defined schemas |
| Private pilot evaluation | Small-batch quality and workflow validation | Processed sample, HTML/PDF report |

---

## Security and Data Handling

Security requirements are agreed before each commercial project.

Depending on project scope, the workflow can include:

- project-specific storage and access rules
- restricted access to customer data
- agreed retention and deletion schedules
- no external model training with customer data without written approval
- NDA or customer-provided security requirements
- delivery through an agreed secure method

This public repository is a demonstration. Formal compliance claims should only be made after the applicable customer requirements, contracts, infrastructure, and procedures have been confirmed.

---

## Known Limitations

Automated anonymization can be affected by:

- severe motion blur
- extreme low light
- heavy occlusion
- very small or distant faces
- reflections, displays, posters, or face-like objects
- rapid camera movement
- compression artifacts
- unusual camera angles

Automation alone may not fully resolve every situation. Human verification can be included according to the quality target and risk level agreed for the project.

---

## Reports and Files

- [HTML Evaluation Report](reports/report.html?raw=1)
- [Technical Evaluation Report — PDF](reports/technical_report.pdf?raw=1)
- [Public V58 Demo Video](demo/Origin%20Data%20Lab%20Face%20Anonymization%20Demo%20(V58).mp4?raw=1)

<details>
<summary><strong>Repository structure</strong></summary>

```text
privacy-processing-demo/
├── README.md
├── LICENSE
├── assets/
│   ├── logo/
│   │   └── origindatalab-logo.png
│   ├── charts/
│   │   ├── confidence_chart.png
│   │   └── detection_chart.png
│   ├── images/
│   │   ├── before_after.jpg
│   │   ├── before_after_003s.jpg
│   │   ├── before_after_008s.jpg
│   │   ├── before_after_030s.jpg
│   │   └── before_after_061s.jpg
│   └── thumbnails/
│       └── demo-thumbnail.jpg
├── demo/
│   └── Origin Data Lab Face Anonymization Demo (V58).mp4
└── reports/
    ├── report.html
    └── technical_report.pdf
```

</details>

---

## About Origin Data Lab

Origin Data Lab supports privacy processing, human verification, Human GT, dataset quality review, and custom data-production workflows.

We focus on practical execution: start with a small sample, define the quality rules clearly, communicate directly, and scale only after the customer has reviewed the output.

---

## Contact

**Website:** [https://origindatalab.io](https://origindatalab.io)

For a private pilot, send a short description of:

- data type and approximate volume
- target objects to anonymize
- expected output format
- desired schedule
- security or deletion requirements

---

<p align="center">
  <strong>Origin Data Lab — Practical AI Processing, Human Verification, and Dataset Quality Support</strong>
</p>
