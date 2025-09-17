# 🎓 Undergraduate Projects Repository  

This repository showcases two major machine learning projects completed during my undergraduate studies at **Bowling Green State University**.  

Each project explores different aspects of applied AI/ML — from **human-centered explainability and fairness** to **object detection and domain generalization**.  

---

## Project 1: Human-Centered XAI Impact Assessment Framework  
**Team:** Group 07 — *Gary Brammer, Nathan Shafer, Vy Nguyen*  
**Dataset:** [UCI Adult Dataset](https://archive.ics.uci.edu/ml/datasets/adult)  
**Focus:** Explainable AI (XAI), Fairness, Transparency  

### Overview  
We developed a **human-centered framework** to assess the impact of XAI methods on fairness, interpretability, and usability.  
Using the UCI Adult dataset (income prediction), we evaluated how methods like **SHAP**, **LIME**, and **PDP** reveal or mitigate bias — and whether explanations are meaningful to human decision-makers.  

### Key Contributions  
- **Fairness & Bias Analysis**  
  - Gender disparity in prediction rates: **9.7%**  
  - Accuracy gap of **10.8%** between White and Black participants:contentReference[oaicite:0]{index=0}:contentReference[oaicite:1]{index=1}  
- **Explainability Insights**  
  - SHAP → marital status (0.14) & education (0.11) = strongest predictors  
  - LIME → contradictory feature effects in ~17% of cases  
  - Counterfactuals → marital status flips predictions for ~34% near decision boundary:contentReference[oaicite:2]{index=2}  
- **Evaluation Pipeline**  
  - Modular Python framework: preprocessing, fairness metrics, XAI methods  
  - Dashboard for subgroup fairness + interpretability:contentReference[oaicite:3]{index=3}  

### Tools & Tech  
- Python (scikit-learn, SHAP, LIME, imbalanced-learn)  
- Jupyter Notebooks  
- JSON artifacts + visualization for interactive dashboards  

---

## Project 2: YOLOv8 Object Detection – Cross-Domain Performance Analysis  
**Team:** *Nathan Shafer & Evan Sluterbeck*  
**Dataset:** [BDD100k](https://bdd-data.berkeley.edu/) + custom local images  
**Focus:** Object Detection, Domain Shift, Real-World Generalization  

### Overview  
This project tested how well **YOLOv8s**, trained on the BDD100k dataset, generalized to **real-world environments**.  
We ran inference on both still images and live camera captures to evaluate **domain shift** — the impact of lighting, weather, and environment on detection reliability.  

### Key Contributions  
- **Model Training**  
  - YOLOv8s (11.2M params, 22MB) with pretrained weights  
  - 300 training epochs, cosine learning rate decay, extensive augmentations:contentReference[oaicite:4]{index=4}:contentReference[oaicite:5]{index=5}  
- **Results**  
  - Precision peaked at **0.73** (epoch 40)  
  - Recall improved from 0.35 → 0.48  
  - F1 stabilized at 0.57  
  - mAP50 reached **0.52**:contentReference[oaicite:6]{index=6}:contentReference[oaicite:7]{index=7}  
- **Domain Shift Findings**  
  - Still images (daytime) → strong detection accuracy  
  - Live camera (overcast, variable lighting) → reduced accuracy & confidence  
  - Same location yielded different results depending on conditions:contentReference[oaicite:8]{index=8}  
- **Future Improvements**  
  - Early stopping (~220 epochs)  
  - Fine-tuned class loss weights & confidence thresholds  
  - Balance training data distribution  

### 🛠 Tools & Tech  
- Python + Ultralytics YOLOv8  
- CUDA GPU acceleration (RTX 4060, 8GB VRAM)  
- OpenCV for inference (still & live capture)  
- Matplotlib / Seaborn for metrics visualization  

---

## Results Summary  

| Project              | Team                               | Dataset                 | Focus                           | Key Findings |
|----------------------|------------------------------------|-------------------------|--------------------------------|--------------|
| Human-Centered XAI   | Gary Brammer, Nathan Shafer, Vy Nguyen | UCI Adult               | Explainability & Fairness       | Detected systemic gender & race disparities; built fairness-aware XAI framework:contentReference[oaicite:9]{index=9}:contentReference[oaicite:10]{index=10} |
| YOLOv8 Detection     | Nathan Shafer, Evan Sluterbeck     | BDD100k + Local Images  | Object Detection & Domain Shift | Achieved high precision (0.73) but lower recall (0.48); live testing showed strong environmental sensitivity:contentReference[oaicite:11]{index=11}:contentReference[oaicite:12]{index=12} |

---

