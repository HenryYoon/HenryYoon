# Curriculum Vitae

**Name:** Hee-Seung Yun  
**Job:** ML Engineer (Vision AI / Edge Deployment)  
**Email:** yoonihg@gmail.com  
**Social:** [GitHub](https://github.com/HenryYoon) · [LinkedIn](https://linkedin.com/in/yunihg)

---

## Skills

**Languages & Frameworks:** Python, PyTorch, FastAPI, Ultralytics  
**Optimization:** ONNX, ONNXRuntime, YOLO model tuning  
**Deployment & Infra:** Docker, PyInstaller, Linux, H100/A100 GPU clusters  
**Data & Tools:** CVAT, SAM, NumPy, Git, GitHub, Slack, Jira  
**Domain:** Object Detection, Model Compression, Edge AI, Computer Vision  
**Language:** English — near-native (delivered technical presentations to Singapore government agencies)

---

## Work Experience

### AiRISS — AI Engineer (2023.05 – 2026.02)

**ONNX-based Vision AI Optimization**
- Background: PyTorch-dependent executables exceeded 2 GB, causing frequent deployment failures and compatibility issues on client machines.
- Contribution: Removed PyTorch dependency by converting inference to Numpy + ONNXRuntime. Analyzed Ultralytics source to customize ONNX build pipeline and resolve export errors.
- Result: Inference latency 600 ms → 300 ms (50% reduction); deployment size 3 GB → 700 MB (76% reduction).

**Pill Detection Model Architecture Improvement**
- Background: Small pill objects resulted in low detection precision with default YOLO architecture.
- Contribution: Categorized pill imaging cases by size, color, and shape. Proposed a per-case photography protocol to streamline data collection. Added P2 feature map to YOLOv8 backbone and applied sliding window for small-object detection.
- Result: Precision 0.60 → 0.80 (33% improvement). Reduced false positives. Research outcomes led to a government-funded project selection.

**Singapore Government PoC**
- Background: Conducted AI PoC targeting correctional facilities through a local Singapore agent.
- Contribution: Designed and developed a real-time AI demo system for on-site presentation. Led scenario planning and delivered technical presentation in English to the client.
- Result: Successful PoC delivery contributing to contract negotiations with the Singapore government agency.

**Standalone Executable Deployment Pipeline**
- Background: Docker-based deployments failed on client Windows environments, causing installation failures and increased support costs.
- Contribution: Analyzed client environments and built a PyInstaller-based single-executable pipeline. Designed a packaging structure integrating AI model and ONNX runtime dependencies.
- Result: Initial setup time 20 min → 10 min (50% reduction). Achieved zero-dependency deployment, resolving compatibility issues.

**MLOps & Data Operations Infrastructure**
- Contribution: Secured A100×4 and H100×1 GPU servers via AICA partnership, optimizing training infrastructure. Reduced model generation cycle from 1 month to 1 week.
- Contribution: Configured Redis AOF (Append Only File) on CVAT server to prevent annotation data loss and maintain recovery integrity.
- Contribution: Integrated SAM-based auto-labeling tools into CVAT to increase data preprocessing efficiency.

**Real-time API Performance Optimization**
- Background: Flask-based API response time was 3 seconds, unable to meet real-time security monitoring requirements.
- Contribution: Migrated to FastAPI with asynchronous processing architecture.
- Result: Response time 3 s → 0.5 s (83% reduction). Enabled real-time threat detection compliance.

---

## Other Experience

### Edge-Device LLM Deployment Research (2025.12 – Present)
- Analyzing feasibility and technical constraints of LLM deployment on low-power NPU accelerators (Hailo-10H).
- Fine-tuning legal domain Qwen 2.5 (3B) model using Unsloth library.
- Investigating Tensor Shape mismatch and data type incompatibility issues during Hailo compiler conversion.

### KPMG Ideathon — Team Lead (2022.12 – 2023.02)
- Led a 6-member cross-functional team (planners, designers, AI engineers) through project roadmap planning and management.
- Built and presented a Gradio-based technical demo, advancing to finals.

---

## Education

### Chung-Ang University — M.S. in Computer Engineering (2021.03 – 2023.02)
- Research: Transformer-based automated fact-checking models (Advisor: Prof. Seok-Hwan Lee)
- Thesis: Document embedding and sentiment analysis-based international issue analysis system
- Best Paper Award at KIICE Fall Conference (2021)
- Reduced Transformer training time by 3× using LSH-based attention mechanism design

### Hansung University — B.A. in Public Administration (2014.03 – 2021.02)

---

## Publication

- **Automated Fact-checking Model Using Efficient Transformers** (2021, KIICE — Best Paper Award)

---

## Projects

| Project | Description |
|---------|-------------|
| [auto-factcheck](https://github.com/HenryYoon/auto-factcheck) | Transformer-based automated fact verification system (M.S. thesis) |
| [anomaly-detection](https://github.com/HenryYoon/anomaly-detection) | Anomaly detection model training and evaluation |
| [KPMG HotSix Chat](https://github.com/kpmg-hotsix/kpmg_hotsix_chatbot) | 2023 KPMG Competition (Finalist) |
