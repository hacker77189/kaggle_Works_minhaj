# 🧬 NHANES-Based Age Group Classification

This project is part of **Summer Analytics 2025**, organized by the *Consulting and Analytics Club, IIT Guwahati*. The goal is to build a binary classification model that predicts whether a respondent is a **Senior (65+)** or **Adult (<65)** using a subset of health and nutrition data from the **NHANES** study by the CDC.

---

## 📝 About the Dataset

The **National Health and Nutrition Examination Survey (NHANES)** is a nationally representative health survey conducted by the CDC’s National Center for Health Statistics. It collects data via:

- 📋 In-home interviews
- 🧪 Lab tests
- 🏥 Mobile clinics

This hackathon dataset is a simplified and focused version, containing **6,287 entries** and **7 core features**, ideal for binary classification tasks in healthcare.

---

## 🎯 Objective

Predict whether a person is a **Senior (age ≥ 65)** or an **Adult (age < 65)** using health, lifestyle, and lab information.

- **Adult** → `0`
- **Senior** → `1`

⚠️ The submission format accepts **only 0 or 1**, as shown in the `sample-submission.csv`.

---

## 📁 Dataset Files

- `train.csv` – 2,016 rows with features + target (`age_group`)
- `test.csv` – 312 rows with features only (target to be predicted)
- `sample-submission.csv` – Format your submission to match this file

---

## 🔍 Features

| Column   | Description |
|----------|-------------|
| `SEQN`   | Unique identifier (Sequence number) |
| `RIAGENDR` | Gender (1 = Male, 2 = Female) |
| `PAQ605` | Physical activity indicator (moderate or vigorous activity) |
| `BMXBMI` | Body Mass Index |
| `LBXGLU` | Glucose level |
| `DIQ010` | Diabetes questionnaire response |
| `LBXGLT` | Oral glucose tolerance |
| `LBXIN`  | Insulin level |

> ⚠️ Missing values (`NaN`) may be present and must be handled appropriately (e.g., imputation, removal).

---

## 🛠️ Approach

You are encouraged to explore:

- ✅ Exploratory Data Analysis (EDA)
- ✅ Feature Engineering (transformations, binning, interaction terms)
- ✅ Handling missing data
- ✅ Applying binary classification algorithms
- ✅ Submitting results in the correct format

In case of **tie scores**, top-5 submissions will be chosen based on the quality of EDA and feature engineering techniques used.

---

## 📦 Output Format

Submit a CSV file with the following:

```
age_group
0
1
...
```

Ensure the number of predictions equals the number of rows in `test.csv`.

---

## 📬 Contact

**Minhaj Alam**  
[GitHub](https://github.com/hacker77189) | [Email](mailto:your-email@example.com)

---

## 📌 Disclaimer

This dataset is based on NHANES data, modified for educational purposes. The data is not owned by the organizers. It has been preprocessed to provide a balanced and focused challenge on binary classification and feature engineering.

---
