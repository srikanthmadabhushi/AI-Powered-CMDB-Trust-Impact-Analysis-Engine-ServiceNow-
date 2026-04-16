# AI-Powered-CMDB-Trust-Impact-Analysis-Engine-ServiceNow-

## 📌 Overview
This project demonstrates an intelligent CMDB enhancement built on ServiceNow that transforms traditional CMDB into a **data quality and impact-aware system**.

It introduces:
- Automated **Trust Scoring**
- **Data Issue Detection**
- Real-time **Impact Analysis**
- UI-driven **Impact Simulation**

---

## 💡 Problem Statement

In most enterprises:
- CMDB stores data but does not validate it
- Missing relationships go unnoticed
- No clear visibility of downstream impact

👉 Result: Poor decision-making and increased operational risk

---

## 🎯 Solution

This project builds an **AI-style CMDB Engine** that:

- Evaluates CI data quality in real-time  
- Detects missing or inconsistent configurations  
- Uses relationship mapping to simulate impact  
- Provides instant insights through UI interaction  

---

## 🔥 Key Features

### ✅ 1. CMDB Trust Score Engine
- Calculates Trust Score (0–100)
- Evaluates:
  - Missing relationships
  - Incomplete data
- Updates fields dynamically:
  - `u_trust_score`
  - `u_data_issue`
  - `u_last_validated`

---

### ⚠️ 2. Data Issue Detection
- Identifies:
  - Missing relationships
  - Data inconsistencies
- Displays issues directly on CI form

---

### 🔗 3. Relationship Mapping
- Uses:
  - `cmdb_rel_ci` table
- Establishes parent-child dependencies

---

### 🔍 4. Impact Simulator (Core Feature)
- Predicts downstream impact of a CI failure
- Uses Script Include logic to traverse relationships

👉 Example:

If ConnectorWare fails → Email is impacted

---

### 🖱️ 5. Real-Time UI Interaction
- Custom UI Action Button: **Check Impact**
- Uses **GlideAjax** for real-time execution
- Displays instant result:
Impacted Systems: Email

---

## 🏗️ Architecture

UI Action (Check Impact Button)
↓
GlideAjax Call
↓
CMDBImpactAjax (Script Include)
↓
CMDBImpactAnalyzer (Core Logic)
↓
cmdb_rel_ci (Relationship Data)

---

## 🛠️ Technologies Used

- ServiceNow CMDB
- GlideRecord
- Script Includes
- GlideAjax
- UI Actions
- JavaScript (Client + Server)

---

## 📸 Screenshots

Added in the Screenshots folder
---

## 🚀 Business Value

This solution enables:

- Improved CMDB data reliability  
- Faster impact analysis during incidents  
- Better decision-making  
- Reduced operational risk  

---

## 🔮 Future Enhancements

- AI-based predictive risk scoring  
- Multi-level dependency traversal  
- CMDB Health Dashboard  
- Integration with AIOps  
- Automated remediation recommendations  

---

## 👨‍💻 Author

**Srikanth Madabhushi**  
🔗 Portfolio: https://SrikanthMadabhushi.github.io  

---

## ⭐ Conclusion

This project demonstrates how CMDB can evolve from a static repository into an **intelligent, decision-support system** using AI-inspired logic and ServiceNow capabilities.
