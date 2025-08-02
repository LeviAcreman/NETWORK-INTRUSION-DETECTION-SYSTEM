
# 🛡️ Network Intrusion Detection System (NIDS) using IBM Watsonx.ai

A cloud-based, intelligent **Network Intrusion Detection System (NIDS)** designed to classify cyberattacks such as DoS, Probe, R2L, and U2R in real-time using machine learning. Built and deployed using **IBM Watsonx.ai AutoAI** and trained on the NSL-KDD dataset.

---

## 📌 Table of Contents

- [🚨 Problem Statement](#-problem-statement)
- [✅ Proposed Solution](#-proposed-solution)
- [🧠 System Development Approach](#-system-development-approach)
- [📊 Algorithm & Deployment](#-algorithm--deployment)
- [📈 Results](#-results)
- [📌 Conclusion](#-conclusion)
- [🔮 Future Scope](#-future-scope)
- [🔗 References](#-references)

---

## 🚨 Problem Statement

Modern networks are constantly exposed to a wide range of cyberattacks. Manual detection methods are ineffective for large-scale, real-time environments. This project aims to **automatically detect and classify network intrusions** using machine learning to enhance cyber defense.

---

## ✅ Proposed Solution

The proposed solution is a **cloud-based NIDS using IBM Watsonx.ai AutoAI**, which includes:

- 🔍 **Data Source**: [NSL-KDD dataset from Kaggle](https://www.kaggle.com/datasets/sampadab17/network-intrusion-detection)
- 🧹 **Preprocessing**:
  - Encode categorical features (`protocol_type`, `flag`, etc.)
  - Normalize numerical features
  - Handle class imbalance using SMOTE or undersampling
- 🤖 **Modeling with AutoAI**:
  - Automatic data splitting, feature selection, model selection (e.g., Random Forest, XGBoost), and hyperparameter tuning
- ☁️ **Deployment**:
  - Best model deployed on IBM Watson Machine Learning as a web service

---

## 🧠 System Development Approach

- **Dataset**: [NSL-KDD](https://www.kaggle.com/datasets/sampadab17/network-intrusion-detection)
- **Platform**: IBM Watsonx.ai & Watson Studio
- **Tools**:
  - AutoAI for automated ML
  - Cloud Object Storage for dataset management

---

## 📊 Algorithm & Deployment

### 🧪 AutoAI Workflow:
- Splits dataset into training and testing sets
- Automatically performs:
  - Categorical encoding
  - Feature scaling
  - Hyperparameter optimization
  - Algorithm benchmarking

### 🔧 Features:
- 41 input features used: protocol attributes, service types, connection stats, flags, etc.

### 🛰️ Prediction Pipeline:
- JSON input with 41 fields representing real-time or batch network traffic
- Output: Predicted class → Normal / DoS / Probe / R2L / U2R

---

## 📈 Results

> The AutoAI-generated pipeline achieved **high classification accuracy** across all attack categories, showcasing the effectiveness of automated ML in cybersecurity use cases.

---

## 📌 Conclusion

- ✅ Successfully implemented and deployed a cloud-based NIDS using IBM Watsonx.ai.
- 🚀 Leveraged AutoAI to automate model training, evaluation, and deployment.
- 🔒 Achieved robust performance in detecting various attack types in network traffic.

---

## 🔮 Future Scope

- 🌐 **Real-Time Traffic Monitoring**: Integration with Wireshark, Zeek, or custom sniffers.
- 📡 **Threat Intelligence Feeds**: Enhance detection of zero-day threats.
- 🔁 **Auto Retraining**: Periodic model updates based on new labeled data.
- 🧩 **Visualization & Alerts**: Build a security dashboard for anomaly alerts.
- ☁️ **Production Deployment**: Use IBM Code Engine or Kubernetes for scalability.
- 📱 **Edge Integration**: Extend to edge devices for IoT security.

---

## 🔗 References

- 📚 [IBM Watsonx.ai AutoAI Documentation](https://dataplatform.cloud.ibm.com/docs/content/wsj/autoai/)
- 📁 [Kaggle - NSL-KDD Dataset](https://www.kaggle.com/datasets/sampadab17/network-intrusion-detection)

---

> 🧑‍💻 **Presented by**: Amit Kumar Bhardwaj  
> 🎓 **Degree**: Bachelor of Computer Applications (IGNOU)  
> 📅 **Capstone Project - 2025**
