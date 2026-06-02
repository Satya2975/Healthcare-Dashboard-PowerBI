# 🏥 Healthcare Dashboard | Power BI Project

## 📌 Project Overview

This project is an interactive Healthcare Dashboard developed using Power BI to monitor hospital operations and patient service performance. The dashboard enables management to track appointments, patient waiting times, doctor performance, and no-show rates through a centralized reporting solution.

## 🎯 Project Objective

The main objective of this project was to create an interactive Healthcare Dashboard to monitor hospital operations and patient service performance. The dashboard helps management track appointments, patient waiting time, doctor performance, and no-show rates in one place.

## 🚩 Business Problem

The hospital management team was maintaining reports manually in Excel, which made reporting slow and difficult. They needed a centralized dashboard to monitor:

- Total Patients and Appointments
- Department-wise Waiting Time
- Doctor Performance
- Patient No-Show Trends
- Overall Operational Efficiency

## 🛠️ Tools & Technologies Used

- Power BI
- Power Query
- DAX
- Excel / CSV Files

## 📊 Dataset Information

The dataset contains:

- Patient Details
- Appointment Records
- Doctor Information
- Department Data
- Wait Time Records
- No-Show Status

Data from multiple tables was connected in Power BI using relationships and a structured data model.

## 🧹 Data Cleaning & Transformation

Using Power Query:

- Removed Null Values
- Removed Duplicate Records
- Corrected Data Types
- Standardized Department Names
- Created Calculated Columns
- Prepared Data for Analysis

## 📈 Key Performance Indicators (KPIs)

The dashboard includes:

- Total Departments
- Total Patients
- Total Doctors
- Total Appointments
- Average Wait Time

These KPIs provide a quick overview of hospital workload and performance.

## 📉 Dashboard Visuals

### Average Wait Time by Department
Helps identify departments experiencing longer patient waiting times.

### Average Wait Time by No-Show Risk
Analyzes whether longer waiting times contribute to higher no-show rates.

### Doctor Performance Matrix
Provides doctor-wise analysis including:

- Total Appointments
- Average Consultation Duration
- No-Show Rate
- Available Hours

### No-Show Rate Gauge
Compares actual no-show percentage against target performance.

## 🎛️ Interactive Features

Users can dynamically filter the dashboard using:

- Doctor Slicer
- Department Slicer
- Date Slicer

## 🧮 DAX Measures Used

### Average Wait Time

```DAX
Avg Wait Time =
AVERAGE(Appointments[Wait_Time])
```

### No Show Rate

```DAX
No Show Rate =
DIVIDE(
    COUNTROWS(
        FILTER(
            Appointments,
            Appointments[Status] = "No Show"
        )
    ),
    COUNTROWS(Appointments)
)
```

## 📷 Dashboard Preview

Add your dashboard screenshot here:

![Healthcare Dashboard](Screenshots/dashboard.png)

## 💼 Business Impact

This dashboard helps hospital management:

- Reduce patient waiting time
- Improve doctor scheduling
- Track no-show trends
- Improve operational efficiency
- Make faster data-driven decisions

## 📚 Key Learnings

Through this project, I enhanced my skills in:

- Power BI Dashboard Development
- Power Query Data Transformation
- DAX Calculations
- KPI Design
- Healthcare Data Analytics
- Interactive Report Development

## 🔮 Future Enhancements

- Predictive No-Show Analysis
- Patient Satisfaction Tracking
- Real-Time Data Refresh
- Advanced Healthcare KPIs

## 👨‍💻 Author

**Satyajit Chavan**

Power BI Developer | Data Analyst

📧 Email: satyajitchavan22@gmail.com

🔗 LinkedIn: https://www.linkedin.com/in/satyajitchavan/

🔗 GitHub: https://github.com/Satya2975
