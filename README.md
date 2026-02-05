# Internship-assignment-Titanic-Survival-Prediction---Encoding-I-
# Feature Encoding Module 🔢

This module handles the encoding of categorical features in the Titanic Survival Prediction project.  
It converts non-numeric variables into machine-learning–ready numerical features.

---

## 📌 Purpose
Machine learning models require numerical inputs.  
This encoding step transforms categorical data such as gender, cabin availability, and embarkation port into meaningful numerical representations.

---

## 🧾 Features Encoded

### 1️⃣ Gender Encoding
- `Sex` → binary encoding
  - Female → `female = 1`
  - Male → `female = 0`

---

### 2️⃣ Cabin Encoding
- Converted cabin information into a binary feature:
  - `isCabin = 1` → Passenger has a cabin assigned
  - `isCabin = 0` → No cabin information available

This helps capture survival patterns related to cabin availability.

---

### 3️⃣ Embarkation Port Encoding
One-hot encoding applied to the `Embarked` column:
- `S` → Southampton
- `C` → Cherbourg
- `Q` → Queenstown

Each port is represented as a separate binary feature.

---

## ⚙️ Encoding Techniques Used
- Binary encoding
- One-hot encoding
- Missing value handling prior to encoding

---

## 📤 Output
After encoding, the dataset contains only numerical columns suitable for:
- Feature selection
- Model training
- Prediction

Example encoded features:
```python
['female', 'isCabin', 'S', 'C', 'Q']
