# Vending Machine 

```markdown
# Vending Machine - State Transition Testing

## 📋 Project Overview

This project focuses on modeling and testing the **state transitions** of a vending machine using a **Model-Based Testing** approach. The main technique used is **State Transition Testing**, ideal for systems where outputs change depending on the current state and input.

---

## 🎯 Objective

- Validate correct transitions between defined states.
- Ensure proper system responses under both normal and exceptional conditions.
- Confirm correct handling of edge cases like timeouts, insufficient funds, and out-of-stock scenarios.

---

## 🔁 State Transition Model

The vending machine operates through the following states:

- `Idle`
- `Selecting Product`
- `Dispensing`
- `Out of Stock`

### Transition Events:
- Coin Insertion
- Product Selection
- Dispensing Completion
- Cancel Transaction
- Product Unavailability
- Invalid Selection
- Insufficient Funds
- Timeout (no input)

Refer to the included state transition diagram in the `/docs` folder.

---

## ✅ Test Strategy

### ✔ Test Scope
- Functional testing of user interactions.
- Focus on transitions and behavior during abnormal inputs or system states.

### ✔ Test Cases
10 test cases were defined to cover:
- Valid state transitions
- Exceptional scenarios
- Edge cases and timeouts

> ✅ 9 Passed | ❌ 1 Failed (coin not returned on out-of-stock)

Test cases and results are available in `test_cases.md`.

---

## 🧪 Sample Test Case

```

Test Case ID: TC2

Title: Product Selection after Coin Insertion

Initial State: Selecting Product

Event: Product Selection

Expected Output: Product is dispensed

Final State: Dispensing

```

---

## ⚠ Risk Management

| Risk ID | Description | Mitigation |
|--------|-------------|------------|
| PR-01 | Tight deadlines may impact thorough testing | Prioritize critical test paths |
| PR-02 | Limited testing tools | Use automation, task redistribution |
| PR-03 | Late requirement changes | Freeze scope during testing phase |

See full list in `risk_management.md`.

---

## 🔍 White-Box Testing

- Control Flow Graph created for core logic
- Line, branch, and path coverage applied
- Sample code snippets available in `/src` directory

---

## 📊 Traceability Matrix

Mapped requirements to test conditions and cases. Ensures full coverage and aligns with acceptance criteria.

---

## 🚀 Future Enhancements

- Add a maintenance mode and refill button
- Enable mobile payment support
- Introduce audio/LED feedback
- Implement energy-saving idle mode

---

## 🧰 Tech Stack

- Python simulation framework (for state transitions)
- Markdown for documentation
- Git for version control

---

## 📁 Project Structure

```

.

├── /src                  # Simulation code (Python)

├── /docs                 # Diagrams, charts, GUI sketches

├── test_cases.md         # Defined test scenarios

├── risk_management.md    # Risk and incident tracking

├── README.md             # Project overview (this file)

└── report.pdf            # Final report with detailed analysis

```

---

## 👨‍💻 Contributors

- (Nada Elmokdem, Malak Mosaad,Heba Amer, Youmna Hesham)

---

## 📌 Conclusion

This project ensures a robust testing model for vending machines using **State Transition Testing**. It captures both normal flow and edge case behavior to ensure reliability, accuracy, and a strong user experience.

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

```
