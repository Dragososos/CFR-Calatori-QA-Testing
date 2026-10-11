# Manual QA Testing – CFR Călători / Mersul Trenurilor

**Final project** for **Școala Informală de IT** – Manual Quality Assurance course.

This repository contains the complete documentation of a manual testing project performed on the public website of the Romanian national railway company (**CFR Călători** – mersultrenurilor.cfrcalatori.ro).

> **Important**: This was an independent student project done for educational purposes only.  
> I am **not** affiliated with, employed by, or working for CFR Călători.

---

## Project Overview

| Item                    | Details                                      |
|-------------------------|----------------------------------------------|
| **Application tested**  | Mersul Trenurilor / CFR Călători (public website) |
| **Project type**        | Final project – Școala Informală de IT       |
| **Testing Period**      | 21 Oct 2023 – 17 Nov 2023                    |
| **Tester**              | Szabo Dragos-Florin                          |
| **Effort**              | ~35–40 hours                                 |
| **Test Cases Executed** | 24                                           |
| **Pass Rate**           | **91.67%** (22 passed / 2 failed)            |
| **Defects Found**       | 6 (2 Major, 3 Normal, 1 Minor)               |

---

## Website Under Test

- Public web application used for train schedule search and ticket-related information.
- Main areas tested:
  - Search engine (by keyboard + by interactive map)
  - User Registration
  - Login
  - Multi-language support (Romanian / English / French)

---

## Testing Scope

| Feature              | Status          |
|----------------------|-----------------|
| Searching (keyboard) | Fully tested    |
| Searching by map     | Fully tested    |
| Registration         | Fully tested    |
| Login                | Fully tested    |
| Languages            | Fully tested    |

**Test Environment**:
- Windows 11 + iOS 16.7.2
- Browsers: Mozilla Firefox 118, Google Chrome 119, Safari 17.1
- Desktop + limited mobile testing (map functionality)

---

## Testing Approach & Types Used

- Functional Testing
- Exploratory Testing (main source of the discovered bugs)
- Smoke Testing
- Usability Testing
- Compatibility Testing (cross-browser)
- Integration Testing (search engine)
- Positive / Negative / Blank / Big Data testing

---

## Tools Used

| Tool                  | Purpose                     |
|-----------------------|-----------------------------|
| TestLink              | Test case management        |
| Mantis Bug Tracker    | Bug reporting               |
| XMind                 | Mind mapping                |
| Snipping Tool         | Screenshots                 |

---

## Test Results Summary

| Functionality   | Total | Passed | Failed | Defects Linked          |
|-----------------|-------|--------|--------|-------------------------|
| Login           | 2     | 2      | 0      | –                       |
| Registration    | 10    | 8      | 2      | 0054956, 0054954        |
| Search          | 5     | 5      | 0      | 0054957, 0054953, 0054952 |
| Languages       | 7     | 7      | 0      | –                       |
| **Overall**     | **24**| **22** | **2**  | –                       |

**Success Rate**: 91.67%

---

## Defects Found

| ID       | Summary                                                                 | Severity |
|----------|-------------------------------------------------------------------------|----------|
| 0054953  | Searching by map: Chunks of the map do not load                         | **Major**|
| 0054955  | Account: Website does not recognize a valid account's email             | **Major**|
| 0054957  | Searching: Search engine does not recognize "Cluj-Napoca" as valid      | Normal   |
| 0054956  | Account creation: Error after registration if email is very long        | Normal   |
| 0054954  | Account creation: Error if first name field is left empty               | Normal   |
| 0054952  | Searching by map: Map does not load properly                            | Minor    |

All 6 defects were discovered during exploratory testing.

---

## Repository Contents

```
├── README.md
├── LICENSE
├── .gitignore
├── reports/
│   └── Test-Report-CFR-Calatori.docx      ← Full formal Test Report
├── test-data/
│   └── Test-Data-CFR-Calatori.xlsx        ← Complete Test Data Set
└── presentations/
    └── QA-Presentation-CFR-Calatori.pptx  ← Project presentation
```

---

## Conclusions

- 24 test cases were executed → 22 passed, 2 failed (91.67% success rate).
- 6 bugs were identified (2 major, 3 normal, 1 minor).
- Recommendation made at the time: fix the two major bugs before considering the application ready for wider use, then address the normal and minor ones.

---

## Lessons Learned

- Exploratory testing works very well together with usability and compatibility testing.
- Reproducing the same steps many times to confirm a bug can become tiring — good notes and screenshots help a lot.
- Starting the work early leaves more time for deeper exploratory sessions.

---

## Author

**Szabo Dragos-Florin**  
Final project – Școala Informală de IT (Manual QA)

---

## License

This project documentation is released under the **MIT License**.
