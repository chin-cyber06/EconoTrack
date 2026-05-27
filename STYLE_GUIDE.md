# EconoTrack — Team Style Guide

This document contains the official coding standards, naming conventions, formatting rules, and Git workflow guidelines for **Group 5 – EconoTrack**. All members are expected to follow these rules to maintain consistency in documentation, design assets, and future system development for the Butuan City LGU project.

---

# 1. Naming Conventions

To maintain consistency in our prototype, database structure, and future source code, the following naming conventions will be used:

| Element | Convention | Example |
| :--- | :--- | :--- |
| Variables | camelCase | `registeredBusinessCount` |
| Functions / Methods | camelCase | `updateApplicationStatus()` |
| Classes | PascalCase | `AdminDashboard` |
| Files | kebab-case | `admin-dashboard.html` |
| Constants | UPPER_SNAKE_CASE | `PRIMARY_VIOLET` |
| Database Tables | snake_case | `business_permits` |
| Database Fields | snake_case | `application_status` |

---

# 2. Formatting Rules

The following formatting rules should be followed for cleaner and more readable code:

- **Indentation:** Use **4 spaces** only.
- **Line Length Limit:** Maximum of **100 characters** per line.
- **Brace Style:** Use **One True Brace Style (1TBS)**.
    ```javascript
    if (applicationStatus === "approved") {
        displaySuccessBadge();
    }
    ```
- **Spaces vs. Tabs:** Tabs should automatically convert into 4 spaces.
- **Blank Lines:** Leave 1 blank line between functions or sections.
- **Max Function Length:** Functions should not exceed **50 lines** whenever possible.

---

# 3. Commenting Standards

Comments should help explain important parts of the code and improve readability.

- **File Header Comments:** Every major script file should contain a short description at the top.
    ```javascript
    /**
     * @file admin-dashboard.js
     * @description Dashboard rendering logic for EconoTrack
     * @author Cafe, Shayna
     * @date May 2026
     */
    ```

- **Function Comments:** Use JSDoc comments for functions.
    ```javascript
    /**
     * Updates the dashboard status counters.
     * @param {string} statusId
     * @param {number} totalCount
     * @returns {boolean}
     */
    ```

- **Inline Comments:** Use only when necessary for complex logic.
- **TODO Format Example:**
    ```javascript
    // TODO (Andrea): Connect table data to backend dataset
    ```
- **Language:** Comments must be written in English.

---

# 4. Branch Naming Strategy

Branch names should clearly describe their purpose and use lowercase letters with hyphens.

| Branch Type | Format | Example |
| :--- | :--- | :--- |
| Feature | `feature/<name>` | `feature/admin-sidebar` |
| Bug Fix | `bugfix/<name>` | `bugfix/status-badge-fix` |
| Hotfix | `hotfix/<name>` | `hotfix/signout-link-fix` |
| Release | `release/<version>` | `release/v1.0.0` |
