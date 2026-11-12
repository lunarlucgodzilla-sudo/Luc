# Session 2: Edge Cases & Boundary Testing Portfolio Module

## 1. Objective
To demonstrate proficiency in identifying and documenting edge cases, boundary value analysis, and negative testing scenarios for a web input form.

## 2. Target Feature Scenario
* **Feature:** User Account Registration Age Input Field
* **Acceptance Criteria:** Users must be between 18 and 120 years old to register.

## 3. Boundary Value Analysis (BVA) & Test Cases
| Test ID | Scenario / Description | Input Value | Expected Result | Pass/Fail |
| :--- | :--- | :--- | :--- | :--- |
| **TC_BE_01** | Lower Boundary (Just below limit) | 17 | Error: "Must be at least 18 years old" | [ ] |
| **TC_BE_02** | Lower Boundary (Exact limit) | 18 | Success: Account created | [ ] |
| **TC_BE_03** | Lower Boundary (Just above limit) | 19 | Success: Account created | [ ] |
| **TC_BE_04** | Upper Boundary (Just below limit) | 119 | Success: Account created | [ ] |
| **TC_BE_05** | Upper Boundary (Exact limit) | 120 | Success: Account created | [ ] |
| **TC_BE_06** | Upper Boundary (Just above limit) | 121 | Error: "Invalid age entered" | [ ] |

## 4. Negative & Edge Case Testing
| Test ID | Edge Case Description | Input / Action | Expected Result | Pass/Fail |
| :--- | :--- | :--- | :--- | :--- |
| **TC_NE_01** | Alphabetical Input | "eighteen" | Error: "Only numeric values allowed" | [ ] |
| **TC_NE_02** | Special Characters | "!@#$" | Error: "Invalid characters" | [ ] |
| **TC_NE_03** | Blank / Empty Field | [ Leave Empty ] | Error: "Field cannot be blank" | [ ] |
| **TC_NE_04** | Negative Numbers | -5 | Error: "Age cannot be negative" | [ ] |
