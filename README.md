# Salesforce-Agentforce-Ticket-Intelligence
Autonomous Customer Support Ticket Priority Prediction and Automated Task Assignment System using Salesforce Agentforce and Flow Builder.
# Customer Support Ticket Priority Prediction and Automated Assignment System Using Agentforce

## 📌 Project Overview
This project delivers an autonomous customer support intelligence system built on the Salesforce Platform. By combining a custom object, an Auto-Launched Flow, and a Salesforce Agentforce subagent, the system evaluates incoming customer support ticket descriptions conversationally, classifies ticket urgency (High, Medium, Low), routes critical cases to senior engineers, and automatically generates follow-up tasks without manual intervention.

---

## 🛠️ Components Implemented
* **Custom Object**: `Support_Ticket_Intelligence__c`
* **Backend Automation**: Auto-Launched Flow (`Support Ticket Intelligence - V2`)
* **AI Subagent**: `Support Ticket Priority Analysis`
* **Agent Action**: `Support Ticket Intelligence`

---

## ⚙️ How It Works
1. **User Query**: The user asks Agentforce to analyze tickets for an account (e.g., `"Analyze support ticket for kows"`).
2. **Record Lookup**: The Flow retrieves the customer Account and the most recent ticket record (`TKT-0001`).
3. **Keyword Analysis**: Evaluates description text for urgency keywords (`urgent`, `not working`, `failure`).
4. **Autonomous Actions**:
   * Classifies priority as **High**.
   * Assigns case to **Senior Support Agent**.
   * Creates an automated **Task** record (`Urgent Ticket Handling`) mapped to the Account.
5. **Output**: Agentforce provides structured conversational feedback with ticket status.

---

## 🧪 Validation & Test Results
* **Test Account**: `kows`
* **Ticket Number**: `TKT-0001`
* **Description**: `urgent not working failure`
* **Calculated Priority**: `High`
* **Assigned Agent**: `Senior Support Agent`
* **Status**: `High priority ticket detected`

---

## 🔗 Deliverables & Links
* **Project Report**: [View Documentation PDF](https://github.com/kowsalyarajalingam/Salesforce-Agentforce-Ticket-Intelligence/blob/main/Project_Report.pdf.pdf)
* **Demo Video Link**: [https://drive.google.com/file/d/1Qhq7yIVIcrz9NDb-XwE98OJ99x_7TDoz/view?usp=drive_link]
