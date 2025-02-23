# [software-testing-assistance-with-github-copilot-ai](https://www.linkedin.com/learning/software-testing-assistance-with-github-copilot-ai/)

# 1. Overview
## 1.1. What is GitHub Copilot?
- As we know GitHub Copilot is an AI coding assistant that helps with code completion, identifying bugs, and understanding code.
- It works primarily through code completion and chat features, suggesting solutions as you type and allowing you to interact with it through your IDE.
- Copilot can be enabled in various IDEs by installing the Copilot extension and connecting it to your GitHub account.
- It offers valuable functionalities like explaining code, translating code snippets, and creating complex shell commands.

## 1.2. Copilot for Code Completion
**Code Completion:** GitHub Copilot provides code suggestions as you type, helping to complete functions, conditionals, and other code structures.

**Prompting Copilot:** You can prompt Copilot by starting a function, writing a comment, or creating a new file. It will then suggest relevant code.

**Flexibility and Accuracy:** While Copilot's suggestions can significantly increase your output, it's important to review and refine its suggestions to ensure accuracy and relevance.

## 1.3. Chatting with Copilot
**Code Explanation and Generation:** Copilot Chat can explain sections of code, generate comments, and even create new code based on your prompts.

**Versatility:** You can ask Copilot to perform various tasks, such as explaining code, generating classes in different languages, and writing tests for highlighted code.

**Slash Commands:** Using slash commands like /fix and /optimize, you can prompt Copilot to identify and fix issues or optimize code for faster execution.

## 1.4. Automated Testing
**Automated Testing Basics:** Automated testing involves creating statements of fact about your code to identify any changes that violate these facts.

**Simple Example:** The instructor demonstrates a simple add function and how to write a test for it using phpunit, a testing framework.

**Importance of Execution:** Tests need to be executed to provide value, and they should cover various scenarios to prevent regressions.

## 1.5. Configuring a Testsuite
**Test Conventions:** Understand the test conventions in your programming language, such as where to place test files and how to structure them.

**AAA Pattern:** Use the Arrange, Act, Assert (AAA) pattern to structure your tests: set up the test environment, perform the action, and then assert the outcome.

**Mocking:** Utilize mocking to isolate the logic being tested, especially when dealing with external dependencies.

**Framework Support:** Some frameworks have better support for testing out of the box, and it's often easier to comply with their conventions.


## 1.6. AI and Automated Testing
**AI Support for Testing:** AI, like GitHub Copilot, can assist in writing and refactoring tests, improving test coverage and code quality.

**Identifying Testable Code:** It's crucial to identify which parts of your code are testable to effectively use AI for generating tests.

**Initial Test Setup:** Start with simple tests, such as asserting that true equals true, to ensure your test configuration is correct.

**Refactoring with AI:** Use AI tools to refactor complex functions into smaller, testable units, enhancing the overall testability of your code.

# 2. Add Testing to Existing Code with Copilot
## 2.1. Identifying Testable Code
**Testable Code:** All code is testable, but some code is harder to test than others. Writing code with testing in mind helps in identifying patterns that make testing easier.

**Real-World Example:** The instructor uses a real-world example to demonstrate how to refactor a complex function into simpler, testable units.

**Test-Driven Development (TDD):** Emphasizes the importance of TDD by writing tests first and then refactoring the code to meet those tests, ensuring better code quality and maintainability.

## 2.2. Generate Tests with Copilot
**Generating Tests with Copilot:** The instructor demonstrates how to use GitHub Copilot to generate a test for a function, such as the slugify function.

**Running Specific Tests:** Learn how to run specific tests using the file path to ensure that the generated tests work correctly.

**Refining Tests:** The importance of limiting assertions per test and adding more methods to the test class for better test management and accuracy.

## 2.3. Refactoring with Copilot
**Refactoring for Improvement:** Refactoring involves making small changes to improve the code base, such as identifying brittle functions and adding tests to prevent regressions.

**Using GitHub Copilot:** GitHub Copilot can assist in creating tests and refactoring code by generating test cases and simplifying complex conditionals.

**Extracting Responsibilities:** Breaking down functions with too much responsibility into smaller, single-responsibility functions can make the code cleaner and easier to test.


## 2.4. Copilor Slash Commands
**Slash Commands:** GitHub Copilot offers various slash commands like /doc, /explain, and /optimize to help with documentation, code explanation, and optimization.

**Context Awareness:** Copilot considers different parts of your IDE, such as test results, build logs, and the active Git repository, to provide relevant suggestions.

**Practical Use:** Commands like fix can help resolve syntax issues, and optimize can improve runtime performance, but it's important to keep code legible for your team.


# 3. Use Copilot to Generate Code from Tests
## 3.1. Generating Tests to Document Business Logic
**Documenting Business Logic:** Automated tests can serve as documentation for the intent of your business logic, making it easier for new developers to understand the codebase.

**Using GitHub Copilot:** GitHub Copilot can assist in generating tests by suggesting solid test cases based on the context of your code.

**Identifying Breakages:** Tests can highlight breakages and areas that need fixing, which helps in maintaining code quality.

**Future Improvements:** Incomplete tests can document decisions that need to be made, providing a roadmap for future improvements.

## 3.2. Generating Code from Tests

**Test-Driven Development (TDD):** TDD involves writing tests first and then writing the minimum code necessary to make them pass, ensuring that the code meets the requirements.

**Using GitHub Copilot:** GitHub Copilot can generate code based on the tests you write, helping you implement the necessary logic to pass the tests.

**Refactoring and Code Quality:** Refactoring code to remove duplicate logic and improve code quality is essential for maintaining a clean and efficient codebase.

**Value Objects:** Value objects are immutable objects representing specific values without identity, helping in organizing and managing code more effectively.


## 3.3. Update Functionality with by Writing More Tests

**Contextual Code Generation:** GitHub Copilot uses the context of your open code to generate relevant code, but it may include extra, unnecessary parts that need manual removal.

**Importance of Testing:** Running tests after making changes ensures that the code remains functional and helps identify any issues caused by the changes.

**Documenting and Refactoring:** Documenting relationships and logic in comments before jumping into code helps create a clear path forward. Refactoring is essential to clean up messy code and remove duplicated logic.


# 4. Real-World Benefits
## 4.1. Code Quality and Maintainability

**Higher Quality Code:** Writing tests forces you to think through execution paths and simplify logic, leading to higher quality code.

**Documentation through Tests:** Tests serve as documentation, making it easier for new developers to understand what specific functions are supposed to do.

**Refactoring with AI:** GitHub Copilot can assist in refactoring code by suggesting improvements, helping maintain code quality and consistency.


## 4.2. Running Tests in CI/CD Pipelines

**CI/CD Integration:** Continuous Integration and Continuous Delivery (CI/CD) practices enable frequent and reliable deployment of small changes to production, ensuring that automated tests are run regularly.

**GitHub Actions:** The video demonstrates how to set up GitHub Actions to automate the running of tests on events like pull requests, helping to catch regressions early.

**Importance of Automated Testing:** Regularly running automated tests in a CI/CD pipeline helps maintain code quality and reduces the risk of new bugs being introduced.

## 4.3. Limiting Risk by Limiting Exposure

**Early Detection:** Tests are crucial for early detection of side effects caused by code changes, helping to limit risk.

**Small, Tested Functions:** Writing code that solves specific problems results in small, tested functions and classes that can be assembled into larger systems.

**Test-Driven Development (TDD):** Following Kent Beck's TDD approach, start with writing tests to capture requirements and edge cases, which helps in building stable and predictable systems.


https://github.com/features/copilot/

https://docs.github.com/en/copilot/about-github-copilot

https://docs.github.com/en/copilot/github-copilot-in-the-cli/about-github-copilot-in-the-cli

https://github.com/LinkedInLearning/software-testing-assistance-with-GitHub-Copilot-AI-3904213/codespaces


