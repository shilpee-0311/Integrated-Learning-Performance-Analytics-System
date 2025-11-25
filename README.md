Integrated Learning & Performance Analytics System
Advanced Academic • Business • Engagement Intelligence Platform for Mindsprout | Aptech | BioskoolUP
<p align="center"> <img src="https://img.shields.io/badge/Python-0D1117?style=for-the-badge&logo=python&logoColor=3776AB"> <img src="https://img.shields.io/badge/Power%20BI-0D1117?style=for-the-badge&logo=powerbi&logoColor=F2C811"> <img src="https://img.shields.io/badge/OpenCV-0D1117?style=for-the-badge&logo=opencv&logoColor=white"> <img src="https://img.shields.io/badge/Excel%20MIS-0D1117?style=for-the-badge&logo=microsoftexcel&logoColor=1D6F42"> </p> <p align="center"> <img src="https://img.shields.io/badge/Status-Production%20Ready-22c55e?style=flat-square"> <img src="https://img.shields.io/badge/Dataset-300%2B%20Learners-blue?style=flat-square"> </p>
📘 Project Overview

The Integrated Learning & Performance Analytics System is a complete academic & business intelligence platform designed for:

Mindsprout Career Hub

Aptech Learning Alambagh

BioskoolUP

This system unifies student performance analytics, batch quality monitoring, revenue tracking, trainer analysis, and social media growth into a single data-driven platform.

It includes:

ETL pipelines

KPI engineering

Behavior analysis using OpenCV

Power BI dashboards

Excel MIS automation

Cross-platform social media analytics

Built as a fully operational intelligence ecosystem.

🛠️ Tech Stack (Technical Overview)
🔹 Core

Python 3.10+

Power BI Desktop

OpenCV 4.x

Excel (Advanced Reporting)

🔹 Python Libraries
Category	Libraries
Data Manipulation	Pandas, NumPy
Visualization	Matplotlib, Seaborn
Automation	openpyxl, os, schedule
AI / CV	OpenCV, cvzone
🔹 Data Sources

Student registration data

Attendance logs

Fee data

Course & batch details

Trainer rating sheets

Social media analytics exports

🗂️ Project Architecture
Integrated-Learning-Analytics/
│
├── data/
│   ├── students.csv
│   ├── batches.csv
│   ├── attendance.xlsx
│   ├── fees.xlsx
│   ├── trainers.csv
│   └── social_media/
│       ├── instagram.csv
│       ├── youtube.csv
│       ├── facebook.csv
│       └── linkedin.csv
│
├── etl/
│   ├── student_cleaner.py
│   ├── batch_formatter.py
│   ├── fee_cleaner.py
│   └── attendance_processor.py
│
├── models/
│   ├── dropout_score.py
│   ├── efficiency_score.py
│   ├── bqi.py
│   └── engagement_model.py
│
├── reports/
│   ├── fee_pending_report.xlsx
│   ├── attendance_mis.xlsx
│   ├── monthly_performance.xlsx
│   └── top_performers.xlsx
│
├── dashboards/
│   ├── student_performance.pbix
│   ├── batch_quality.pbix
│   ├── trainer_analysis.pbix
│   └── revenue_dashboard.pbix
│
└── engagement/
    └── opencv_engagement_tracker.py

⭐ Key Features (Deep Technical Breakdown)
🧩 1. Data Integration & Cleaning (ETL Pipelines)
Tech Used: Pandas, NumPy
Modules: student_cleaner.py, batch_formatter.py
What It Does

Merges 300+ records across 3 institutions

Normalizes:

Course titles

Batch codes

Attendance formats

Fee structures

Data Cleaning Operations

✔ Null handling
✔ Categorical standardization
✔ Duplicate removal
✔ Outlier correction
✔ Feature normalization

Example snippet:

df['attendance_rate'] = df['attended_classes'] / df['total_classes']
df['attendance_rate'] = df['attendance_rate'].fillna(0).clip(0, 1)

📐 2. KPI Engineering (Custom Models)
Model Files: dropout_score.py, bqi.py, efficiency_score.py
KPIs Built
KPI	Formula (Technical)
Student Efficiency Score	Weighted blend of attendance, tests, submissions
Dropout Risk Score	Logistic model using attendance & fee delay
Batch Quality Index (BQI)	Mean(TrainerRating + AvgPerformance + EngagementScore)
Active Learner Score	Activity frequency × Submission reliability

These KPIs feed into Power BI dashboards.

📊 3. Power BI Dashboards (4 Professional Pages)
Dashboard Pages:

Student Performance Dashboard

KPI cards

Performance heatmap

Attendance drill-down

Batch Analysis Dashboard

Batch-wise comparison

Trainer effectiveness

Batch Quality Index

Trainer Rating Dashboard

Rating trends

Student feedback distribution

Revenue & Business Analytics

Monthly revenue

Fee pending stats

Enrolment vs revenue correlation

Power BI uses DAX Measures, for example:

Attendance % = DIVIDE(SUM(Attendance[Present]), SUM(Attendance[Total]))

📲 4. Social Media Analytics Engine
Platforms Included

Instagram

Facebook

YouTube

LinkedIn

Metrics Extracted

Engagement Rate

Reach Growth

Impressions

Follower Velocity

CTR on posts

Python Example:
df['engagement_rate'] = (df['likes'] + df['comments']) / df['followers'] * 100


Outputs feed into a Power BI Social Dashboard.

🤖 5. OpenCV Engagement Analyzer (AI-Based)
Tech: OpenCV, cvzone, Haar Cascades
Functionality

Detects students’ faces in real time

Classifies engagement as:

Focused

Neutral

Distracted

Engagement Score Formula
Engagement = (Focused Frames / Total Frames) × 100

Example Code:
faces = detector.detectMultiScale(gray, 1.3, 5)
engagement_score = focused_frames / total_frames


Results are merged into student analytics.

🧾 6. Excel Automation (MIS System)
Automated Reports Generated:

Fee Pending Report

Attendance MIS

Top Performer List

Monthly Analysis Sheets

Tools Used:

openpyxl

Conditional formatting

Auto-filtering

Dynamic formulas

🎯 Impact (Business + Technical ROI)
✔ Reduced manual reporting load by 70%
✔ Unified academic + revenue + engagement analytics
✔ Improved decision-making using data-driven KPIs
✔ Enabled real-time class engagement tracking
✔ Provided institute-level growth intelligence
🚀 Future Enhancements

Deploy dashboards to Microsoft Power BI Service

Build a Streamlit student performance portal

Add NLP-based student feedback analysis

Integrate smartwatch/biometric data for engagement

Develop a mobile version
