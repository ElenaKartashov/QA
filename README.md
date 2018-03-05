




Test Automation Framework Manual







Framework Overview
1.1.	Technology landscape
Test automation framework is comprised of 2 key components:
•	Framework page object model that accommodates all necessary cross project features and technologies
•	Infrastructure and tools that facilitate scalable, distributed and reliable test execution and reporting.
Page object model is a technology solution that accommodates essential features needed for success implementation. Framework has been built with the following common goals in mind:
•	Equip both technical and non-technical people with straightforward tool for test design, test data management, test execution and reporting
•	Design and implement reusable and low maintenance framework with essential features and infrastructure to be reused across all projects
•	Incorporate test automation into automated build-deploy process to enable continuous assessment of build quality
Framework leverages a number of open source technologies and custom source code. 
It is based on Python language, open source technology stack and open industry standards such as unittest, XML, JSON, Selenium, REST WS, Panda, Allure and others. The table below outlines the technology stack which is currently in use.

Technology
Covers
Notes
Selenium WebDriver, Python
Web UI, Database, PDF, Mobile Web, Mobile Native, Web Services, integration with other open source frameworks and tools
Open Source
Python
Primary scripting language
Open Source
Pytest allure adaptor
Execution report
Open Source
Selenium libraries
Web iOS apps
Open Source
Pytest, unittest
Test structure libraries
Open Source
Panda 0.22
Excel/CSV file interaction
All open source.

Intelij IDEA (Python plugin)


Integration and execution from CI
Open Source + JPMC already has license version
Jenkins
CI, test execution planning
OpenSource

1.2.	Test design
Test automation Framework provides the following approaches of test design and execution:
•	Data-driven - Excel/CSV (e.g. PS BRD files or test matrixes)
•	Behavior/keyword-driven - User story keyword based testing
•	Hybrid - Excel based parameterized Data/Behavior/Keyword-driven approach
For example: keyword “Build an XML 10X Acord file with all test data from column C”
Test designer can come up with best fit approach for their current needs and then design test and data accordingly. Pure Behavior-driven (BDD) works better for testing new functionality and may serve as a basis for acceptance testing of a User story. Data-driven and hybrid approaches serve better for regression testing and when massive amount of data/fields involved in testing.

1.3.	Test execution 
Test execution will be flexible and configurable through Context Manger component of Framework. The context will specify environments, test suites for execution, test data and other variables. The following types of execution will be available:
•	On demand locally
•	On demand remotely via Selenium Grid and scripting on Test automation server
•	On demand remotely via Jenkins dedicated automation server
•	Scheduled/triggered execution initiated from Build-deploy or and CI server.

1.4.	Test reporting
Allure library was integrated into the Framework in order to facilitate consistent and transparent test reporting across all types of test design approaches and projects.
Web based report is generated at the end of each execution cycle (test set execution) and accomodates full traceability for BDD and data-driven types of tests.


