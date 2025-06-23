### **1. Prerequisites to Master First: Your Solid Foundation**

Before we deep dive, ensure you have a strong command over these fundamentals. They are the building blocks upon which your software testing and automation expertise will rest.

* **Java Basics:**
    * **OOP:** Classes, Objects, Inheritance, Polymorphism, Abstraction, Encapsulation.
    * **Collections:** `List`, `Set`, `Map` and their implementations (`ArrayList`, `HashSet`, `HashMap`).
    * **Exceptions:** `try-catch-finally`, `throws`, custom exceptions.
    * **I/O:** File handling, reading from/writing to files.
    * **Multithreading:** Basic concepts of threads, `Runnable`, `Callable`, `ExecutorService`.
* **Web Technologies:**
    * **HTML, CSS, JavaScript:** Understanding DOM structure, element properties, basic styling, and frontend interactions for effective UI testability.
* **Database:**
    * **SQL:** DDL (CREATE, ALTER), DML (SELECT, INSERT, UPDATE, DELETE), Joins, basic aggregation functions.
    * **JDBC:** Connecting Java applications to databases, executing queries.
* **Spring Boot Basics:**
    * **Controllers, Services, Repositories:** Understanding the layered architecture.
    * **Dependency Injection:** `@Autowired`.
    * **REST APIs:** Understanding `GET`, `POST`, `PUT`, `DELETE` methods, common HTTP status codes (2xx, 4xx, 5xx).
* **Build Systems:**
    * **Maven/Gradle:** Basic commands (`clean`, `install`, `test`), understanding `pom.xml`/`build.gradle` for dependency management.
* **Version Control:**
    * **Git and GitHub basics:** `clone`, `add`, `commit`, `push`, `pull`, `branch`, `merge`.
* **DevOps Concepts (Basic Awareness):**
    * **CI/CD:** Continuous Integration, Continuous Delivery.
    * **Docker:** Containers, images (conceptual understanding for test environments).
    * **Jenkins:** Basic understanding of build automation servers.

---

## **2. Software Testing and Automation: Structured Modules**

This curriculum is meticulously designed into five modules, aligning with Anna University's Regulation 2021 for **Software Testing and Automation (CCS366)**. Each module blends theory, practical implementation, Java full-stack examples, tool usage, and interview preparation.

---

### **Module 1: Foundations of Software Testing & Manual Testing**

This module lays the groundwork by introducing core concepts of software testing, its lifecycle, and the fundamental approaches to manual testing.

**📘 Theory:**
* **Software Development Life Cycle (SDLC):** Phases (Requirements, Design, Development, Testing, Deployment, Maintenance).
* **Software Testing Life Cycle (STLC):**
    * Requirement Analysis, Test Planning, Test Case Development, Test Environment Setup, Test Execution, Test Cycle Closure.
* **Principles of Testing:** (e.g., Testing shows presence of defects, not absence; Exhaustive testing is impossible; Defect clustering).
* **Quality Assurance (QA) vs. Quality Control (QC) vs. Testing:** Differentiating roles and responsibilities.
* **Test Plan:** Purpose, components (scope, objectives, resources, schedule, entry/exit criteria).
* **Test Case:** Attributes (ID, Description, Pre-conditions, Steps, Expected Result, Actual Result, Status).
* **Traceability Matrix:** Linking requirements to test cases, defects.
* **Defect/Bug Life Cycle:** Stages of a bug (New, Open, Assign, Test, Verify, Reopen, Closed, Deferred, Duplicate, Rejected).
* **Severity vs. Priority:** Understanding their classification and impact on bug fixing.

**🧠 Java Full Stack Examples:**
* Illustrate how requirements for a full-stack e-commerce application (e.g., "User must be able to log in") translate into specific test cases.
* Discuss how a defect found in the login API (backend) or login form (frontend) would go through the defect lifecycle.

**🗂️ Anna University Mapping (Unit I: INTRODUCTION TO SOFTWARE TESTING):**
* Introduction to Software Testing
* Objectives of software testing
* Software test strategies
* Testing methodologies
* Software testing process
* Test plan
* Test case
* Traceability Matrix
* Defect Management
* Defect Life Cycle
* Severity and Priority

**🛠️ Tools:**
* **Jira/Azure DevOps/Trello:** For defect tracking and test case management (conceptual overview for theory).
* **Spreadsheets (Excel/Google Sheets):** For creating simple traceability matrices and test cases.

**🔧 Practical Labs:**
* **Lab 1.1: Test Plan Creation:**
    * Given a simple requirement for a web application (e.g., user registration), draft a high-level test plan document.
* **Lab 1.2: Test Case and Traceability Matrix:**
    * For the user registration feature, write 5-7 detailed manual test cases.
    * Create a simple traceability matrix linking requirements to these test cases.
* **Lab 1.3: Defect Reporting:**
    * Simulate finding a defect in a provided mock application (or a public website example).
    * Write a clear, concise bug report including steps to reproduce, expected vs. actual results, severity, and priority.

**💬 Interview Qs:**
* **MCQs:**
    * Which phase comes after Test Execution in STLC? (A) Test Planning (B) Test Closure (C) Test Environment Setup (D) Test Case Development
    * What is the difference between severity and priority?
* **Scenario Qs:**
    * You find a bug where the "Add to Cart" button is intermittently unresponsive. How would you classify its severity and priority, and why?
    * A developer pushes a fix for a critical bug. What steps would you take to verify the fix and ensure no new issues are introduced?

---

### **Module 2: Test Techniques & Types of Testing**

This module delves into various test design techniques and different categories of testing, from component level to full system validation.

**📘 Theory:**
* **Test Techniques (Design Techniques):**
    * **Black-box Testing:** Definition, when to use.
        * **Equivalence Partitioning:** Dividing input data into valid and invalid partitions.
        * **Boundary Value Analysis (BVA):** Testing at the boundaries of input ranges.
        * **Decision Table Testing:** For complex business rules with multiple conditions.
        * **State Transition Testing:** For systems with distinct states and transitions (e.g., login status, order status).
        * **Use Case Testing:** Testing based on user interactions.
    * **White-box Testing:** Definition, when to use.
        * **Statement Coverage:** Executing every line of code.
        * **Decision Coverage (Branch Coverage):** Executing every branch of code.
        * **Condition Coverage:** Executing all conditions.
    * **Grey-box Testing:** Combination of black-box and white-box.
    * **Error Guessing:** Intuitively identifying potential error-prone areas.
* **Types of Testing:**
    * **Unit Testing:** Individual components/methods.
    * **Integration Testing:** Interaction between integrated modules/services.
    * **System Testing:** Testing the complete, integrated system.
    * **Regression Testing:** Ensuring new changes don't break existing functionality.
    * **Smoke Testing (Build Verification Test):** Quick test of core functionalities after a build.
    * **Sanity Testing:** Subset of regression testing, performed after minor changes.
    * **User Acceptance Testing (UAT) / Acceptance Testing:** Formal testing against business requirements.
    * **Performance Testing:** Load, Stress, Scalability, Volume testing.
    * **Security Testing:** Penetration testing, vulnerability scanning (basics).
    * **Recovery Testing:** How well the system recovers from crashes/failures.
    * **Installation Testing:** Verifying correct installation.

**🧠 Java Full Stack Examples:**
* **Unit Testing:** Testing a Java `UserService` method in isolation, mocking its dependencies (`UserRepository`).
* **Integration Testing:** Testing the interaction between a `UserController` and `UserService` in Spring Boot.
* **API Testing:** Using Postman to test backend REST APIs.
* **UI Testing:** Manual black-box testing of a React login page.
* **Performance Testing:** Conceptual discussion of loading a React app or hammering a Spring Boot API with many requests.

**🗂️ Anna University Mapping (Unit II: TEST DESIGN AND TEST PROCESS):**
* Test design strategies (Black-box, White-box, Grey-box).
* Test design techniques (Equivalence Partitioning, BVA, Decision Table, State Transition).
* Testing levels (Unit, Integration, System, Acceptance).
* Types of testing (Functional, Non-functional - Performance, Security, Usability etc.).
* Regression testing, Smoke and Sanity testing.

**🛠️ Tools:**
* **JUnit 5 / TestNG:** For Unit and Integration testing (theory and conceptual usage for now).
* **Postman:** For manual API testing.

**🔧 Practical Labs:**
* **Lab 2.1: Black-box Test Case Design:**
    * For a given input field (e.g., age 18-60), apply Equivalence Partitioning and Boundary Value Analysis to design test cases.
* **Lab 2.2: Decision Table Testing:**
    * Given a scenario with multiple conditions and actions (e.g., online discount rules), create a decision table and derive test cases.
* **Lab 2.3: Manual API Testing with Postman:**
    * Given a simple Spring Boot REST API, manually test `GET`, `POST`, `PUT`, `DELETE` endpoints using Postman.
    * Verify response status codes and JSON payloads.
* **Lab 2.4: Traceability and Defect Analysis:**
    * Map the test cases from Lab 2.1 and 2.2 back to requirements using a traceability matrix.
    * Analyze provided mock defect data for severity/priority trends.

**💬 Interview Qs:**
* **MCQs:**
    * Which test technique is primarily concerned with the internal structure of the code? (A) Black-box (B) White-box (C) Grey-box (D) Usability testing
    * When is Smoke Testing typically performed?
* **Scenario Qs:**
    * You are asked to test a new "password reset" feature. What types of testing would you prioritize, and why?
    * Describe a scenario where Boundary Value Analysis would be more effective than Equivalence Partitioning.

---

### **Module 3: Test Management, Metrics, and Automation Fundamentals**

This module covers the strategic aspects of test management, relevant metrics, and the foundational principles of test automation.

**📘 Theory:**
* **Test Management:**
    * **Test Strategy vs. Test Plan:** High-level organizational approach vs. project-specific details.
    * **Resource Estimation:** Techniques (e.g., Wideband Delphi, Three-Point Estimation).
    * **Test Scheduling:** Integrating testing into project timelines.
    * **Risk-Based Testing:** Prioritizing testing efforts based on perceived risks.
* **Test Metrics:**
    * **Test Coverage:** Code coverage (statement, branch), requirement coverage, test case coverage.
    * **Defect Density:** Number of defects per unit of code.
    * **Mean Time To Detect (MTTD):** Average time from defect introduction to detection.
    * **Mean Time To Fix (MTTF):** Average time to fix a defect.
    * **Test Effectiveness:** How good are tests at finding defects.
    * **Traceability (revisit):** Ensuring comprehensive linkage.
* **Version Control for QA:**
    * **Git Branching Strategy for QA:** How QA teams use branches (e.g., feature branches, release branches).
    * **Test Artifact Management:** Storing test cases, test data, automation scripts in Git.
* **Automation Basics:**
    * **When to Automate:** Criteria for choosing automation candidates (repetitive, stable, critical).
    * **ROI of Automation:** Justifying automation investment.
    * **Automation Pyramid:** Unit > Integration > UI tests, and their benefits.
    * **Characteristics of Good Automated Tests:** Reliable, maintainable, fast, independent.

**🧠 Java Full Stack Examples:**
* Discuss how test coverage metrics are collected for Java backend code (JUnit).
* Show how automation scripts (Selenium, Postman collections) are managed in a Git repository.
* Relate the automation pyramid to a full-stack architecture, emphasizing unit tests for Java services, API tests for REST endpoints, and fewer UI tests for React components.

**🗂️ Anna University Mapping (Unit III: TEST MANAGEMENT AND AUTOMATION BASICS):**
* Test management (Test strategy, planning, estimation, scheduling).
* Test metrics (Coverage, defect density, MTTD/MTTF).
* Introduction to test automation.
* When to automate and ROI.
* Automation pyramid.

**🛠️ Tools:**
* **Jira/Azure DevOps:** (revisit for advanced concepts like dashboards, reports).
* **Git/GitHub:** For practical management of test artifacts.
* **SonarQube (Conceptual):** For code quality and test coverage reporting.

**🔧 Practical Labs:**
* **Lab 3.1: Git Branching for Test Automation:**
    * Practice creating feature branches for test automation scripts, committing changes, and merging.
    * Manage sample test cases and automation scripts in a GitHub repository.
* **Lab 3.2: Analyze Code Coverage Report (Mock):**
    * Given a mock JUnit test coverage report (e.g., from JaCoCo), interpret statement and branch coverage percentages.
    * Discuss how to improve coverage.
* **Lab 3.3: Justifying Automation ROI (Spreadsheet):**
    * Given a hypothetical manual test suite, calculate the estimated time savings and ROI for automating parts of it over a year.

**💬 Interview Qs:**
* **MCQs:**
    * Which level of the automation pyramid usually has the most tests? (A) UI (B) API (C) Unit (D) Performance
    * What is the primary purpose of a test traceability matrix?
* **Scenario Qs:**
    * Your team wants to introduce test automation. How would you convince your manager of its ROI?
    * Describe a scenario where you would prioritize manual testing over automation.
    * How do you ensure test artifacts (like test plans and automation scripts) are version controlled effectively within a QA team?

---

### **Module 4: Practical Automation with Selenium, JUnit, TestNG & API Testing**

This module dives into the most common automation frameworks and tools for both UI and API testing, with a strong focus on Java implementation.

**📘 Theory:**
* **Selenium WebDriver:**
    * Architecture: WebDriver, Browser Drivers, Browsers.
    * Locators: ID, Name, ClassName, TagName, LinkText, PartialLinkText, CSS Selector, XPath (absolute vs. relative).
    * Waits: Implicit, Explicit (`WebDriverWait`), Fluent Waits.
    * Handling Alerts, Frames, Windows.
    * `Select` class for dropdowns.
    * Page Object Model (POM): Design pattern for robust, maintainable UI tests.
    * Cross-Browser Testing: Setting up tests for Chrome, Firefox, Edge.
* **JUnit & TestNG:**
    * **Assertions:** `assertEquals`, `assertTrue`, `assertNull`, etc.
    * Annotations: `@Test`, `@BeforeEach/@BeforeMethod`, `@AfterEach/@AfterMethod`, `@BeforeAll/@BeforeClass`, `@AfterAll/@AfterClass`.
    * Test Lifecycle and Execution Order.
    * Grouping Tests: Categories (JUnit), Groups (TestNG).
    * Parameterization: Running tests with multiple data sets.
    * Test Suites: Combining multiple test classes.
* **Maven/Gradle for Test Automation:**
    * Configuring test dependencies (`selenium-java`, `junit-jupiter-api`, `testng`, `webdrivermanager`).
    * Running test suites via build commands (`mvn test`).
    * Generating test reports (`maven-surefire-plugin`).
* **API Testing with Postman & Newman:**
    * Testing REST APIs (GET, POST, PUT, DELETE) programmatically.
    * Request Chaining: Using output from one request as input for another.
    * JSON Assertions: Validating response payloads.
    * Automation via Newman: Running Postman collections from the command line.

**🧠 Java Full Stack Examples:**
* **Selenium POM:** Creating Page Objects for a React login page (e.g., `LoginPage.java` with locators and methods).
* **JUnit for Backend Unit Tests:** Writing unit tests for Spring Boot service methods.
* **TestNG for End-to-End Tests:** Using TestNG to orchestrate a full end-to-end flow involving both API and UI interactions.
* **API Automation with Postman/Newman:** Testing the REST endpoints of a Spring Boot backend.

**🗂️ Anna University Mapping (Unit IV: TEST AUTOMATION):**
* Test automation framework (e.g., Selenium WebDriver).
* Unit Testing frameworks (JUnit, TestNG).
* Automated regression testing.
* API automation tools (Postman/Newman).

**🛠️ Tools:**
* **Selenium WebDriver:** The core tool.
* **JUnit 5:** Primary Java unit testing framework.
* **TestNG:** Powerful testing framework with advanced features.
* **Maven/Gradle:** Build automation for managing dependencies and running tests.
* **WebDriverManager:** For easy browser driver management.
* **Postman:** For manual and automated API testing.
* **Newman:** Postman Collection Runner for CLI automation.
* **IntelliJ IDEA/Eclipse:** IDEs for writing and debugging Java code.

**🔧 Practical Labs:**
* **Lab 4.1: Selenium Basics - Locators & Waits:**
    * Write a Selenium script to open Google, search for a term, and assert the title. Practice different locators and explicit waits.
* **Lab 4.2: Selenium Page Object Model (POM):**
    * Automate a login process for a sample web application (e.g., a test website or a simple React app you build).
    * Implement POM for the login page, separating locators and actions.
* **Lab 4.3: JUnit/TestNG for Unit Testing (Spring Boot):**
    * Write unit tests for a Spring Boot service layer method, using JUnit/TestNG assertions.
    * Explore `@BeforeEach`, `@AfterEach`, `@ParameterizedTest` (JUnit) or `@BeforeMethod`, `@AfterMethod`, `@@Parameters` (TestNG).
* **Lab 4.4: API Automation with Postman/Newman:**
    * Create a Postman collection to test the CRUD operations of a Spring Boot REST API.
    * Add tests to assert status codes and JSON response data.
    * Run the collection using Newman from the command line.

**💬 Interview Qs:**
* **MCQs:**
    * Which Selenium locator strategy is generally preferred for its robustness? (A) ClassName (B) XPath (C) ID (D) TagName
    * What is the purpose of `@BeforeAll` annotation in JUnit?
* **Scenario Qs:**
    * Explain the Page Object Model in Selenium. Why is it important?
    * You are automating a test case that involves waiting for an element to become clickable. Which Selenium wait strategy would you use, and why?
    * How do you manage test data for parameterized tests in JUnit/TestNG?
    * Describe how you would automate the testing of a REST API endpoint that requires data from a previous API call.

---

### **Module 5: Advanced Test Automation, CI/CD, and Quality Engineering**

This final module integrates testing into the DevOps pipeline, explores advanced automation techniques, and introduces concepts for holistic quality assurance.

**📘 Theory:**
* **Behavior-Driven Development (BDD) with Cucumber:**
    * **Gherkin Syntax:** `Given-When-Then` format for writing readable test scenarios.
    * **Feature Files:** Defining high-level business features.
    * **Step Definitions:** Mapping Gherkin steps to Java code.
    * Hooks (`@Before`, `@After`): Setting up/tearing down test environments.
* **Spring Boot Testing (In-depth):**
    * **Mocking with Mockito:** Stubbing dependencies for isolated testing (`@Mock`, `@InjectMocks`).
    * **Integration Tests:** Testing slices of the application (e.g., `@WebMvcTest`, `@DataJpaTest`).
    * **REST Controllers Testing with MockMvc:** Simulating HTTP requests without starting a full server.
* **React Testing (Basics):**
    * **Jest:** JavaScript testing framework.
    * **React Testing Library:** User-centric testing approach.
    * Simulating events, snapshot testing.
* **CI/CD Integration:**
    * **Jenkins/GitHub Actions:** Introduction to build automation servers.
    * How to auto-trigger test pipelines (on code commit, scheduled).
    * Integrating Maven/Gradle tests into CI/CD.
* **Test Reporting:**
    * **Allure Reports:** Rich, interactive test reports.
    * **ExtentReports / HTML Reports:** Generating human-readable reports.
    * **Test Dashboards:** Visualizing test results over time.
* **Performance Testing (Basics):**
    * **JMeter basics:** Recording requests, creating thread groups, listeners.
    * Load testing REST APIs.
* **Security & Compliance Testing (Basics):**
    * Common vulnerabilities: SQLi/XSS basic test cases (revisit from WAS course, focus on testing methods).
    * OWASP ZAP scanner integration in CI/CD (conceptual).
* **DevOps + Testing:**
    * **Docker Test Environment Setup:** Containerizing test dependencies (database, mock servers).
    * **Containerized Test Suites:** Running automation tests inside Docker containers.
    * **Test Orchestration:** Managing execution order and dependencies in complex test suites.
* **Static Code Analysis:**
    * **SonarQube:** For code quality, bug detection, security vulnerabilities, test coverage.
    * **PMD, Checkstyle:** For coding standards and style enforcement.
* **Test Data Management:**
    * Data creation scripts, environment isolation.
    * Data anonymization techniques (conceptual).

**🧠 Java Full Stack Examples:**
* **BDD for User Story:** Writing a Gherkin feature for a "User Login" and implementing step definitions using Selenium and Spring Boot API calls.
* **Spring Boot Mocking:** Mocking a `UserRepository` to test a `UserService` method that interacts with the database.
* **CI/CD Pipeline:** Demonstrating a `Jenkinsfile` or `GitHub Actions` workflow that builds a Spring Boot app, runs JUnit tests, and then runs Selenium UI tests.
* **JMeter for API Load Testing:** Creating a simple JMeter script to stress test a Spring Boot endpoint.

**🗂️ Anna University Mapping (Unit V: ADVANCED TESTING CONCEPTS):**
* Behavioral testing (BDD, Cucumber).
* Performance testing (JMeter).
* Security testing (Vulnerability scanning with ZAP/Burp - conceptual).
* Test automation in CI/CD pipeline.
* Test reporting tools.
* (Implicitly covers aspects of static analysis, test data management as part of advanced practices).

**🛠️ Tools:**
* **Cucumber-JVM:** For BDD implementation.
* **Mockito:** For mocking in Java unit tests.
* **Spring Boot Test Modules:** (`spring-boot-starter-test`, `@WebMvcTest`, `@DataJpaTest`).
* **Jest & React Testing Library:** For React component testing.
* **Jenkins / GitHub Actions:** CI/CD platforms.
* **Allure Reports / ExtentReports:** For generating rich test reports.
* **Apache JMeter:** For performance testing.
* **OWASP ZAP:** For basic security scanning.
* **Docker:** For setting up isolated test environments.
* **SonarQube:** For static code analysis and quality gates.

**🔧 Practical Labs:**
* **Lab 5.1: BDD with Cucumber:**
    * Write a Gherkin feature file for a simple user story (e.g., "Login with valid credentials").
    * Implement step definitions using Selenium WebDriver or Spring Boot API calls.
* **Lab 5.2: Spring Boot Integration Testing & Mocking:**
    * Write an integration test for a Spring Boot REST Controller using `MockMvc`.
    * Write a unit test for a `UserService` using Mockito to mock its `UserRepository` dependency.
* **Lab 5.3: CI/CD Pipeline for Test Automation:**
    * (Conceptual/Guided) Set up a basic Jenkins job or GitHub Actions workflow to:
        * Build your Spring Boot application (Maven/Gradle).
        * Run all JUnit/TestNG tests.
        * (Optional) Trigger a Selenium test suite.
        * Generate a test report (e.g., Surefire/Failsafe HTML report).
* **Lab 5.4: Basic Performance Test with JMeter:**
    * Create a simple JMeter test plan to send 100 concurrent requests to a Spring Boot REST API endpoint.
    * Analyze the aggregate report (throughput, response times).
* **Lab 5.5: Static Code Analysis (SonarQube Integration):**
    * Run SonarQube locally.
    * Integrate SonarQube with your Spring Boot Maven/Gradle project.
    * Analyze the generated report for code smells, bugs, and security vulnerabilities.

**💬 Interview Qs:**
* **MCQs:**
    * Which tool is commonly used for BDD in Java? (A) Selenium (B) JUnit (C) Cucumber (D) JMeter
    * What is the main purpose of `MockMvc` in Spring Boot testing?
* **Scenario Qs:**
    * **Scenario:** Your team wants to implement BDD. Explain to them what BDD is, why it's beneficial, and how Cucumber helps achieve it.
    * How would you set up a test environment for end-to-end UI automation using Docker?
    * Your CI pipeline takes too long to run all tests. How would you optimize it, considering the automation pyramid?
    * Describe how you would perform basic load testing on a new REST API endpoint.
    * A critical bug is reported in production. How can your testing practices and tools (like SonarQube, logging) help in faster detection and root cause analysis?

---

### **Testing from Requirement → Test Cases → CI/CD → Reporting Flow**

This section summarizes the complete testing workflow you will master:

1.  **Requirement Analysis:** Understand functional and non-functional requirements.
2.  **Test Planning:** Create a detailed Test Plan, define strategy, scope, resources.
3.  **Test Case Development:** Design manual test cases using techniques (EP, BVA, Decision Tables). Write Gherkin features for BDD.
4.  **Test Environment Setup:** Prepare test data, configure databases, mock external services, use Docker for isolated environments.
5.  **Test Automation (Shift Left):**
    * **Unit Tests (Java):** Write extensive JUnit/TestNG tests for individual methods/classes, using Mockito for dependencies.
    * **Integration Tests (Java/Spring Boot):** Test interactions between components (e.g., `Controller` with `Service`, `Service` with `Repository`). Use `MockMvc` for controller tests, `@DataJpaTest` for repository.
    * **API Tests (Java/Postman/Newman):** Automate REST API validation for backend endpoints.
    * **UI Tests (Java/Selenium/BDD):** Automate critical user flows using Selenium WebDriver with POM, potentially driven by Cucumber.
6.  **CI/CD Integration:**
    * Automate test execution within pipelines (Jenkins, GitHub Actions).
    * Integrate static code analysis (SonarQube), dependency scanning (OWASP Dependency-Check).
    * Set up quality gates.
7.  **Test Execution:** Run automated tests, perform exploratory testing, UAT.
8.  **Defect Management:** Log, track, and manage defects through their lifecycle.
9.  **Test Reporting & Metrics:** Generate comprehensive reports (Allure, ExtentReports), track key metrics (coverage, defect density, MTTD/MTTF), visualize results on dashboards.
10. **Regression Testing:** Automated regression suites run continuously.
