# 🚀 SonicFramework Documentation

## 1. Introduction
SonicFramework is a robust and scalable test automation framework built using **Playwright** with **TypeScript**. 🎯 It is designed to streamline automated UI and API testing with structured test management, custom fixtures, reporting, and CI/CD integration.

## 2. Project Structure 🏗️
The repository follows a modular structure for better maintainability:

### **Root Directory** 📂
- **.github/workflows/** – Contains CI/CD configurations for automated test execution ⚙️.
- **api/** – Houses API testing utilities, including request handlers and response validators 🌐.
- **constants/** – Stores global constants used across the framework 📌.
- **customFixtures/** – Contains custom Playwright fixtures to enhance test capabilities 🏗️.
- **data/** – Stores test data in JSON or CSV format 📊.
- **helpers/** – Utility functions for reusability across test scripts 🛠️.
- **logins/** – Manages authentication flows and user session handling 🔑.
- **pages/** – Implements Page Object Model (POM) to separate UI interactions 🖥️.
- **tests/** – Contains Playwright test cases and suites ✅.
- **customReporterConfig.ts** – Configures custom test reporting 📜.
- **global.setup.ts** – Prepares test environments before execution 🚦.
- **playwright.config.ts** – Stores Playwright configuration settings ⚙️.
- **tsconfig.json** – Configures TypeScript compiler options 📜.

## 3. Features ✨
- **Playwright Integration**: Enables powerful web automation with multi-browser support 🌍.
- **Custom Fixtures**: Enhances Playwright’s capabilities with reusable test utilities 🛠️.
- **Page Object Model (POM)**: Improves test maintainability and reusability 📄.
- **Custom Reporting**: Supports Playwright’s built-in reporters and additional integrations 📊.
- **Continuous Integration (CI/CD)**: Automates test execution through GitHub Actions 🚀.

## 4. Technologies Used 🖥️
- **TypeScript** – Strongly typed JavaScript for better maintainability 🔵.
- **Playwright** – Modern browser automation tool for UI testing 🌍.
- **Jest/Test Runner** – Manages and executes test cases ✅.
- **Allure Report** – Provides detailed test execution reports 📊.
- **GitHub Actions** – Automates testing and deployment 🔄.

## 5. Setup Instructions 🛠️
### **Prerequisites**
- Install **Node.js** (recommended v18 or higher) 📥
- Install **Playwright** globally:
  ```bash
  npm install -g playwright
  ```

### **Clone the Repository** 🔽
```bash
git clone https://github.com/majay3574/SonicFramework.git
cd SonicFramework
```

### **Install Dependencies** 📦
```bash
npm install
```

### **Run Tests** 🚀
```bash
npx playwright test
```

## 6. Running Tests 🏃‍♂️
### **Executing UI Tests** 🖥️
```bash
npx playwright test tests/ui
```

### **Executing API Tests** 🌐
```bash
npx playwright test tests/api
```

### **Running Tests with Custom Configuration** ⚙️
```bash
npx playwright test --config=playwright.config.ts
```

### **Headless Mode Execution** 👀
```bash
npx playwright test --headless
```

## 7. Reporting 📊
### **Playwright Report**
To generate and view test execution reports:
```bash
npx playwright show-report
```

### **Allure Report** 🌟
To use **Allure** for advanced test reports:
```bash
npm install --save-dev allure-playwright
npx allure generate allure-results --clean -o allure-report
npx allure open allure-report
```

## 8. CI/CD Integration 🔄
The framework integrates with **GitHub Actions** for automated test execution. The workflow is defined in `.github/workflows/ci.yml`.

### **Triggering Tests in CI/CD** 🚦
The tests run automatically on **push** and **pull request** events. Manual triggering can be done using:
```bash
gh workflow run ci.yml
```

## 9. Best Practices 🏆
- **Use POM structure** to separate UI interactions from test logic 📄.
- **Leverage fixtures** for test setup and teardown 🔄.
- **Use environment variables** to manage credentials securely 🔑.
- **Run tests in parallel** for improved execution speed 🚀.
- **Integrate CI/CD** to automate testing workflows ⚙️.

## 10. Conclusion 🎯
SonicFramework is a scalable and efficient test automation solution leveraging Playwright. Its modular architecture, integration capabilities, and reporting tools make it ideal for modern UI and API testing needs. ✅

