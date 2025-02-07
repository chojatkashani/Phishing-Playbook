# Phishing-Playbook

**Version 1.0**  

---  

## **Table of Contents**  

1. [Purpose](#purpose)  
2. [Using This Playbook](#using-this-playbook)  
3. [Step 1: Receive Phishing Alert](#step-1-receive-phishing-alert)  
4. [Step 2: Evaluate the Alert](#step-2-evaluate-the-alert)  
5. [Step 3.0: Does the Email Contain Any Links or Attachments?](#step-30-does-the-email-contain-any-links-or-attachments)  
6. [Step 3.1: Are the Links or Attachments Malicious?](#step-31-are-the-links-or-attachments-malicious)  
7. [Step 3.2: Update the Alert Ticket and Escalate](#step-32-update-the-alert-ticket-and-escalate)  
8. [Step 4: Close the Alert Ticket](#step-4-close-the-alert-ticket)  
9. [Phishing Flowchart (Version 1.0)](#phishing-flowchart-version-10)  

---  

## **Purpose**  
This playbook helps **level-one SOC analysts** provide an **appropriate and timely response** to phishing incidents.  

---  

## **Using This Playbook**  
Follow the steps below in order. Some steps may overlap depending on the scenario.  

---  

## **Step 1: Receive Phishing Alert**  
The process begins when you receive an **alert ticket** indicating that a phishing attempt has been detected.  

---  

## **Step 2: Evaluate the Alert**  
Upon receiving the alert, investigate its details and relevant log information. The key factors to evaluate include:  

### **1. Alert Severity**  
- **Low:** Does not require escalation.  
- **Medium:** May require escalation.  
- **High:** Requires immediate escalation to the appropriate security personnel.  

### **2. Receiver Details**  
- The receiver’s **email address**  
- The receiver’s **IP address**  

### **3. Sender Details**  
- The sender's **email address**  
- The sender's **IP address**  

### **4. Subject Line**  
- Assess for suspicious keywords or urgency tactics.  

### **5. Message Body**  
- Look for **social engineering attempts** or requests for sensitive information.  

### **6. Attachments or Links**  
🚨 **Do not open links or attachments** unless using an **authorized and isolated environment**.  

---  

## **Step 3.0: Does the Email Contain Any Links or Attachments?**  
Phishing emails often contain **malicious attachments or links** designed to compromise systems.  

- If the email **contains links or attachments**, proceed to **Step 3.1**.  
- If the email **does not contain links or attachments**, proceed to **Step 4**.  

---  

## **Step 3.1: Are the Links or Attachments Malicious?**  
If the email contains attachments or links, determine if they are malicious.  

### **How to Verify:**  
- **Check the link or file reputation** through hash values using threat intelligence tools like **VirusTotal**.  
- If the link or attachment is **not malicious**, proceed to **Step 4**.  

---  

## **Step 3.2: Update the Alert Ticket and Escalate**  
If you confirm the link or attachment is **malicious**, follow these steps:  
1. **Provide a summary** of findings, including reasons for escalation.  
2. **Update the ticket status** to **Escalated**.  
3. **Notify a Level-Two SOC Analyst** for further action.  

---  

## **Step 4: Close the Alert Ticket**  
Update the ticket status to **Closed** if:  
- The email does **not contain any links or attachments**, or  
- The link or attachment was confirmed to be **not malicious**.  

🔹 **Include a brief summary** of investigation findings and the reason for closing the ticket.  

---  

## **Phishing Flowchart (Version 1.0)**  
<img width="679" alt="Screenshot 2025-02-06 at 8 52 45 PM" src="https://github.com/user-attachments/assets/b9a5594a-4528-4340-8bc2-69e481581970" />


This playbook provides a **structured approach** to handling phishing alerts, ensuring analysts follow **best practices** to mitigate security risks.  

