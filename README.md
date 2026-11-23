<div align="center">

# Nisha Pandey

### Computer Engineer · Trustworthy Medical AI · Medical Image Analysis · Efficient On-Device ML

[![GitHub](https://img.shields.io/badge/GitHub-nishapandey9098-181717?style=for-the-badge&logo=github)](https://github.com/nishapandey9098)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin)](https://linkedin.com/in/np9098)
[![Email](https://img.shields.io/badge/Email-Contact-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:pandeynisha113@gmail.com)
[![Research Paper](https://img.shields.io/badge/Publication-ICICSET%202026-2E6D55?style=for-the-badge&logo=readthedocs&logoColor=white)](https://doi.org/10.65091/icicset.v3i1.76)

**Kathmandu, Nepal** · B.E. in Computer Engineering, Tribhuvan University (2026)

</div>

---

## About me

I am a Computer Engineering graduate interested in building **medical AI systems that are reliable, efficient, and honest about their limitations**. My work sits at the intersection of medical image analysis, trustworthy machine learning, on-device AI, and software quality.

My central research question is simple: **When should an AI system make a prediction, when should it ask for human review, and how can we demonstrate that it behaves reliably?**

I explore this through uncertainty estimation and calibration, selective prediction, model compression, robustness evaluation, and practical applications for low-resource healthcare settings. I am particularly interested in solutions that can operate on limited hardware, work offline, protect sensitive data, and remain accessible to the people who need them.

I am currently a **Junior QA Engineer at ING Consulting Pvt. Ltd. (ING Tech, Innovate Nepal Group)**. Working across web and mobile products has strengthened my test-driven approach to software and informs how I evaluate machine-learning systems: not only by whether they work under ideal conditions, but also by how they fail.

## Research interests

- **Trustworthy machine learning:** uncertainty estimation, probability calibration, selective prediction, and human-in-the-loop referral.
- **Medical image analysis:** retinal imaging, diabetic retinopathy screening, image segmentation, and severity grading.
- **Efficient and on-device AI:** model pruning, quantization, lightweight inference, offline-first systems, and federated learning.
- **Robustness and evaluation:** distribution shift, corruption testing, reproducibility, multi-seed experiments, and statistical reporting.
- **Accessible healthcare technology:** OCR and speech interfaces for older adults and people with visual impairments, including future Nepali-language support.
- **ML systems quality:** automated testing, behavioral validation, and continuous integration for machine-learning pipelines.

## Selected research and engineering work

### 1. Knowing When Not to Predict
**Calibration, uncertainty, and selective referral for medical image classifiers**

[![Repository](https://img.shields.io/badge/Repository-View%20project-181717?logo=github)](https://github.com/nishapandey9098/medical-image-classifier-calibration)

- Compared single models, Monte Carlo dropout, deep ensembles, and temperature scaling on PneumoniaMNIST and RetinaMNIST.
- Evaluated calibration and selective prediction using ECE, NLL, Brier score, AUC/QWK, and risk–coverage analysis.
- On RetinaMNIST, the ensemble achieved **0.595 accuracy overall** and **0.790 accuracy on the 50% of cases it answered with the highest confidence**; its ECE was 0.042.
- The project investigates how a model can route uncertain cases for human review rather than forcing a prediction.

### 2. Compressing a Medical Image Classifier for Offline Use
**FP16, INT8, and pruning trade-offs**

[![Repository](https://img.shields.io/badge/Repository-View%20project-181717?logo=github)](https://github.com/nishapandey9098/medical-image-classifier-compression)

- Benchmarked compressed ResNet-18 variants using ONNX and ONNX Runtime across two MedMNIST datasets.
- Evaluated model size, CPU latency, predictive performance, and calibration—not model size alone.
- A structured-pruning, fine-tuning, and INT8 configuration produced a **5.79 MB model** and approximately **3.9× CPU speedup**.
- The accuracy cost differed by dataset: 2.0 percentage points on RetinaMNIST and 7.1 points on PneumoniaMNIST, motivating further investigation into class- and confidence-specific effects.

### 3. A Multi-Seed Ablation Study of Medical Image Classifiers
**Pretraining, augmentation, and CLAHE**

[![Repository](https://img.shields.io/badge/Repository-View%20project-181717?logo=github)](https://github.com/nishapandey9098/medical-image-classifier-ablation-study)

- Trained and evaluated **80 ResNet-18 runs** across eight experimental settings, five random seeds, and two public datasets.
- Used official data splits, validation-based model selection, confidence intervals, and multiple-comparison control.
- Found that seed-to-seed variation could be comparable to or larger than the effects being measured—highlighting why single-run comparisons can be misleading.

### 4. ML Reliability Test Suite
**Metamorphic and corruption testing with pytest and CI**

- Built automated tests for medical image classifiers under blur, brightness changes, rotation, JPEG compression, and noise.
- Defined pass/fail thresholds and configured execution through GitHub Actions.
- Focuses on repeatable behavioral checks that can help detect regressions when a model or preprocessing pipeline changes.

### 5. MediMate — On-Device OCR and Voice-Assisted Medication Support

[![Published paper](https://img.shields.io/badge/Paper-ICICSET%202026-2E6D55?logo=readthedocs&logoColor=white)](https://doi.org/10.65091/icicset.v3i1.76)

**First-author conference paper:** *An Intelligent Mobile Framework for OCR-Based Medicine Recognition and Voice-Assisted Medication Adherence* (ICICSET 2026, pp. 206–213).

- Led the research and development of an offline-first mobile application using Flutter, Firebase/Firestore, Google ML Kit, and native Android components.
- Designed a confidence-gated OCR workflow that evaluates image, text, and orientation quality, then asks the user to retake an unclear image.
- Developed a fuzzy medicine-matching workflow over an 11,825-record directory; ambiguous matches are presented for user confirmation instead of being selected automatically.
- Implemented medication reminders with native Android alarms, Taken/Missed actions, retry logic, and text-to-speech support.
- In project testing, the workflow achieved 98% operational success under favorable image conditions; performance fell on severely blurred images. All 200 of 200 test alarms were delivered across Android 12–15.

### 6. AI-Based Diabetic Retinopathy Screening
**U-Net++ segmentation and EfficientNetB0 classification**

- Co-authored a rapid scoping review of deep-learning methods for diabetic retinopathy detection, segmentation, and grading.
- Contributed image processing to a segmentation-then-classification pipeline for five-class grading using public retinal fundus images.
- Worked with CLAHE enhancement, U-Net++ segmentation, EfficientNetB0 classification, and a PyQt5 clinician-facing prototype.
- The manuscript is in preparation. Error analysis highlighted confusion around adjacent severity grades and the importance of clinician review at stage boundaries.

> **Research note:** The classifier studies above are controlled experiments on public benchmark datasets. They are not clinical validation studies, and their results should not be interpreted as evidence of real-world diagnostic performance.

## Publications and research writing

- **Pandey, N.**, Rana, S., Lamsal, T., Lamichhane, N., & Koirala, B. (2026). *An Intelligent Mobile Framework for OCR-Based Medicine Recognition and Voice-Assisted Medication Adherence.* Proceedings of the International Conference on Innovation in Computing, Science, Engineering and Technology (ICICSET), 206–213. [https://doi.org/10.65091/icicset.v3i1.76](https://doi.org/10.65091/icicset.v3i1.76)
- Lamichhane, N., Ghimire, B. R., **Pandey, N.**, & Koirala, B. *AI-based Diabetic Retinopathy Screening in Rural Nepal: A Rapid Scoping Review and Experimentation.* Manuscript in preparation.
- Pandey, N., Pandey, S., Rana, S., & Bhandari, S. *Smart Social Travel Platform for Solo Travelers: The Design and Development of Travel Buddy.* Technical research report. [ResearchGate preprint](https://doi.org/10.13140/RG.2.2.16460.17281)

## Engineering and professional experience

**Junior QA Engineer · ING Consulting Pvt. Ltd. (ING Tech, Innovate Nepal Group)**  
*July 2026 – Present · Kathmandu, Nepal*

- Test web and mobile education platforms across CRM, CLMS, Attendance, and Admission workflows.
- Design and execute functional, regression, integration, and performance test cases across tenants and user roles.
- Automate regression scenarios with Playwright and the Page Object Model; validate APIs with Postman and data with SQL.
- Track defects with reproducible steps and root-cause notes in Jira and ClickUp within Agile/Scrum sprints.

**Quality Assurance Associate · Black Tech Pvt. Ltd.**  
*January 2026 – July 2026 · Pokhara, Nepal*

- Tested the RestroX CRM in development and production environments through functional, regression, and exploratory testing.
- Used network inspection to investigate API failures and payload mismatches; developed Playwright scripts and managed defects in Jira and Plane.

## Technical toolkit

| Area | Tools and technologies |
|---|---|
| Machine learning | PyTorch, TensorFlow/Keras, scikit-learn, NumPy, Pandas, OpenCV, Matplotlib |
| Medical AI | ResNet-18, EfficientNet, U-Net/U-Net++, MedMNIST, OCR, calibration, MC dropout, deep ensembles, selective prediction |
| Efficient inference | ONNX, ONNX Runtime, FP16, INT8 quantization, pruning, CPU benchmarking |
| Testing and reliability | Playwright, pytest, Selenium, Cypress, Postman, GitHub Actions, API testing, SQL validation |
| Software development | Python, Dart, JavaScript, TypeScript, C, C++, SQL, Flutter, React, Ruby on Rails, PyQt5 |
| Mobile and cloud | Flutter, Firebase, Firestore, Riverpod, native Android, AlarmManager, BroadcastReceiver |
| Design and collaboration | Figma, Adobe Photoshop, Illustrator, Git, GitHub, Jira, ClickUp, Plane |
| Hardware and robotics | Arduino, microcontrollers, sensors, KiCad |

## Beyond research

I enjoy working across the full path from an idea to a usable product—from researching a problem and building an ML pipeline to designing interfaces and testing the finished system. My broader experience includes UI/UX and graphic design, mobile and web development, Python automation, and robotics.

As a member and executive of the Robotics Club at Pashchimanchal Campus, I worked on robotic-arm and maze-following projects, PCB layouts, and Arduino-based systems. Our maze-following robot won the **Micromouse Competition at LOCUS 2023**. I also taught Arduino IDE programming sessions to junior members.

## What I am exploring next

I am interested in research opportunities and graduate study (M.S./Ph.D.) focused on **trustworthy and efficient AI for healthcare**. In particular, I want to investigate calibrated referral under dataset shift, compression that preserves reliability, and reproducible testing methods for medical ML systems—especially for settings with limited clinical resources and hardware.

I welcome opportunities to collaborate on medical imaging, reliable machine learning, efficient deployment, and ML systems evaluation.

## Connect

- **Email:** [pandeynisha113@gmail.com](mailto:pandeynisha113@gmail.com)
- **LinkedIn:** [linkedin.com/in/np9098](https://linkedin.com/in/np9098)
- **GitHub:** [github.com/nishapandey9098](https://github.com/nishapandey9098)
- **Research paper:** [ICICSET 2026 publication](https://doi.org/10.65091/icicset.v3i1.76)

---

<div align="center">

*Building AI that knows when to predict, when to defer, and how to prove the difference.*

</div>
