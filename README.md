# Apollo Hospitals — Appointment No-Show & Patient Engagement Analysis

An end-to-end **Python Exploratory Data Analysis (EDA)** project focused on understanding appointment behaviour, no-show patterns, patient engagement, revenue performance, and doctor utilisation for Apollo Hospitals.

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-green)
![NumPy](https://img.shields.io/badge/NumPy-Data%20Analysis-blue)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-yellow)
![Seaborn](https://img.shields.io/badge/Seaborn-Visualization-lightblue)

---

## 📑 Table of Contents

- [Project Overview](#-project-overview)
- [Project Highlights](#-project-highlights)
- [Business Objectives](#-business-objectives)
- [Datasets](#-datasets)
- [Tools & Technologies](#️-tools--technologies)
- [Project Structure](#-project-structure)
- [Analysis Areas](#-analysis-areas)
- [Data Analysis Notes](#️-data-analysis-notes)
- [Main Notebook](#-main-notebook)
- [Documentation](#-documentation)
- [Analysis Scope](#-analysis-scope)
- [Project Workflow](#-project-workflow)
- [Project](#-project)

---

## 📌 Project Overview

Apollo Hospitals operates across multiple cities in India through in-clinic consultations, video consultations, and home visits.

Patients can book appointments through multiple channels including:

- Apollo App
- Website
- Call Centre
- Walk-In
- Partner App

This project analyses appointment-level data to understand:

- Appointment volume and trends
- Appointment outcomes
- No-show behaviour
- Booking patterns
- Patient engagement
- Revenue performance
- Doctor utilisation
- Service quality
- Reminder effectiveness
- Patient and demographic segmentation

---

## ⭐ Project Highlights

- **75,000 appointment records** analysed
- **320 doctors** included in the supporting dimension dataset
- Appointment outcome analysis
- No-show behaviour analysis
- Booking-channel analysis
- Booking lead-time analysis
- Revenue and insurance analysis
- Doctor utilisation analysis
- Patient waiting-time analysis
- Consultation and satisfaction analysis
- Reminder effectiveness analysis
- Patient engagement analysis
- Demographic segmentation
- Structured Python EDA workflow

---

## 🎯 Business Objectives

The analysis is designed to answer important business questions such as:

- How does appointment volume change across months and quarters?
- What is the distribution of completed, no-show, cancelled, and scheduled appointments?
- Which booking channels generate the highest appointment volume?
- Which specialties and cities have higher or lower no-show rates?
- How does booking lead time relate to no-show behaviour?
- Do evening slots and weekends show different attendance patterns?
- Which appointment types and booking channels have higher no-show risk?
- How does revenue vary across specialties and appointment types?
- Which cities generate the most revenue?
- How does insurance coverage affect patient out-of-pocket payments?
- Which specialties have different doctor utilisation patterns?
- How does patient waiting time vary?
- Is consultation duration related to patient satisfaction?
- How does doctor experience relate to consultation fees?
- How effective are appointment reminders?
- Does previous no-show history relate to future attendance?
- Do members and repeat patients show different attendance patterns?
- How do age group, gender, and chronic-condition status relate to no-show behaviour?

---

## 📊 Datasets

### 1. Appointments Fact Dataset

**File:** `apollo_appointments_fact.csv`

- **75,000 rows**
- **52 columns**
- One row represents an appointment event.

The dataset contains appointment dates, booking information, patient attributes, appointment outcomes, financial information, reminders, waiting time, consultation duration, satisfaction, and doctor utilisation metrics.

### 2. Doctors Dimension Dataset

**File:** `apollo_doctors_dim.csv`

- **320 rows**
- **15 columns**
- One row represents a doctor.

The dataset contains doctor information such as:

- Doctor name
- Specialty
- Qualification
- Experience
- City
- Hospital
- Consultation fee
- Rating
- Total reviews
- Availability
- Insurance acceptance
- Teleconsultation availability

The datasets can be joined using `doctor_id`.

---

## 🛠️ Tools & Technologies

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Exploratory Data Analysis
- Data Cleaning
- Data Transformation
- Data Visualization
- Business Analysis

---

## 📁 Project Structure

```text
apollo-hospitals-appointment-analysis/
│
├── 📊 data/
│   ├── apollo_appointments_fact.csv
│   └── apollo_doctors_dim.csv
│
├── 📚 documentation/
│   ├── apollo_hospitals_analysis_questions.md
│   └── Data Dictionary.docx
│
├── 📓 notebooks/
│   └── apollo_hospital_professional.ipynb
│
└── 📄 README.md
```

---

## 🔍 Analysis Areas

### 📊 Business Overview

- Appointment volume trends across months and quarters
- Appointment outcome distribution
- Booking-channel analysis

### 🚫 No-Show Analysis

- No-show rates across specialties and cities
- Booking lead-time analysis
- Time-of-day analysis
- Weekend appointment behaviour
- Appointment-type analysis
- Booking-channel patterns

### 💰 Financial Performance

- Revenue analysis
- Consultation fee analysis
- Insurance coverage
- Patient out-of-pocket payments
- Payment-mode analysis

### 👨‍⚕️ Doctor Utilisation & Service Quality

- Doctor utilisation
- Patient waiting time
- Consultation duration
- Patient satisfaction
- Doctor experience
- Consultation fees

### 🔔 Reminder & Patient Engagement

- Reminder effectiveness
- Previous no-show behaviour
- Apollo membership
- Repeat-patient behaviour

### 👥 Patient & Demographic Segmentation

- Age-group analysis
- Gender analysis
- Chronic-condition status
- Visit reasons
- Specialty-level demographic patterns

---

## ⚠️ Data Analysis Notes

For accurate analysis:

- Quality metrics such as **wait time, satisfaction, consultation duration, and doctor utilisation** should be analysed only for **Completed** appointments.
- Revenue-related analysis should focus on **Completed** appointments.
- For **no-show rate**, Scheduled appointments should be excluded from the denominator.
- The value `None` in fields such as chronic condition, membership type, insurance provider, and cancellation reason represents a **non-applicable value**, not a missing value.

---

## 📓 Main Notebook

The complete structured analysis is available in the main professional Jupyter Notebook.

👉 [Open Professional Analysis Notebook](notebooks/apollo_hospital_professional.ipynb)

The notebook contains the structured Python analysis along with the business questions being investigated.

---

## 📚 Documentation

Additional project documentation is available below:

- 📋 [Analysis Questions](documentation/apollo_hospitals_analysis_questions.md)
- 📖 [Data Dictionary](documentation/Data%20Dictionary.docx)

---

## 📈 Analysis Scope

| Area | Focus |
|---|---|
| Appointment Trends | Monthly and quarterly appointment patterns |
| No-Show Analysis | Attendance and dropout behaviour |
| Booking Behaviour | Booking channel and lead-time patterns |
| Financial Analysis | Revenue, fees and insurance |
| Doctor Analysis | Utilisation and experience |
| Service Quality | Waiting time and satisfaction |
| Engagement | Reminders, membership and repeat visits |
| Demographics | Age, gender and patient characteristics |

---

## 🚀 Project Workflow

```text
Data
  ↓
Data Understanding
  ↓
Data Cleaning
  ↓
Data Preparation
  ↓
Exploratory Data Analysis
  ↓
Statistical & Business Analysis
  ↓
Data Visualization
  ↓
Business Insights
```

---

## 📂 Repository Contents

### Dataset

- `apollo_appointments_fact.csv`
- `apollo_doctors_dim.csv`

### Notebook

- `apollo_hospital_professional.ipynb`

### Documentation

- `apollo_hospitals_analysis_questions.md`
- `Data Dictionary.docx`

---

## 👤 Project

**Apollo Hospitals — Appointment No-Show & Patient Engagement Analysis**

Built as a Python-based **Data Analytics / Exploratory Data Analysis** project.

---
