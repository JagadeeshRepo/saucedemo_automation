# saucedemo_automation
QA Assessment (Automation Specialist) - Designing and implement a basic web automation framework to test a sample web application using Selenium. This assignment assesses your ability to write clean, maintainable, and scalable automation code for a web-based system.



# SauceDemo Automation Framework

This framework automates [SauceDemo](https://www.saucedemo.com/) using Selenium WebDriver with Java, TestNG, and ExtentReports.

## 🧰 Tech Stack

- Java 11+
- Selenium WebDriver
- TestNG
- WebDriverManager
- ExtentReports
- Maven

## 🚀 How to Run

### Prerequisites

- Java 11+ installed
- Maven installed
- Chrome and/or Firefox installed

### Steps

1. Clone the repository:

```bash
git clone https://github.com/your-username/saucedemo-automation-framework.git
cd saucedemo-automation-framework


saucedemo-automation-framework/
├── pom.xml
├── README.md
├── testng.xml
├── /drivers/             # Optional if using WebDriverManager
├── /screenshots/         # For captured screenshots
├── /reports/             # For extent HTML reports
├── /src
│   ├── /main
│   │   └── /java
│   │       ├── base/
│   │       │   ├── BaseTest.java
│   │       │   └── DriverFactory.java
│   │       ├── utils/
│   │       │   ├── ExtentReportManager.java
│   │       │   ├── ScreenshotUtil.java
│   │       │   └── TestListener.java
│   │       └── swag_Labs/
│   │           └── saucedemo_automation_pages/
│   │               ├── LoginPage.java
│   │               ├── ProductsPage.java
│   │               └── ... other page objects
│   └── /test
│       └── /java
│           └── tests/
│               ├── LoginTest.java
│               ├── CartTests.java
│               └── CheckoutTest.java

Run tests from terminal:

bash
Copy
Edit
mvn clean test
Or use TestNG from your IDE.

View Extent Report:

Open reports/ExtentReport.html after test execution.

🔧 Browser Parameter
You can switch browsers via testng.xml:

xml
Copy
Edit
<parameter name="browser" value="firefox"/>
Supported values: chrome, firefox.


