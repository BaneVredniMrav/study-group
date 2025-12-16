# ChessKid E2E Playwright Test Automation

Automated end-to-end testing for the ChessKid platform using [Playwright](https://playwright.dev/).

---

## Table of Contents

1. [Prerequisites](#prerequisites)
2. [Installation & Setup](#installation--setup)
3. [Project Overview](#project-overview)
4. [Project Structure](#project-structure)
5. [Configuration](#configuration)
6. [Running Tests](#running-tests)
7. [Test Tags & Filtering](#test-tags--filtering)
8. [Test Reports](#test-reports)
9. [Best Practices](#best-practices)
10. [CI/CD Integration](#cicd-integration)
11. [Troubleshooting](#troubleshooting)
12. [Contributing](#contributing)

---

## Prerequisites

- [Node.js](https://nodejs.org/) (v16+ recommended)
- [npm](https://www.npmjs.com/) (comes with Node.js)

Check versions:

```bash
node -v
npm -v
```

---

## Installation & Setup

1.  **Clone the repository:**

    ```bash
    # Clone the repository
    git clone https://github.com/BaneVredniMrav/study-group.git

    # Navigate into the project directory
    cd study-group
    ```

2.  **Install dependencies:**

    ```bash
    npm install
    ```

3.  **Install Playwright browsers:**

    ```bash
    npx playwright install
    ```

4.  **(Optional) Install TypeScript globally:**

    ```bash
    npm install -g typescript
    ```

5.  **Verify Playwright installation:**
    ```bash
    npx playwright --version
    ```

---

## Project Overview

This project automates end-to-end tests for ChessKid using Playwright. It follows the Page Object Model (POM) for maintainability and scalability, and supports running tests locally or in CI/CD pipelines.

---

## Project Structure

```bash
/pages             # Page Object Model (POM) classes for pages & flows
/tests                # Test cases
package-lock.json     # Dependency lock file
package.json          # Project dependencies
playwright.config.ts  # Playwright configuration
README.md             # Project documentation
```

---

## Running Tests

- **Run all tests:**

    ```bash
    npx playwright test
    ```

- **Run tests with UI:**

    ```bash
    npx playwright test --ui
    ```

- **Run specific test file:**
    ```bash
    npx playwright test tests/feature/example.spec.ts
    ```

---

## Test Tags & Filtering

- Use `@tag` in test titles or comments.
- Filter tests by tag:
    ```bash
    npx playwright test --grep @sanity
    ```

---

## Contributing

1. Fork the repo and create your branch.
2. Make your changes and add tests.
3. Run all tests locally.
4. Submit a pull request.

---
