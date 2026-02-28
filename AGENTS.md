```markdown
# AGENTS.md File Guidelines

These guidelines are designed to ensure a consistent, high-quality, and maintainable codebase for our AI coding agents. Adherence to these principles is crucial for project success and long-term viability.

## 1. DRY (Don't Repeat Yourself)

*   **Single Responsibility Principle:** Each agent module should have a single, well-defined purpose. Avoid creating functions or classes with overlapping functionality.
*   **Code Reuse:**  Leverage existing components and libraries whenever possible.
*   **Abstraction:**  Design agents to be abstract, allowing for easy swapping of implementations without modifying core logic.  Implementations should be robust and handle edge cases gracefully.
*   **Consistent Design:** Utilize consistent naming conventions, data structures, and coding styles across the codebase.

## 2. KISS (Keep It Simple, Stupid)

*   **Minimize Complexity:**  Favor straightforward logic and avoid over-engineering.
*   **Readability:**  Code should be easy to understand for other developers (including future you!).
*   **Concise Logic:** Strive for short, well-commented code.  Avoid overly verbose expressions.
*   **Clear Intent:** Each line of code should have a clear, understandable purpose.

## 3. SOLID Principles

*   **Single Responsibility:**  As stated above.
*   **Open/Closed Principle:**  Agents should be extensible through public interfaces, not modifications to their internal code.
*   **Liskov Substitution Principle:**  Subclasses should be substitutable for their base classes without altering the correctness of the program.
*   **Interface Segregation Principle:**  Clients should not be forced to depend on methods they do not use.
*   **Dependency Inversion Principle:**  High-level modules (agents) should not depend on low-level modules (dependencies).  Interfaces define contracts.

## 4. YAGNI (You Aren't Gonna Need It)

*   **Avoid Unnecessary Code:**  Don’t write functionality that isn’t currently required.  Defer implementation details to later iterations.
*   **Future-Proofing:**  Base solutions on a solid foundation; prioritize design over immediate solutions.

## 5. Code Length & Structure

*   **Maximum Code Length:** 180 lines of code per file.
*   **File Structure:**
    *   `src/agent/[agent_name].py` – Contains the core logic of the agent.
    *   `src/utils/` – Contains utility functions and helper classes.
    *   `src/tests/` – Contains unit and integration tests.
    *   `src/config/` – Contains configuration parameters.
    *   `src/data/` – Contains data structures and associated functions.
    *   `src/error/` – Error handling and handling specific error types.
*   **Modularization:** Break down agents into logical modules with clear responsibilities.
*   **Docstrings:**  Comprehensive docstrings should be provided for each function and class, explaining their purpose, inputs, and outputs.  Docstrings should be formatted using a consistent style.

## 6. Testing

*   **All Development Must Be Productive:**  Prioritize test-driven development.
*   **Mocking Strategy:**  Use mocks and stubs extensively for testing.  Avoid reliance on external data sources during testing.
*   **Test Coverage:**  Ensure at least 80% of code is covered by tests.
*   **Test Cases:**  Each function and class should have a set of test cases covering various scenarios.
*   **Unit Tests:** Focus on individual functions and classes.
*   **Integration Tests:** Verify interactions between agents and other components.
*   **End-to-End Tests:**  Simulate real-world user interactions.
*   **Test Data Management:** Implement a reliable and adaptable test data management system.

## 7.  Documentation & Comments

*   **Inline Comments:** Use concise, helpful comments to explain complex logic.
*   **Docstring Formatting:** Use a consistent docstring format (e.g., Google Style).
*   **README:** Provide a README with a brief description of the project, instructions for running the agent, and relevant dependencies.

## 8.  General Principles

*   **Error Handling:** Implement robust error handling to prevent unexpected crashes.  Log errors appropriately.
*   **Logging:** Use a logging library to provide detailed debugging information.
*   **Configuration:**  Use a robust configuration system to manage agent settings.
*   **Version Control:** Use Git for version control.

These guidelines are a living document and should be reviewed and updated periodically. Any changes must be properly documented and communicated.
```