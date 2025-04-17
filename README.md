# IITM-MLP-Project
System Threat Classifier (Supervised Learning - Classification)

# 🛡️ MLP Project T12025 - Malware Prediction

## 📌 Project Overview

This repository contains my submission for the **MLP Project T12025** Machine Learning competition.  
The task is to **predict whether a system is infected by malware** using telemetry data collected by antivirus software.

Each participant is required to:
- Build a classification model.
- Predict the `target` column for the given `test.csv`.
- Submit predictions in the correct format (`id`, `target`) as demonstrated in `sample_submission.csv`.

---

## 📂 Dataset Description

- `train.csv`: Training dataset with features and `target`.
- `test.csv`: Test dataset without `target`.
- `sample_submission.csv`: Shows the correct format for submission.

### ✅ Target
- `target`: Binary value (1 = Malware detected, 0 = No malware detected).

### 🔑 Key Features
Examples of features in the dataset:
- System specs: `Processor`, `PrimaryDiskType`, `TotalPhysicalRAMMB`
- Software info: `ProductName`, `AppVersion`, `OSVersion`, `EngineVersion`
- Security settings: `IsBetaUser`, `IsSystemProtected`, `FirewallEnabled`, `IsSecureBootEnabled`
- Location/Region: `CountryID`, `CityID`, `GeoRegionID`
- User behavior/environment: `SMode`, `IsGamer`, `FlightRing`, `LicenseActivationChannel`

For a full list of features, refer to the competition instructions.

---

## 🧠 Model Overview

The notebook includes:
- Data loading and cleaning
- Handling missing values
- Encoding categorical variables
- A baseline ML model (e.g., Logistic Regression / Random Forest / DummyClassifier)
- Predicting on test data
- Generating submission file
