# APT1030-A — Fundamentals of Programming Languages

> **Course:** APT1030-A | **Level:** 1–7 | **Institution:** [Your Institution Name]

A comprehensive coursework project covering core programming language concepts through seven progressive levels, each grounded in real-world Kenyan contexts — from eCitizen login systems to mobile money DSLs.

---

##  Repository Structure

```
APT_COURSEWORK_1/
├── APT Level 1/
│   ├── ECitizenLogin.java
│   ├── Login Validation.cpp
│   ├── Login Validation.py
│   └── error_analysis.md
├── APT Level 2/
│   ├── sacco_records.py
│   ├── SaccoRecords.java
│   └── type_analysis.md
├── APT Level 3/
│   ├── Java/
│   │   ├── Main.java
│   │   └── MainNested.java
│   └── Python/
│       ├── advisory.py
│       └── advisory_nested.py
├── APT Level 4/
│   ├── JAVA/
│   │   └── Patient.java
│   └── Python/
│       ├── nhif_oop.py
│       └── python-procedural.py
├── APT Level 5/
│   ├── fare.cpp
│   ├── python-LAMBA.py
│   └── python-OOP.py
├── APT Level 6/
│   ├── Main.java
│   ├── python(exceptions).py
│   └── python(scope).py
├── APT Level 7/
│   └── main.py
└── README.md
```

---

## Levels Overview

### Level 1 — Syntax, Semantics & Program Correctness
**Context:** eCitizen Login Validation System

Implements a login validation program in Python, Java, and C++ that checks hardcoded credentials (`adminKE` / `254Secure`) and prints `Access Granted` or `Invalid Credentials`.

| File | Language |
|---|---|
| `ECitizenLogin.java` | Java |
| `Login Validation.cpp` | C++ |
| `Login Validation.py` | Python |
| `error_analysis.md` | Analysis |

Key analysis:
- Syntax errors introduced and documented per language
- Logical error (wrong comparison operator) explained — why it compiles but behaves incorrectly

---

### Level 2 — Data Types & Type Systems
**Context:** SACCO Member Financial Record
Stores member name, ID, monthly contribution, and computes total savings over 6 months.

| File | Language |
|---|---|
| `sacco_records.py` | Python |
| `SaccoRecords.java` | Java |
| `type_analysis.md` | Analysis |

Key analysis :
- Static vs dynamic typing observed when assigning a string to a numeric field
- Justification for static typing in financial systems vs dynamic typing in startup environments

---

### Level 3 — Control Flow & Decision Systems
**Context:** Drought Advisory Logic (Machakos County)

Rainfall advisory using the rules:
- `< 200mm` → *Irrigation Required*
- `≥ 200mm` and `temp > 30°C` → *Monitor Soil*
- Otherwise → *Normal Conditions*

| File | Description |
|---|---|
| `Java/Main.java` | Standard if-else implementation |
| `Java/MainNested.java` | Nested conditions / switch rewrite |
| `Python/advisory.py` | Standard if-else implementation |
| `Python/advisory_nested.py` | Nested conditions rewrite |

---

### Level 4 — Abstraction & Modularity
**Context:** NHIF Claims Processing

OOP design with a `Patient` class and a `calculateClaim(amount)` method that deducts a 10% co-payment. Includes a procedural refactor for maintainability comparison.

| File | Description |
|---|---|
| `JAVA/Patient.java` | OOP — Patient class with claim logic |
| `Python/nhif_oop.py` | OOP — Python equivalent |
| `Python/python-procedural.py` | Procedural refactor for comparison |

---

### Level 5 — Paradigm Comparison
**Context:** Ride-Hailing Pricing Engine (Nairobi)

Fare formula: `Total = 200 + (50 × distance) KES`

| File | Paradigm |
|---|---|
| `fare.cpp` | Procedural (C++) |
| `python-OOP.py` | Object-Oriented (Python) |
| `python-LAMBA.py` | Functional — lambda (Python) |

Analysis: which paradigm scales best when surge pricing is added.

---

### Level 6 — Scope, Memory & Error Handling
**Context:** Patient Record Access Control

`checkAccess(role)` raises an error if role is not `"Doctor"`. Includes a scope experiment demonstrating variable lifetime inside vs outside functions.

| File | Description |
|---|---|
| `Main.java` | Java try-catch access control |
| `python(exceptions).py` | Python exception handling |
| `python(scope).py` | Scope experiment |

---

### Level 7 — Capstone: Mini DSL for Mobile Money Rules
**Context:** Mobile Money Transaction Rules

Parses and interprets commands such as:
```
TRANSFER 5000 FROM A TO B IF BALANCE > 1000
```

| File | Description |
|---|---|
| `main.py` | Parser + interpreter logic in Python |

Reflection covers why Python suits DSL prototyping, why C++ would be harder for rapid iteration, and how AI code assistants can accelerate DSL development in Kenya.

---

##  Languages Used

![Python]
![Java]
![C++]

---

##  How to Run

**Python**
```bash
python "Login Validation.py"
```

**Java**
```bash
javac ECitizenLogin.java
java ECitizenLogin
```

**C++**
```bash
g++ -o login "Login Validation.cpp"
./login
```

---

## Key Concepts Covered

| Level | Concept |
|---|---|
| 1 | Syntax vs semantics, compilation vs interpretation |
| 2 | Static vs dynamic typing, type coercion |
| 3 | if-else, nested conditions, loops, switch |
| 4 | Classes, encapsulation, methods, modularity |
| 5 | Procedural, OOP, and functional paradigms |
| 6 | Scope, variable lifetime, exception handling |
| 7 | DSL design — parsing and interpretation |

---

##  Author

**[Emmanuel Banani Mugisha]**  
Student ID: [677532]  
Course: APT1030-A — Fundamentals of Programming Languages  
[USIU-Africa] | [2026]

---

##  License

This project is submitted for academic purposes only.