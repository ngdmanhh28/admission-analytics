# 📊 Smart Admission Analytics System

> An intelligent admission data analytics dashboard system for University

The project provides a comprehensive Fullstack solution to digitize, analyze, and visualize important admission indicators. The system helps administrators make decisions based on real data about score distribution, admission sources, and student competency.

---

## Interface & Features

Below are the main modules of the system built from real-world data:

### 1. Dashboard Preview

Displays core KPI indicators and quick admission trends.
![Dashboard Overview]
_ **KPI Cards: Total Applicants (3000), Average Admission Score (20.31), Enrollment Rate (100%), Outstanding Students (4.0%).
_ **Bar Chart: Top 3 majors with the highest admission scores (International Business, Accounting).
_ **Pie Chart: Gender distribution of applicants (51% Male - 49% Female).

### 2. Detailed Statistics Charts (Statistics)

Focuses on in-depth analysis of scores and major quotas.
![Statistics Charts 1]
_ **Score Distribution (Histogram): Visualizes the distribution of admission scores by ranges, automatically drawing the average (Mean) line as a dark orange dashed line using a Custom Canvas Plugin.
_ **Quota vs Actual Enrollment: Double bar chart comparing planned admission quotas and actual enrolled students by major.
![Statistics Charts 2]
_ **Admission Source Map: Horizontal bar chart displaying the Top 10 provinces/cities with the highest number of enrolled students (Bac Giang, Lai Chau...).
_ **Competency Radar Chart: Compares average admission scores among THPT, HSA (Hanoi National University Competency Assessment), and TSA (Hanoi University of Science and Technology Competency Assessment) methods.

### 3. Smart Insights Reports (Insights)

Uses basic algorithms to provide insights and early warnings.

![Smart Insights]
_ **Smart Indicators: IELTS student ratio (0% - Low level of international integration), HSA/TSA admitted student ratio (30.67%).
_ **Performance Analysis: Automatically identifies the leading majors in terms of scores and enrollment rates.
_ **Early Warning: Detects majors with declining enrollment rate trends to propose improvement solutions.

### 4. Student List Management

Detailed management interface for each applicant.
![Student List]
_ **Data Table: Displays Student ID, Full Name, Admitted Major, Exam Score (30-point scale).
_ **Search: Supports real-time search by student name.

---

## 🛠 Technology Architecture

### Backend (Data Server)

- **FastAPI: High-performance Python framework.
- **MySQL / SQLAlchemy: Database management system and ORM for managing admission data.

### Frontend (Interface & Charts)

- **React.js: Library for building user interfaces.
- **Tailwind CSS: Modern UI design framework.
- **Chart.js (react-chartjs-2): Used for Histogram and Radar charts (with custom plugins).
- **Recharts: Used for Bar, Pie, and Horizontal Bar charts.
- **Lucide Icons: Consistent icon system.

---

## 📦Installation Guide

### 1. Backend Configuration

cd backend\FastAPI

python -m venv venv

pip install -r requirements.txt

# Configure the SQL Server connection in the main.py or .env file

python -m uvicorn app.main:app --reload

### 2. Frontend Configuration

cd frontend

npm install

npm start
