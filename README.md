# 🧑‍💼 Automated HR Leave Management System (n8n + Power BI)

## 📌 Overview
This project automates the **HR Leave Management Process** using **n8n**, **Google Sheets**, **Gmail**, and **Power BI**.

It reduces manual work by automatically:
- Processing leave requests
- Approving/rejecting based on rules
- Sending email notifications
- Updating records in real-time
- Visualizing data through dashboards

---

## ⚙️ Workflow Architecture

### 🔄 Process Flow
1. Google Sheets Trigger → Detects new leave entry  
2. IF Condition → Checks leave days  
3. Decision:
   - ✅ ≤ 2 days → Approved  
   - ❌ > 2 days → Not Approved  
4. Gmail → Sends email notification  
5. Google Sheets → Stores final status  

---

## 🧠 Workflow Logic

IF Leave Days ≤ 2  
→ Send "Approved" Email  
→ Append Row (Status: Approved)  

ELSE  
→ Send "Not Approved" Email  
→ Append Row (Status: Not Approved)  

---

## 🛠️ Technologies Used
- **n8n** – Workflow Automation  
- **Google Sheets** – Data Storage & Trigger  
- **Gmail API** – Email Notifications  
- **Power BI** – Dashboard Visualization  

---

## 📂 Project Structure

