# rest-assured-api-testing
# RestAssured API Testing Framework

## Project Overview

This project demonstrates API automation testing using **Java, REST Assured, Cucumber BDD, and JUnit**.

The framework is designed to validate a Quote Management API that allows sales representatives to create quotes for customers by providing product details, quantities, unit prices, and discounts.

It follows the Behavior-Driven Development (BDD) approach using Cucumber feature files, making test scenarios easy to understand and maintain.

## Technologies Used

- **Programming Language:** Java
- **API Testing Library:** REST Assured 5.5.0
- **BDD Framework:** Cucumber 7.18.0
- **Test Runner:** JUnit
- **Build Tool:** Maven
- **Test Reporting:** Cucumber HTML Reports
- **JSON Processing:** Gson
- **IDE:** IntelliJ IDEA

## Project Structure

```text
RestAssured-API-Testing/
│
├── src/
│   └── test/
│       ├── java/
│       │   ├── core/
│       │   ├── hooks/
│       │   ├── steps/
│       │   └── RunCucumberTest.java
│       │
│       └── resources/
│           ├── documents/
│           └── features/
│               └── create_quote.feature
│
├── pom.xml
├── README.md
└── .gitignore
```

## Features Tested

The framework covers the following Quote Management API functionalities:

- Creating a new quote for a customer.
- Adding single and multiple products to a quote.
- Validating customer and product details.
- Verifying product quantities and unit prices.
- Testing discount percentage calculations.
- Validating individual line item totals.
- Checking the overall quote price.
- Verifying API response status codes and confirmation messages.

## Framework Architecture

The project follows a BDD-based automation framework:

1. **Feature Files:** Define test scenarios using Gherkin syntax (Given, When, Then).
2. **Step Definitions:** Connect Gherkin steps to Java automation code.
3. **Hooks:** Handle test setup and teardown activities.
4. **Core:** Contains reusable framework components.
5. **REST Assured:** Sends HTTP requests and validates API responses.
6. **JUnit:** Executes the Cucumber test scenarios.

## Prerequisites

Before running the project, install:

- Java JDK 15 or compatible configured JDK.
- IntelliJ IDEA.
- Apache Maven.
- Git.

## Installation and Setup

**1. Clone the repository**

```bash
git clone https://github.com/YOUR-USERNAME/RestAssured-API-Testing.git
```

**2. Navigate to the project directory**

```bash
cd RestAssured-API-Testing
```

**3. Install dependencies**

```bash
mvn clean install
```

**4. Execute the test cases**

```bash
mvn test
```

Alternatively, run `RunCucumberTest.java` directly from IntelliJ IDEA.

## Test Execution Report

The framework generates an HTML report after test execution.

Report location:

```text
target/cucumber-reports.html
```

The report provides details about executed scenarios, passed tests, failed tests, and execution results.

## Learning Outcomes

- Understanding REST API automation testing.
- Working with REST Assured for HTTP requests and response validation.
- Implementing BDD using Cucumber and Gherkin.
- Integrating Cucumber with JUnit.
- Managing dependencies using Maven.
- Understanding API testing framework architecture.
- Generating and analyzing automated test reports.

## Author

**Your Name**

GitHub: https://github.com/YOUR-USERNAME

---

*This project is intended for learning and demonstrating API automation testing concepts using Java and BDD.*
