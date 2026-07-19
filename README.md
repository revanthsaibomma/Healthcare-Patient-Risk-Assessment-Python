# Healthcare Patient Risk Assessment System

A simple Python application that assesses a patient's health risk based on vital signs using **if-elif-else** statements. This project demonstrates how real-world healthcare business rules can be implemented in Python while practicing Git and GitHub workflows.

---

## Project Objective

The objective of this project is to automate the initial patient screening process in a hospital. Based on the patient's age and vital signs, the application classifies the patient into different health risk categories and provides the appropriate medical recommendation.

---

## Features

- Accepts patient information
- Determines patient risk level
- Displays appropriate recommendation
- Identifies senior citizens (75 years and above)
- Displays priority consultation message for senior citizens
- Beginner-friendly Python code
- Uses only `if`, `elif`, and `else`

---

## Technologies Used

- Python 3.x
- Git
- GitHub

---

## Project Structure

```
Healthcare-Patient-Risk-Assessment/
│
├── healthcare_patient_risk_assessment.py
├── README.md
├── .gitignore
└── venv/
```

---

## Input

The application accepts the following inputs:

- Patient Name
- Patient Age
- Body Temperature (°C)
- Heart Rate (BPM)
- Oxygen Saturation (SpO₂)

---

## Business Rules

### Critical Condition

- Oxygen Level < 90
- OR Temperature > 40°C

**Recommendation:**
Immediately transfer the patient to ICU.

---

### High Risk

- Oxygen Level between 90 and 94
- OR Temperature between 38°C and 40°C

**Recommendation:**
Doctor consultation and hospital admission required.

---

### Medium Risk

- Heart Rate > 100 BPM
- OR Age > 60 years

**Recommendation:**
Keep the patient under observation.

---

### Low Risk

If none of the above conditions are satisfied.

**Recommendation:**
Patient is healthy and can go home after consultation.

---

### Senior Citizen Priority

If Age ≥ 75 years

Display:

- Senior Citizen
- Priority Consultation Required

---

## How to Run

### Clone the Repository

```bash
git clone https://github.com/your-username/Healthcare-Patient-Risk-Assessment.git
```

### Navigate to the Project Folder

```bash
cd Healthcare-Patient-Risk-Assessment
```

### Create Virtual Environment

```bash
python -m venv venv
```

### Activate Virtual Environment

#### Windows

```bash
venv\Scripts\activate
```

#### Linux / macOS

```bash
source venv/bin/activate
```

### Run the Application

```bash
python healthcare_patient_risk_assessment.py
```

---

## Sample Output

```
========================================
 Healthcare Patient Risk Assessment System
========================================

Enter Patient Name: Rahul
Enter Patient Age: 68
Enter Body Temperature (°C): 39
Enter Heart Rate (BPM): 95
Enter Oxygen Saturation (SpO₂): 92

========================================
        Patient Assessment Report
========================================
Patient Name   : Rahul
Age            : 68
Temperature    : 39.0 °C
Heart Rate     : 95 BPM
Oxygen Level   : 92 %
Risk Level     : High
Recommendation : Doctor consultation and hospital admission required.
========================================
```

---

## Learning Outcomes

This project helps learners understand:

- Python Variables
- User Input
- Conditional Statements (`if`, `elif`, `else`)
- Boolean Operators (`and`, `or`)
- Real-world Business Logic
- Git Version Control
- GitHub Repository Management

---

## Git Commands Used

Initialize Git

```bash
git init
```

Add Files

```bash
git add .
```

Commit

```bash
git commit -m "Initial implementation of Healthcare Patient Risk Assessment System"
```

Push to GitHub

```bash
git branch -M main
git remote add origin https://github.com/your-username/Healthcare-Patient-Risk-Assessment.git
git push -u origin main
```

Update Project

```bash
git add .
git commit -m "Added Senior Citizen Priority feature"
git push
```

---

## Future Enhancements

- Input validation
- BMI calculation
- Blood pressure analysis
- Diabetes risk assessment
- Report generation
- GUI using Tkinter or Streamlit
- Database integration

---

## Author

**Revanth Sai Bomma**

GitHub: https://github.com/revanthsaibomma

---

## License

This project is created for educational and learning purposes.