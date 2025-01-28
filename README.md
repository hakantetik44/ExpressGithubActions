# 🛍️ AliExpress E2E Test Automation Framework

![Java](https://img.shields.io/badge/Java-21-orange.svg)
![Selenium](https://img.shields.io/badge/Selenium-4.16.1-green.svg)
![TestNG](https://img.shields.io/badge/TestNG-7.8.0-blue.svg)
![Allure](https://img.shields.io/badge/Allure-2.24.0-yellow.svg)

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
This project is a robust end-to-end test automation framework for AliExpress.com, built using Java and following the Page Object Model design pattern. It includes automated test scenarios for product search functionality with detailed reporting capabilities.

## ✨ Features
- **Page Object Model**: Maintainable and reusable code structure
- **Allure Reporting**: Detailed test execution reports with screenshots
- **Parallel Execution**: Support for running tests in parallel
- **Cross-browser Testing**: Support for multiple browsers
- **Logging**: Comprehensive logging with Log4j and SLF4J
- **Cookie Handling**: Automated cookie consent management
- **Error Handling**: Robust error handling and recovery mechanisms

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

## 📋 Prerequisites
- Java Development Kit (JDK) 21
- Maven 3.8.x or higher
- Chrome/Firefox browser
- Allure command-line tools (for reports)

## 🚀 Installation
1. Clone the repository:
```bash
git clone https://github.com/yourusername/aliexpress-e2e.git
```

2. Install dependencies:
```bash
mvn clean install
```

3. Install Allure (macOS):
```bash
brew install allure
```

## 🏃‍♂️ Running Tests
### Run all tests:
```bash
mvn clean test
```

### Run specific test class:
```bash
mvn test -Dtest=SearchTest
```

### Generate and view Allure report:
```bash
mvn allure:serve
```

## 📊 Test Reports
Allure reports provide detailed test execution information including:
- Test execution summary
- Step-by-step test execution details
- Screenshots on failures
- Test execution time
- Environment details

## 📑 Page Objects
### HomePage
- Navigation to AliExpress homepage
- Cookie consent handling
- Product search functionality

### SearchResultsPage
- Product listing verification
- Product selection
- Search result filtering

## 🤝 Contributing
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👥 Authors
- Your Name - *Initial work* - [YourGitHub](https://github.com/yourusername)

## 🙏 Acknowledgments
- Selenium WebDriver team
- TestNG team
- Allure Framework team
