# Kyla Product Analyst Test Task

We are glad to continue the recruitment process for the Product Analyst position with you. Before we meet for the second interview, we have a task for you as your first assignment. This will help us evaluate your practical skills. Please note that we will discuss your solution only as part of this recruitment process.

## Task 1: New App Feature Analysis

### Description:
You are tasked with evaluating the effectiveness of a new appointment reminder feature in a healthcare app. This involves analyzing patient data, conducting A/B testing, validating hypotheses, building funnels, and examining traffic sources. Your findings will help determine how the new feature impacts appointment confirmations and overall patient engagement.

### Data Files Provided:
1. **appointments_data.csv**:
   - Fields:
     - `patient_id`: Unique identifier for each patient.
     - `age`: Age of the patient.
     - `gender`: Gender of the patient.
     - `doctor_name`: Name of the doctor the appointment is with.
     - `appointment_reason`: Reason for the appointment (e.g., Annual Exam, Screening for COVID, Asthma, Allergy Injection, etc.).
     - `appointment_date`: Date of the scheduled appointment.
     - `appointment_status`: Whether the appointment was attended or not.

2. **ab_test_data.csv**:
   - Fields:
     - `patient_id`: Unique identifier for each patient.
     - `group`: A/B testing group (Control or Test).
       - **Control Group**:
         - Purpose: Serves as the baseline for comparison. Patients in this group do not receive a reminder about their appointment. Their attendance is tracked without any intervention to understand the natural behavior of patients without the reminder.
       - **Test Group**:
         - Purpose: This group receives a reminder about their appointment. The data collected includes whether they viewed the reminder, confirmed their appointment, and eventually attended it. This allows for analysis of the reminder’s impact on attendance.
     - `event_name`: Name of the event related to the appointment process (e.g., reminder_sent, reminder_viewed, appointment_confirmed, attended_appointment).
     - `event_datetime`: Timestamp of when the event occurred.

3. **app_data.csv**:
   - Fields:
     - `patient_id`: Unique identifier for each patient.
     - `traffic_source`: The source through which the patients downloaded the app (e.g., Organic Search, Meta Ads, Google Ads, Referral, Direct).
     - `device`: The type of device used by the patient (e.g., IOS 18.1, Android 9.3).

### Tasks:

1. **Data Exploration and Cleaning**:
   - Load the datasets and explore the data to understand its structure. Identify any inconsistencies or missing values and perform necessary data cleaning.

2. **A/B Testing Analysis**:
   - Conduct an A/B test analysis to determine whether the app reminder feature in the Test group leads to a higher rate of appointment confirmations compared to the Control group.
   - Use appropriate statistical methods (e.g., t-tests, chi-square tests) to validate your findings.

3. **Hypothesis Testing**:
   - Formulate and test hypotheses related to the effectiveness of the app reminders. For example:
     - Hypothesis 1: "Patients in the Test group are more likely to confirm their appointments within 1 hour of viewing the reminder compared to the Control group."
     - Hypothesis 2: "Young patients using newer device versions are more likely to view and respond to reminders promptly."

4. **Funnel Analysis**:
   - Build a funnel to analyze the patient journey from receiving a reminder to attending the appointment. Identify any significant drop-offs or conversion points and provide insights on how to improve appointment attendance.

5. **Traffic Source Analysis**:
   - Determine which traffic sources are most effective in bringing patients who engage with the app reminders.
   - Provide a breakdown of the performance of different paid ad platforms (e.g., Meta Ads, Google Ads, Apple Ads) compared to organic and referral sources.

6. **SQL Queries**:
   - Use DuckDB to assume the provided CSV files are stored in a relational database. Write SQL queries to:
     - Retrieve patients who confirmed their appointment within 5 minutes of viewing the reminder.
     - Identify the most common traffic sources for patients who attended their appointments.
     - Calculate the average time between reminder viewing and appointment confirmation for different age groups.

### Expected Output:
- A report summarizing your findings, including:
  - A/B test results and hypothesis testing outcomes.
  - Funnel analysis with visualizations.
  - Insights from the traffic source analysis.
  - SQL queries.
  - Recommendations based on your analysis.
- Answer the following questions:
  1. What inconsistencies in data did you find?
  2. What additional patients' data would be helpful for a deeper analysis?
- Python code or Jupyter Notebook used for the analysis.

---

## Task 2: R&D Product Analysis

### Description:
Conduct research on how the business of selling Kyla’s lab tests ([https://kyla.com/labs?product_analyst_test_task](https://kyla.com/labs?product_analyst_test_task)) and other At-Home Lab Test solutions is organized. Compile an **OKR Tree** with an argument for its application to this type of business.

### Expected Output:
- The solution should consist of two parts:
  1. **Tree of Product Metrics**.
  2. **Analysis and argumentation** of the built solution.
  
  *Note: You can use any preferred tool for graphical representation of the OKR Tree (e.g., Figma).*
