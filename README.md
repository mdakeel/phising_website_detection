
# 🛡️ Phishing Website Detection Using Machine Learning
##Landing Page :
<img width="1903" height="961" alt="Screenshot 2025-08-06 122446" src="https://github.com/user-attachments/assets/bf9bc207-8019-48ce-a582-23bc8260926a" />

##Upload CSV file
<img width="1905" height="834" alt="image" src="https://github.com/user-attachments/assets/cf185a13-56f3-407f-8eb9-fccb7c66a3d5" />

##Website link dectectin , Phising or Safe
<img width="1890" height="950" alt="image" src="https://github.com/user-attachments/assets/6200785c-2e8b-43d6-8c3e-3f319e1fefcc" />


## 🔍 Overview of the Problem

### What is Phishing?
- A cyber-attack where fraudulent websites steal sensitive information.

### Why is it Important?
- Protects users from scams, financial loss, and identity theft.

### Role of Machine Learning
- Automates phishing detection using website features.

---

## 📊 Dataset Overview

- **Source**: [Kaggle Dataset](https://www.kaggle.com/datasets/sai10py/phishing-websites-data)
- **Total Columns**: 31 (30 Features + 1 Target)
- **Target Variable**: `Result`  
  - `-1` → Phishing  
  - `1` → Legitimate

### Feature Categories:
- **URL-Based**:  
  `having_IP_Address`, `URL_Length`, `Shortening_Service`, `having_At_Symbol`, `Prefix_Suffix`, `double_slash_redirecting`

- **Domain-Based**:  
  `SSLfinal_State`, `Domain_registeration_length`, `age_of_domain`, `DNSRecord`, `having_Sub_Domain`

- **Content-Based**:  
  `Request_URL`, `URL_of_Anchor`, `Links_in_tags`, `Favicon`, `port`, `HTTPS_token`

---

## 🧹 Data Preprocessing

- Handling missing values  
- Converting categorical data  
- Normalizing feature values  
- Splitting into training & testing sets

---

## 🤖 Model Selection & Training

Popular ML models used:
- Logistic Regression  
- Random Forest  
- Support Vector Machine (SVM)  
- Gradient Boosting (XGBoost)

---

## 📈 Model Evaluation

- Metrics: Accuracy, Precision, Recall, F1-score  
- Confusion Matrix for analyzing false positives/negatives

---

## 🚀 Project Flow & Deployment

1. Introduction  
2. Environment Setup  
3. Dataset Exploration  
4. Data Preprocessing  
5. Feature Engineering  
6. Model Training & Evaluation  
7. FastAPI Deployment  
8. Docker Containerization  
9. Cloud Deployment  
10. CI/CD with GitHub Actions  
11. Terraform Infrastructure  
12. Final Wrap-Up

---

## 🧠 Feature Descriptions

### URL-Based Features
- `Prefix_Suffix`: Checks for hyphens in domain names  
- `double_slash_redirecting`: Detects suspicious redirects  
- `having_At_Symbol`: Flags deceptive use of `@` in URLs  
- `Shortining_Service`: Identifies shortened URLs  
- `URL_Length`: Measures URL length  
- `having_IP_Address`: Detects use of IP instead of domain

### Domain-Based Features
- `having_Sub_Domain`: Evaluates subdomain count  
- `SSLfinal_State`: Validates SSL certificate  
- `Domain_registeration_length`: Measures domain lifespan  
- `age_of_domain`: Age of domain in days  
- `DNSRecord`: Checks for valid DNS records

### Webpage-Based Features
- `Favicon`: External favicon detection  
- `port`: Flags suspicious ports  
- `HTTPS_token`: Detects deceptive use of "HTTPS"  
- `Request_URL`: External resource loading  
- `URL_of_Anchor`: Trustworthiness of anchor links  
- `Links_in_tags`: Checks `<meta>`, `<script>`, `<link>` tags

---


