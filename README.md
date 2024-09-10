# Kyla Product Analyst Test Task

This README outlines the two tasks assigned for the Product Analyst position at Kyla, detailing the requirements for analyzing the effectiveness of a new app feature and conducting product research for Kyla's lab tests.

## Task 1: New App Feature Analysis

You are tasked with evaluating the effectiveness of a new appointment reminder feature in a healthcare app. The analysis includes A/B testing, hypothesis validation, funnel building, and traffic source analysis.

### Data Provided
1. **appointments_data.csv**:
   - Fields: `patient_id`, `age`, `gender`, `doctor_name`, `appointment_reason`, `appointment_date`, `appointment_status`.

2. **ab_test_data.csv**:
   - Fields: `patient_id`, `group` (Control or Test), `event_name` (e.g., reminder_sent, reminder_viewed, appointment_confirmed, attended_appointment), `event_datetime`.

3. **app_data.csv**:
   - Fields: `patient_id`, `traffic_source` (e.g., Organic, Meta Ads, Google Ads), `device` (e.g., IOS, Android).

### Task Breakdown

1. **Data Exploration & Cleaning**:
   - Load and explore the datasets.
   - Clean the data if there are inconsistencies or missing values.

2. **A/B Testing Analysis**:
   - Compare the appointment confirmation rates between the Test and Control groups.
   - Use statistical methods (e.g., t-tests, chi-square tests).

3. **Hypothesis Testing**:
   - Formulate and test hypotheses related to the reminder feature. Example:
     - "Patients in the Test group confirm appointments more often than the Control group."

4. **Funnel Analysis**:
   - Build a funnel to analyze the patient journey from receiving a reminder to attending an appointment.
   - Identify drop-off points and make recommendations.

5. **Traffic Source Analysis**:
   - Identify the most effective traffic sources for patients engaging with reminders.
   - Analyze paid ad platforms versus organic sources.

6. **SQL Queries**:
   - Use DuckDB for querying:
     - Retrieve patients who confirmed their appointment within 5 minutes of viewing the reminder.
     - Find the most common traffic sources for patients who attended appointments.
     - Calculate average time between reminder viewing and appointment confirmation across age groups.

### Expected Output:
- A report with:
  - A/B test and hypothesis testing results.
  - Funnel analysis and visualizations.
  - Insights from traffic source analysis.
  - SQL queries.
  - Recommendations based on your analysis.
  - Answers to:
    1. What inconsistencies did you find in the data?
    2. What additional data would help in deeper analysis?
- Python code or Jupyter Notebook for the analysis.

---

## Task 2: R&D Product Analysis

Research the business model for selling Kyla’s lab tests and other At-Home Lab Test solutions. Build an **OKR Tree** and provide a rationale for its application to this business type.

### Expected Output:
- A graphical **OKR Tree**.
- Analysis and argumentation of the solution.
  
---

For more information on the lab tests: [Kyla At-Home Lab Tests](https://kyla.com/labs?product_analyst_test_task)