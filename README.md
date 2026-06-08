AI-Powered Loan Approval Automation using n8n
📌 Project Overview

This project demonstrates how a traditional loan approval process can be automated using the n8n low-code automation platform. The workflow evaluates loan applications based on credit score, debt-to-income ratio (DTI), and AML/PEP watchlist screening, then automatically routes applications for approval, rejection, or manual review.

The solution was developed as part of an MBA Applied Finance project to showcase the practical application of AI-driven financial process automation in banking and fintech.

🎯 Problem Statement

Traditional loan approval processes suffer from:

Long approval cycles (3–5 days)
High operational costs
Manual errors in risk assessment
Compliance and AML screening gaps
Limited scalability

This project automates the process to improve efficiency, accuracy, and compliance.

🚀 Key Features
Automated Loan Evaluation
Credit Score Validation
Debt-to-Income (DTI) Analysis
AML/PEP Watchlist Screening
Automated Decision Routing
Decision Outcomes
✅ Auto Approve
❌ Auto Reject
🔍 Manual Review
🛡️ AML/Compliance Escalation
Automated Notifications
Approval Emails
Rejection Emails
Compliance Team Alerts
AML Risk Notifications
🏗️ Workflow Architecture
Trigger
   │
   ▼
Read Loan Applications
(Google Sheets)
   │
   ▼
Credit Score & DTI Check
   │
 ┌─┴───────────────┐
 │                 │
 ▼                 ▼
Approve Path    Reject/Review Path
 │                 │
 ▼                 ▼
Watchlist Check   AML Screening
 │                 │
 ▼                 ▼
Email Alerts    Compliance Alerts
📊 Dataset Information

The project uses a custom-built dataset containing 40 loan applications with the following fields:

Column	Description
Application_ID	Unique Application Identifier
Applicant_Name	Applicant Name
Annual_Income_USD	Annual Income
Loan_Amount_Requested	Requested Loan Amount
Credit_Score	Credit Rating
Debt_To_Income_Ratio	Financial Risk Indicator
Watchlist_Match_Pct	AML/PEP Screening Score
System_Initial_Action	Automated Decision
Max_Allowable_EMI	Maximum EMI Allowed
Decision_Primary_Basis	Decision Reason
⚙️ Decision Rules
Auto Approve
Credit Score ≥ 600
AND
DTI ≤ 0.50
AND
Watchlist Score < 0.30
Auto Reject
Credit Score < 560
OR
DTI > 0.55
Manual Review
Watchlist Score ≥ 0.30
AND
Watchlist Score < 0.80
AML Escalation
Watchlist Score ≥ 0.80
OR
PEP Match Found
📈 Results
Metric	Manual Process	Automated Process
Processing Time	3–5 Days	< 2 Minutes
Human Effort	100% Manual	73% Automated
Error Rate	35%	< 3%
Cost per Application	$2,400	$180
Daily Capacity	20–30 Applications	500+ Applications
Compliance Coverage	60%	100%
Achievements
🚀 99.9% Faster Processing
💰 92% Cost Reduction
📈 17x Throughput Increase
🎯 91% Error Reduction
🔒 Full AML/PEP Compliance Coverage
🛠️ Technology Stack
n8n
Google Sheets
Gmail API
Workflow Automation
Financial Risk Rules Engine
AML/PEP Screening Logic
📂 Project Structure
Loan-Approval-Automation/
│
├── Dataset/
│   └── Loan_Approval_Dataset.xlsx
│
├── Workflow/
│   └── n8n_workflow.json
│
├── Screenshots/
│   └── Workflow_Architecture.png
│
├── Presentation/
│   └── Loan_Approval_Automation.pptx
│
└── README.md
🔮 Future Enhancements
Phase 1
Automated Audit Trail Logging
Regulatory Reporting
Phase 2
Machine Learning Credit Scoring
WhatsApp Notification Integration
Multi-Currency Loan Processing
Phase 3
Predictive Risk Engine
AI-Powered Fraud Detection
CRM Integration (Salesforce / HubSpot)
