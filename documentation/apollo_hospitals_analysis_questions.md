# Apollo Hospitals - Appointment No-Show and Patient Engagement Analysis

## Background

Apollo Hospitals operates across 15 cities in India through a mix of in-clinic consultations, video consults, and home visits. Patients book through the Apollo App, website, call centre, walk-in, and partner apps. A significant share of booked appointments result in no-shows, which hurts doctor utilisation, revenue, and patient health outcomes. As a Data Analyst at Apollo, you are tasked with performing Exploratory Data Analysis in Python to surface actionable insights across booking behaviour, no-show patterns, patient engagement, and financial performance.

## Dataset

Two files are provided. The primary file is `apollo_appointments_fact.csv` with 75,000 rows and 52 columns, where each row is one appointment. The supporting file is `apollo_doctors_dim.csv` with 320 rows and 15 columns, where each row is one doctor. Join on `doctor_id` when doctor-level attributes like experience or rating are needed.

**Dataset Link:** [apollo hospitals - Python Project](#)

---

## Business Overview

- How is appointment volume trending across months and quarters from 2022 to 2024?
- What is the split of outcomes across completed, no-show, cancelled, and scheduled appointments?
- Which booking channels drive the highest volume and how does the channel mix look?

## No-Show Analysis

- Which specialties and cities have the highest and lowest no-show rates?
- How does booking lead time affect the probability of a no-show?
- Do evening slots, weekends, and longer-lead bookings see higher dropout?
- Which appointment types and booking channels carry the most no-show risk?

## Financial Performance

- How much revenue is being lost to no-shows?
- How does average revenue vary across specialties and appointment types?
- Which cities generate the most revenue and what is the payment mode mix?
- How does insurance coverage affect what patients pay out of pocket?

## Doctor Utilisation and Service Quality

- Which specialties have the highest and lowest doctor utilisation rates?
- How long are patients waiting and does it vary by specialty or time of day?
- Is there a relationship between consultation duration and patient satisfaction?
- How does doctor experience relate to the fee charged (join with doctors dim)?

## Reminder and Engagement Effectiveness

- How much does reminder type reduce no-show rates compared to no-reminder patients?
- Does prior no-show history predict future no-show behaviour?
- Do Apollo members and repeat patients show better attendance than non-members and first-time patients?

## Patient and Demographic Segmentation

- How do age group, gender, and chronic condition status influence no-show likelihood?
- Which visit reasons are most common and are some associated with higher dropout?
- What does the patient age distribution look like within specialties like Paediatrics, Gynaecology, and Psychiatry?

---

## Important Notes

Quality metric columns like wait time, satisfaction, consultation duration, and utilisation are null for all non-Completed rows. Always filter on Completed status before analysing these.

Revenue columns are zero for non-Completed rows so scope all revenue analysis to Completed only.

For no-show rate, always divide no-show count by the total of Completed plus No-Show plus Cancelled rows, excluding Scheduled.

The value `None` in chronic condition, membership type, insurance provider, and cancellation reason means the field does not apply and is not a missing value.
