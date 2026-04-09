# APT1030-A — Fundamentals of Programming Languages

> **Course:** APT1030-A | **Level:** 1–7 | **Institution:** [Your Institution Name]

A comprehensive coursework project covering core programming language concepts through seven progressive levels, each grounded in real-world Kenyan contexts — from eCitizen login systems to mobile money DSLs.

---

## 📁 Repository Structure

```
APT1030-A/
├── Level1_Syntax_Semantics/
│   ├── login_validation.py
│   ├── LoginValidation.java
│   ├── login_validation.cpp
│   └── error_analysis.md
├── Level2_Data_Types/
│   ├── sacco_records.py
│   ├── SaccoRecords.java
│   └── type_analysis.md
├── Level3_Control_Flow/
│   ├── drought_advisory.py
│   ├── DroughtAdvisory.java
│   └── readability_comparison.md
├── Level4_Abstraction_Modularity/
│   ├── nhif_claims/
│   │   ├── Patient.java
│   │   ├── ClaimsProcessor.java
│   │   └── nhif_claims.py
│   └── procedural_refactor/
├── Level5_Paradigm_Comparison/
│   ├── pricing_procedural.cpp
│   ├── PricingOOP.java
│   └── pricing_functional.py
├── Level6_Scope_Memory_Errors/
│   ├── access_control.py
│   ├── AccessControl.java
│   └── scope_experiment.md
├── Level7_Capstone_DSL/
│   ├── parser.py
│   ├── interpreter.py
│   └── reflection.md
└── README.md
```

---

## 🗂️ Levels Overview

### Level 1 — Syntax, Semantics & Program Correctness
**Context:** eCitizen Login Validation System

Implements a login validation program in Python, Java, and C++ that checks hardcoded credentials (`adminKE` / `254Secure`) and prints `Access Granted` or `Invalid Credentials`.

Key analysis:
- Syntax errors introduced and documented per language
- Logical error (wrong comparison operator) explained — why it compiles but fails

---

### Level 2 — Data Types & Type Systems
**Context:** SACCO Member Financial Record

Stores member name, ID, monthly contribution, and computes total savings over 6 months.

Key analysis:
- Static vs dynamic typing observed when assigning a string to a numeric field
- Justification for static typing in financial systems vs dynamic typing in startup environments

---

### Level 3 — Control Flow & Decision Systems
**Context:** Drought Advisory Logic (Machakos County)

Rainfall advisory program using the following rules:
- `< 200mm` → *Irrigation Required*
- `≥ 200mm` and `temp > 30°C` → *Monitor Soil*
- Otherwise → *Normal Conditions*

Includes a rewrite using nested `if` statements and `switch` (Java/C++) with readability comparison.

---

### Level 4 — Abstraction & Modularity
**Context:** NHIF Claims Processing

OOP design with a `Patient` class (name, policy number) and a `calculateClaim(amount)` method that deducts a 10% co-payment. Also includes a procedural refactor for comparison of maintainability.

---

### Level 5 — Paradigm Comparison
**Context:** Ride-Hailing Pricing Engine (Nairobi)

Fare formula: `Total = 200 + (50 × distance)`

Implemented in three paradigms:
| Paradigm | Language |
|---|---|
| Procedural | C++ |
| Object-Oriented | Java or Python |
| Functional (lambda) | Python |

Includes analysis of which paradigm scales best when surge pricing is added.

---

### Level 6 — Scope, Memory & Error Handling
**Context:** Patient Record Access Control

`checkAccess(role)` function raises an error if the role is not `"Doctor"`. Demonstrates:
- Exception handling in Python (`try/except`)
- Structured error handling in Java (`try-catch`)
- Scope experiment: variable declared inside a function, accessed outside

Analysis covers why lexical scope improves security and the risks of dynamic scope in hospital systems.

---

### Level 7 — Capstone: Mini DSL for Mobile Money Rules
**Context:** Mobile Money Transaction Rules

Parses and interprets commands of the form:
```
TRANSFER 5000 FROM A TO B IF BALANCE > 1000
```

Built in Python. The parser extracts amount, sender, and receiver; the interpreter validates balance and prints the transaction result.

Reflection covers:
- Why Python suits DSL prototyping
- Why C++ would be harder for rapid rule iteration
- How AI code assistants can accelerate DSL development in Kenya

---

## 🛠️ Languages Used

- Python 3.x
- Java (JDK 17+)
- C++ (C++17)

---

## ▶️ How to Run

**Python**
```bash
python Level1_Syntax_Semantics/login_validation.py
```

**Java**
```bash
cd Level1_Syntax_Semantics
javac LoginValidation.java
java LoginValidation
```

**C++**
```bash
cd Level1_Syntax_Semantics
g++ -o login login_validation.cpp
./login
```

---

## 📚 Key Concepts Covered

- Syntax vs semantics; compilation vs interpretation
- Static vs dynamic typing; type coercion
- Control flow: `if-else`, nested conditions, loops, `switch`
- OOP: classes, encapsulation, methods
- Programming paradigms: procedural, OOP, functional
- Scope, variable lifetime, exception handling, stack vs heap
- DSL design: parsing and interpretation

---

## ✍️ Author

**[Your Full Name]**  
Student ID: [Your Student ID]  
Course: APT1030-A — Fundamentals of Programming Languages  
[Your Institution] | [Year]

---

## 📄 License

This project is submitted for academic purposes only.
