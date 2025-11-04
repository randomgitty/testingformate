<p align="center">
  <img src="https://via.placeholder.com/1000x250?text=Store+Connect+Automation+Suite" alt="Store Connect Automation Banner" width="100%">
</p>

<h1 align="center">Store Connect Automation Suite</h1>
<p align="center">
  <b>End-to-End Automation for the Store Connect Application</b><br>
  Built with <b>Python, Pytest, Selenium,</b> and <b>Appium</b> to ensure scalability, stability, and performance.
</p>

<p align="center">
  <a href="https://www.python.org/"><img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python"></a>
  <a href="https://docs.pytest.org/"><img src="https://img.shields.io/badge/Pytest-0A9EDC?style=for-the-badge&logo=pytest&logoColor=white" alt="pytest"></a>
  <a href="https://www.selenium.dev/"><img src="https://img.shields.io/badge/Selenium-43B02A?style=for-the-badge&logo=selenium&logoColor=white" alt="Selenium"></a>
  <a href="https://appium.io/"><img src="https://img.shields.io/badge/Appium-9932CC?style=for-the-badge&logo=appium&logoColor=white" alt="Appium"></a>
</p>

---

## 🧩 Overview

The **Store Connect Automation Suite** streamlines Automation testing for the Store Connect application, supporting **mobile (Android)** interface.  
It is engineered for **modular, data-driven, and reusable** test design, enabling rapid regression testing and continuous integration.
---

## 🧪 Test Coverage Highlights

- ✅ **Login and Session Management**  
- 🔍 **Product Search** (valid/invalid barcode validation)  
- 🏬 **Multi-Branch Product Availability Verification**  
- ⚙️ **Service & Repair Module Navigation**  
- 📦 **Comprehensive Module Coverage**  
- 🔝 **Top 500 Items Validation**

---

## 🧠 Key Features
- 🧱 Modular, reusable page object architecture  
- 🧾 HTML and Allure test reports  
- 🧰 Config-driven environment management  

---

## 🛠️ Environment Setup

### 🔧 Prerequisites

## 🛠️ Tools & Dependencies

| Component            | Role                   | Version       |
|----------------------|------------------------|---------------|
| **Python**           | Core Language          | 3.11+          |
| **Selenium WebDriver** | Browser Automation   | 4.24.0           |
| **Pytest**           | Test Framework         | Latest        |
| **Allure**           | HTML Test Reporting    | Latest        |
| **Appium Server**     | Automation Frameworf for Mobile Testing         | Latest        |
| **Logger**           |  Debugging CLI         | Latest        |
| **ADB (Android Debug Bridge)**           |  Device communication interface         | Latest        |
| **Environment Variables**           |  System-level configuration paths         |<ul><li>`ANDROID_HOME`</li><li>`JAVA_HOME`</li><li>`SDK_ROOT`</li><li>All added to system `PATH`</li></ul> |

---

### 🚀 Setup & Execution

#### 1. Clone the repository
```bash
git clone https://github.com/your-org/store-connect-automation.git
cd store-connect-automation 
```

### 2. Create and Activate Virtual Environment 
It is best practice to isolate project dependencies 
```bash 
# Create Environment 
python -m venv venv 

# Activate environment (Windows) [Gitbash]: 
source venv/Scripts/activate 

# Activate environment (MacOS / Linux): 
source venv/bin/activate 
``` 
### 3. Install Dependencies 
All required Python libraries are listed in `requirements.txt`.
```bash 
pip install -r requirements.txt 
```
## ▶️ Execution 
### Run the Test 
Execute the main checkout flow using Pytest, generating Allure report, HTML report and Logs files in the process : 

```bash 
# Change Directory if you are not in STORECONNECTAPP
cd STORECONNECTAPP

# Run Tests 
pytest test_cases/test_case_name.py
```
## 📊 Test Reporting 
After execution, serve the generated report files to view the interactive dashboard. 
```bash 
# Serve Allure Report locally in your browser 
allure serve reports/allure-results
```

## 📂 Project Structure 
```plaintext
store-connect-automation/
├── pages/                     # Page Object Model classes
│   ├── login_page.py
├── tests/                     # Test modules
├── utilities/                     # Helpers (screenshot, env loader, driver_factory, config)
├── pytest.ini               # Pytest initialization (Auto generate logs and reports)
├── requirements.txt
└── README.md
```

