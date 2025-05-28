# 🧾 Automatic Ticket Classification using Topic Modeling & Supervised Learning

This project aims to build an **automatic ticket classification system** for a financial company using **Natural Language Processing (NLP)** techniques. The objective is to classify unstructured customer complaints into relevant product or service categories, improving support efficiency and customer satisfaction.

---

## 📌 Problem Statement

Financial companies receive thousands of unstructured complaints related to various services like **credit cards**, **bank accounts**, **mortgages**, etc. Manually assigning each ticket to the correct department is time-consuming and error-prone.

As an NLP engineer, your task is to automate this classification process. You'll use **Non-negative Matrix Factorization (NMF)** for **topic modeling**, and later build supervised classification models to assign new complaints to predefined categories.

---

## 🎯 Business Objective

- **Automatically classify** customer complaints into service categories.
- Use **NMF topic modeling** to identify patterns in unlabeled complaints.
- Build **supervised machine learning models** for accurate prediction.
- Improve the **turnaround time** and **accuracy** of complaint resolution.

---

## 🧰 Tools & Technologies

- Python
- Pandas, NumPy
- Scikit-learn
- NLTK, SpaCy
- Matplotlib, Seaborn
- JSON for data ingestion

---

## 📁 Dataset

- Format: `.json`
- Total Complaints: **78,313**
- Features: **22**
- Each record is a **customer complaint ticket** with details like complaint text, date, product type, etc.

---

## ✅ Expected Categories (Labels)

The complaints should be classified into the following **five clusters**:

1. Credit card / Prepaid card  
2. Bank account services  
3. Theft / Dispute reporting  
4. Mortgages / Loans  
5. Others  

---

## 📌 Project Tasks

The assignment is divided into the following major steps:

1. **Data Loading**  
   - Load `.json` data into a DataFrame  
   - Basic data inspection  

2. **Text Preprocessing**  
   - Clean text: remove noise, special characters  
   - Lemmatization & POS tagging  

3. **Exploratory Data Analysis (EDA)**  
   - Word count distributions  
   - Common bigrams/trigrams  

4. **Feature Extraction**  
   - Use **TF-IDF Vectorization** to convert text into numerical features  

5. **Topic Modeling**  
   - Apply **NMF** to group tickets into 5 topics  
   - Assign topic labels to tickets  
   - Interpret clusters and map them to service categories  

6. **Supervised Model Building**  
   - Use labeled data from NMF to train models  
   - Try at least 3 models:
     - Logistic Regression
     - Decision Tree
     - Random Forest
     - (Optional) Naive Bayes

7. **Model Evaluation**  
   - Use metrics like Accuracy, Precision, Recall, F1 Score  
   - Confusion Matrix to visualize performance  

8. **Inference**  
   - Test model on new, custom complaint text  

---

## 🧪 Evaluation Rubrics

| Stage                      | Weightage | Description                                                                 |
|---------------------------|-----------|-----------------------------------------------------------------------------|
| Data Reading/Understanding| 5%        | Load and inspect JSON data                                                 |
| Data Cleaning             | 10%       | Remove missing values, rename columns, clean text                          |
| Preprocessing             | 10%       | Lemmatization, POS tagging                                                 |
| Visualization             | 10%       | Word clouds, n-gram plots                                                  |
| Feature Extraction        | 5%        | TF-IDF vectorization                                                       |
| Topic Modeling            | 25%       | NMF to find 5 clusters, map to categories                                  |
| Model Building            | 20%       | Train multiple models and evaluate                                         |
| Model Inference           | 5%        | Predict topic of a new, unseen complaint                                   |
| Code Quality              | 10%       | Commented, readable, and well-structured code                              |

---
