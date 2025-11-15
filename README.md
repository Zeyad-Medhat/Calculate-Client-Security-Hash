# Calculate Client Security Hash – UiPath REFramework Project

## 📌 Project Overview
**Calculate Client Security Hash** is a UiPath automation project created as part of the UiPath RPA Developer training program.  
The objective is to automate the extraction of client data from the ACME System 1 platform, format it, generate a SHA1 hash, and update the corresponding work item. The solution follows the full **Robotic Enterprise Framework (REFramework)**.

---

## 🧠 Objective
- Log in to **ACME System 1**
- Navigate to **Work Items**
- Filter for **WI5** items with status **Open**
- Extract the Client information (ID, Name, Country)
- Format the data as:  
  `ClientID-ClientName-ClientCountry`
- Generate a **SHA1 hash** based on the formatted data
- Update the Work Item comment with the calculated hash


---

## 🚀 Process Workflow

### **1. Initialization**
- Loads configuration from `Config.xlsx`
- Opens ACME System 1 website
- Logs into user account

### **2. Get Transaction Data**
- Retrieves the next `WI5` item with status `Open`
- Extracts Client data from the Description field

### **3. Process Transaction**
- Formats the client data into:  
  `ClientID-ClientName-ClientCountry`
- Generates SHA1 hash
- Updates the Work Item by adding a comment with the generated hash

### **4. End Process**
- Logs out
- Closes all open applications

---

## 🛠️ Key Features
- Built using **REFramework**
- Full exception handling and retry logic
- Uses secure credential storage (Assets)
- Clean, modular XAML workflows
- Demonstrates:
  - Web automation
  - Regex/string manipulation
  - Data extraction
  - Hashing and updates to ACME system

---

## 🔧 Technologies & Activities Used
- UiPath Studio
- Robotic Enterprise Framework
- SHA1 Hash activity
- Regex and string functions
- Browser automation (Chrome recommended)
- Orchestrator Assets

---

## 🧪 Prerequisites
- UiPath Studio installed
- ACME System 1 account
- Credentials stored in Orchestrator or added in Config.xlsx
- Chrome or Edge with UiPath extension

---

## ➕ How to Run
1. Open the project in UiPath Studio  
2. Enter your ACME credentials (Orchestrator Asset or Config)  
3. Run **Main.xaml**  
4. View updated items in ACME Work Items list  

---

## 🎯 Learning Outcomes
- Understanding of REFramework states  
- Working with Transactions  
- Parsing and formatting data  
- Using SHA1 hashing  
- Web data extraction and system updates  


