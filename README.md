# Apollo Hospitals — Appointment No-Show & Patient Engagement Analysis

An end-to-end Python Exploratory Data Analysis (EDA) project focused on understanding appointment behaviour, no-show patterns, patient engagement, revenue performance, and doctor utilisation for Apollo Hospitals.

## 📌 Project Overview

Apollo Hospitals operates across multiple cities in India through in-clinic consultations, video consultations, and home visits. Patients can book appointments through different channels including the Apollo App, website, call centre, walk-ins, and partner applications.

This project analyses appointment-level data to identify patterns related to:

- Appointment volume and trends
- Completed, no-show, cancelled, and scheduled appointments
- Booking channels
- No-show behaviour
- Booking lead time
- Appointment types and time slots
- Revenue performance
- Doctor utilisation
- Patient waiting time
- Patient satisfaction
- Reminder effectiveness
- Patient engagement
- Demographic segmentation

## 🎯 Business Objectives

The analysis is designed to answer important business questions such as:

- How does appointment volume change across months and quarters?
- Which booking channels generate the highest appointment volume?
- Which specialties and cities have higher or lower no-show rates?
- How does booking lead time relate to no-show behaviour?
- Which appointment types and booking channels have higher no-show risk?
- How much revenue is associated with completed appointments and no-shows?
- How does doctor experience relate to consultation fees?
- Do reminders influence appointment attendance?
- Does previous no-show behaviour relate to future attendance?
- How do membership, repeat visits, age group, gender, and chronic-condition status relate to appointment behaviour?

## 📊 Datasets

### 1. Appointments Fact Dataset

"apollo_appointments_fact.csv"

- 75,000 rows
- 52 columns
- One row represents an appointment event.

The dataset contains appointment dates, booking information, patient attributes, appointment outcomes, financial information, reminders, waiting time, consultation duration, satisfaction, and doctor utilisation metrics.

### 2. Doctors Dimension Dataset

"apollo_doctors_dim.csv"

- 320 rows
- 15 columns
- One row represents a doctor.

The doctor dataset contains doctor information such as specialty, qualification, experience, consultation fee, rating, reviews, availability, insurance acceptance, and teleconsultation availability.

The two datasets can be joined using "doctor_id".

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
## 🔍 Analysis Areas

### Business Overview

Appointment trends, appointment outcomes, and booking-channel distribution.

### No-Show Analysis

No-show behaviour across specialties, cities, booking lead time, time of day, appointment types, and booking channels.

### Financial Performance

Revenue, consultation fees, insurance coverage, patient out-of-pocket payments, and payment modes.

### Doctor Utilisation & Service Quality

Doctor utilisation, patient waiting time, consultation duration, satisfaction, and doctor experience.

### Reminder & Patient Engagement

Reminder effectiveness, previous no-show history, Apollo membership, and repeat-patient behaviour.

### Patient & Demographic Segmentation

Age groups, gender, chronic-condition status, visit reasons, and specialty-level patient demographics.

## ⚠️ Data Analysis Notes

For accurate analysis:

- Quality metrics such as waiting time, satisfaction, consultation duration, and doctor utilisation should be analysed for Completed appointments.
- Revenue-related analysis should focus on Completed appointments.
- No-show rate should exclude Scheduled appointments from the denominator.
- The value "None" in fields such as chronic condition, membership type, insurance provider, and cancellation reason represents a non-applicable value rather than a missing value.

## 📓 Main Notebook

The complete structured analysis is available in:

"notebooks/apollo_hospital_professional.ipynb"

The notebook contains the project analysis in a structured format along with the business questions being investigated.

## 📚 Documentation

Additional project documentation is available in the "documentation/" folder:

- Analysis Questions — business questions addressed by the project
- Data Dictionary — definitions and descriptions of dataset columns

## 👤 Project

### Apollo Hospitals — Appointment No-Show & Patient Engagement Analysis

Built as a Python-based Data Analytics / Exploratory Data Analysis project.
