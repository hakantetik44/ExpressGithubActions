# 🛍️ AliExpress E2E Test Automation Framework

![Java](https://img.shields.io/badge/Java-21-orange.svg)
![Selenium](https://img.shields.io/badge/Selenium-4.16.1-green.svg)
![TestNG](https://img.shields.io/badge/TestNG-7.8.0-blue.svg)
![Allure](https://img.shields.io/badge/Allure-2.24.0-yellow.svg)

![AliExpress Banner](https://via.placeholder.com/800x200.png?text=AliExpress+E2E+Test+Automation)

## 📋 Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Running Tests](#running-tests)
- [Test Reports](#test-reports)
- [Page Objects](#page-objects)
- [Contributing](#contributing)

## 🔍 Overview
This project is a robust end-to-end test automation framework for AliExpress.com, built using Java and following the Page Object Model design pattern. It includes automated test scenarios for product search functionality with detailed reporting capabilities. The framework aims to streamline the testing process, ensuring high-quality software delivery.

## ✨ Features
- **Page Object Model**: Maintainable and reusable code structure, allowing easy updates and scalability.
- **Allure Reporting**: Detailed test execution reports with screenshots, providing insights into test results and failures.
- **Parallel Execution**: Support for running tests in parallel, reducing overall test execution time.
- **Cross-browser Testing**: Support for multiple browsers, ensuring compatibility across different environments.
- **Logging**: Comprehensive logging with Log4j and SLF4J, aiding in debugging and monitoring.
- **Cookie Handling**: Automated cookie consent management, ensuring compliance with privacy regulations.
- **Error Handling**: Robust error handling and recovery mechanisms, minimizing test failures due to unexpected issues.

## 🛠️ Tech Stack
- **Java 21**: Programming language
- **Selenium WebDriver**: Web automation
- **TestNG**: Test execution framework
- **Allure**: Test reporting
- **Maven**: Build and dependency management
- **Log4j & SLF4J**: Logging framework
- **WebDriverManager**: Browser driver management

## 📁 Project Structure
```
aliexpress-e2e/
├── src/
│   ├── main/
│   │   └── java/
│   │       └── com/
│   │           └── aliexpress/
│   │               ├── pages/
│   │               │   ├── BasePage.java
│   │               │   ├── HomePage.java
│   │               │   └── SearchResultsPage.java
│   │               └── utils/
│   │                   └── Constants.java
│   └── test/
│       ├── java/
│       │   └── com/
│       │       └── aliexpress/
│       │           └── tests/
│       │               └── SearchTest.java
│       └── resources/
│           ├── log4j2.xml
│           └── testng.xml
└── pom.xml
```

## 🛠️ Prerequisites
- Java 21 or later
- Maven 3.6+
- A web browser (Chrome, Firefox, etc.)

## 🚀 Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/aliexpress-e2e.git
   ```
2. Navigate to the project directory:
   ```bash
   cd aliexpress-e2e
   ```
3. Install dependencies:
   ```bash
   mvn clean install
   ```

## 🏃 Running Tests
To execute tests, run the following command:
```bash
mvn test
```

## 📊 Test Reports
After running tests, generate the Allure report:
```bash
mvn allure:serve
```

## 🧩 Page Objects
The framework uses the Page Object Model to organize code. Each page of the application is represented by a class.

## 🤝 Contributing
Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/YourFeature`)
5. Open a pull request.

## 📝 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👥 Authors
- Your Name - *Initial work* - [YourGitHub](https://github.com/yourusername)

## 🙏 Acknowledgments
- Selenium WebDriver team
- TestNG team
- Allure Framework team
