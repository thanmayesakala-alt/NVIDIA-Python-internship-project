# 🚗 CAN-IDS: In-Vehicle Network Intrusion Detection System

An interactive web-based Intrusion Detection System (IDS) for Controller Area Network (CAN) traffic using Tree-Based Ensemble Machine Learning techniques.

The application demonstrates the complete IDS workflow—from CAN log ingestion and preprocessing to model training, evaluation, and multi-threat detection—through an intuitive browser interface.

---

## 📌 Features

- 📂 Upload CAN log datasets
- 🔍 Supports multiple log formats
  - CSV
  - JSON
  - TXT
  - Linux `candump` logs
- ⚙️ Automatic CAN message parsing
- 📊 Shannon Entropy based feature extraction
- 📈 Sliding Window preprocessing
- 🌲 Random Forest Classifier
- 🌳 Extra Trees Classifier
- 📉 ROC Curve visualization
- 📊 Confusion Matrix metrics
- 🚨 Multi-threat detection dashboard
- 🎯 Interactive IDS workflow

---

## Project Workflow

```
CAN Log Files
      │
      ▼
Data Ingestion
      │
      ▼
Smart Log Parser
      │
      ▼
Feature Extraction
(Entropy + Time Delta)
      │
      ▼
Tree Ensemble Model
(Random Forest / Extra Trees)
      │
      ▼
Performance Evaluation
      │
      ▼
Threat Detection
```

---

## Detection Capabilities

The system can identify:

- ✅ Normal Traffic
- 🚨 DoS Attack
- ⚠️ Gear Spoofing
- ⚠️ RPM Spoofing
- 🚨 Fuzzy Attack

---

## Project Phases

### Phase 1 — Data Ingestion

Upload multiple CAN datasets including:

- Normal Traffic
- DoS Attack
- Gear Spoofing
- Fuzzy Attack
- RPM Spoofing

---

### Phase 2 — Feature Extraction

Extracts statistical features including:

- Shannon Entropy
- Mean Message Delta Time
- Dominant CAN ID
- Window Message Count

Sliding Window preprocessing is used before model training.

---

### Phase 3 — Model Training

Supported classifiers:

- Random Forest
- Extra Trees

Adjustable parameters:

- Number of Trees
- Maximum Depth

---

### Phase 4 — Performance Evaluation

Displays:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC Curve
- AUC Score
- Confusion Matrix

---

### Phase 5 — Multi-Threat Detection

Real-time analysis of mixed CAN traffic.

Threats detected include:

- DoS Flooding
- RPM Spoofing
- Gear Spoofing
- Fuzzy Attacks

Each detected event includes:

- Severity
- Description
- Dominant CAN ID
- Entropy
- Mean Time Delta

---

## Supported Input Formats

### CSV

```csv
timestamp,id,dlc,data,label
1625097600.001,0x158,8,00 AA FF 00 23 11 C2 54,Normal
```

### JSON

```json
[
  {
    "timestamp":1625097600.001,
    "id":"0x158",
    "dlc":8,
    "data":["00","AA","FF","00","23","11","C2","54"]
  }
]
```

### Linux candump

```text
(1625097600.001) can0 158#00AAFF002311C254
```

---

## Technologies Used

- React 18
- Tailwind CSS
- JavaScript (ES6)
- HTML5
- Browser File API
- SVG Graphics

---

## Machine Learning Concepts

- Tree-Based Ensemble Learning
- Random Forest
- Extra Trees
- Sliding Window Processing
- Shannon Entropy
- Statistical Feature Engineering
- Binary Classification
- Multi-Class Classification
- ROC Analysis

---

## Folder Structure

```
project/
│
├── index.html
├── README.md
└── assets/
```

---

## How to Run

1. Clone the repository

```bash
git clone https://github.com/yourusername/can-ids.git
```

2. Open the project folder

```bash
cd can-ids
```

3. Open `index.html` in your browser.

No installation is required because the project uses CDN-hosted React and Tailwind CSS.

---

## Screenshots

Add screenshots such as:

- Home Page
- Dataset Upload
- Feature Extraction
- Model Training
- ROC Curve
- Metrics Dashboard
- Multi-Threat Detection

---

## Future Improvements

- TensorFlow.js integration
- XGBoost support
- Live SocketCAN monitoring
- Real-time CAN interface
- Model export/import
- Dataset management
- Authentication
- Backend API
- Database integration

---

## Learning Objectives

This project demonstrates:

- CAN Bus security
- Automotive cybersecurity
- Intrusion Detection Systems (IDS)
- Ensemble Machine Learning
- Feature Engineering
- Interactive data visualization
- Browser-based analytics

---

## License

This project is intended for educational and research purposes.

---

## Author

**Your Name**

GitHub: https://github.com/yourusername

---

## Acknowledgements

- React
- Tailwind CSS
- Automotive Cybersecurity Research
- CAN Bus Protocol
- Machine Learning Community

---

⭐ If you found this project useful, consider giving it a star on GitHub!
