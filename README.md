# 🚗 Urban Routes — Web Testing Project · Car Sharing Platform
 
> Software testing project applied to the **Urban Routes** platform, covering layout testing, form validation, booking button logic, and rental workflows.

---

## Objective

Planning, documentation, and execution of testing activities for a car-sharing web application, focusing on functional validation, usability, responsiveness, and cross-browser compatibility.

---
 
## 📋 Overview
 
This repository documents the complete execution of a manual testing cycle on the **Urban Routes** (Car Sharing) web platform, including layout checklists, functional test cases, and Jira-format bug reports.
 
| Item | Detail |
|-------------------------|----------------------------------|
| **Platform** | Urban Routes – Car Sharing Web |
| **Browser** | Google Chrome |
| **Resolution** | 800 × 600 px |
| **Total items tested** | 60+ |
| **Bugs found (FAILED)** | 33 |
| **Approved items** | 20+ |
| **Blocked items** | 5 |

---

## 🧪 Test Scope
 
### Tab 1 — Layout Checklist
 
Visual verification of the interface in its initial state, Personal mode, map, Casual fare, driver's license section, and confirmation pop-up.
 
| ID | Brief Description | Result |
|----|--------------------|-----------|
| L1 | Displays Urban.Routes logo | ✅ PASSED |
| L2 | Displays "PLATFORM" text | [❌ FAILED](https://drive.google.com/file/d/1a7ka2W9It39bT_AbbbmWpKLf49n0Oysn/view?usp=drive_link) |
| L3 | Red (From) and blue (To) button | ✅ PASSED |
| L4 | Phrase "Carshering~$ X Duration: X min" — spelling and formatting error | [❌ FAILED](https://drive.google.com/file/d/1t2M5meKtArEyQvGKbt0n5rCKsFSK0vo5/view?usp=drive_link) |
| L5 | "Book" button layout differs from specification | [❌ FAILED](https://drive.google.com/file/d/1NtrpqTMUAGXKW-dq1t6-lx12_CR2UHXJ/view?usp=drive_link) |
| L6 | Displays blue car in Personal mode | ✅ PASSED |
| L7 | Route not displayed on map | [❌ FAILED](https://drive.google.com/file/d/1H_blCEOjqCVK37a5h__yB8i3LFBydOET/view?usp=drive_link) |
| L8 | Blue cars do not appear on the map after booking | [❌ FAILED](https://drive.google.com/file/d/1vr2hu1oB-3kW35hyKx-eLVQcOmUbRXT9/view?usp=drive_link) |
| L9 | BMW location missing on map (Casual) | [❌ FAILED](https://drive.google.com/file/d/1050flMFKjDrHHBYbWIlKrDyUOd9zB1xM/view?usp=drive_link) |
 L10 | Displays vehicle model in Casual fare | ✅ PASSED |
| L11 | Displays phrase "Business only, nothing extra" | ✅ PASSED |
| L12 | Visual inconsistency in time/wait text (Casual) | [❌ FAILED](https://drive.google.com/file/d/1RgZeYGK47qQw5-OvqGA171kYa4U2FSQ1/view?usp=drive_link) |
| L13 | Illustration missing trim details on wheel/front door (Casual) | [❌ FAILED](https://drive.google.com/file/d/1db51WjGnprbATGYnJe67lxmfPPkMDz_t/view?usp=drive_link) |
| L14 | Accessories text incorrectly displayed in lowercase | [❌ FAILED](https://drive.google.com/file/d/1LjlXc_fvjjYilhNoqCSg7dmsK_eXW_FS/view?usp=drive_link) |
| L15 | Distance/duration info missing near "BOOK" button | [❌ FAILED](https://drive.google.com/file/d/1Z8LzMKZeDxfqF268Jhcb13d81zeFASMd/view?usp=drive_link) |
| L11-CDM | "Add License" button missing ">" symbol | [❌ FAILED](https://drive.google.com/file/d/1v6hq-i0-4EoOX3hyOjTxlypAzsruiKLo/view?usp=drive_link) |
| L12-CDM | Field lacks green highlight/check icon after valid license | [❌ FAILED](https://drive.google.com/file/d/1iH6RJHUzh4omiPOle642xts5GK68XIG1/view?usp=drive_link) |
| L13-POP | Pop-up displays only "The car has been booked" without full details | [❌ FAILED](https://drive.google.com/file/d/1KKtFbjLpBQAIsQn8A7hOHpC9ZA2TdTJs/view?usp=drive_link) |
| L14-POP | Vehicle name missing in confirmation | [❌ FAILED](https://drive.google.com/file/d/1nbOBK_bw3RWm3oh_0fdltduXzs8N9HzH/view?usp=drive_link) |
| L15-POP | Illustration missing trim details in confirmation pop-up | [❌ FAILED](https://drive.google.com/file/d/1WVnLCUSToB4_3gmAvCzg41lhEojcmNwL/view?usp=drive_link) |
| L16-POP | "Cancel" button inactive on confirmation screen | [❌ FAILED](https://drive.google.com/file/d/17uaJ0rGu_XBLxR35oPo8D1HtX0x4ZOeJ/view?usp=drive_link) |
| L17-POP | Cost not displayed in "Cost – $X" format | [❌ FAILED](https://drive.google.com/file/d/196sJ-rD-D_fW5MtXBDKRhCr3w0fdkqpW/view?usp=drive_link) |
| L18 | Cancellation pop-up displays correct message | 🔒 BLOCKED |
| L19 | Ride canceled message displayed correctly | 🔒 BLOCKED |

---

### Tab 2 — Checklist: Payment Method and Add Card
 
Validation of fields and behaviors in the payment window.
 
| ID | Brief Description | Result |
|----|--------------------|-----------|
| P1 | Field displayed empty in initial state | ✅ PASSED |
| P2 | Requires at least 1 card to complete booking | ✅ PASSED |
| P3 | No restriction on number of cards | ✅ PASSED |
| P4 | Last 4 digits of card not displayed after adding | [❌ FAILED](https://drive.google.com/file/d/1DjixQs-s0CcdQGE19o2wzCiFG3Ci2NPW/view?usp=drive_link) |
| P5 | "Cancel" button closes registration window | ✅ PASSED |
| P6 | "X" button closes registration window | ✅ PASSED |
| P7 | Format nnnn nnnn nnnn accepted | ✅ PASSED |
| P8 | Field accepts non-numeric characters | [❌ FAILED](https://drive.google.com/file/d/1-rnKBOl6AKc9rCh81nzUfHzVpWK_zNMS/view?usp=drive_link) |
| P9 | Validation of range 0000–9999 per block does not work | [❌ FAILED](https://drive.google.com/file/d/1CkPsu4YbmCAdzYEcKWZ3W75uaUf08S4B/view?usp=drive_link) |
| P10 | Spaces not inserted automatically when leaving field | [❌ FAILED](https://drive.google.com/file/d/1xHJrMFzVzd_njlV1D9xW-0L-wt7Dj4ye/view?usp=drive_link) |
| P11 | "Add" button inactive with fewer than 12 symbols | ✅ PASSED |
| P12 | Field allows entering more than 12 symbols | [❌ FAILED](https://drive.google.com/file/d/1e4p-ET9CwXTHY4dc-0uu9P6VnlK9xkE5/view?usp=drive_link) |
| P13 | Code format: 2 symbols | ✅ PASSED |
| P14 | Code accepts numbers only | ✅ PASSED |
| P15 | "Code" field allows entering "00" | [❌ FAILED](https://drive.google.com/file/d/1qXvaARv9fqO-blRuBTtZToeCiooTd9XG/view?usp=drive_link) |
| P16–P19 | Values 01, 02, 98, 99 accepted correctly | ✅ PASSED |
| P20 | "Code" field allows entering "100" | [❌ FAILED](https://drive.google.com/file/d/1K-CTt2UD_O4a--4DGHXG3e9xqEbWRdJQ/view?usp=drive_link) |
| P21 | "Add" button active with fewer than 2 code symbols | [❌ FAILED](https://drive.google.com/file/d/1SMIR3AQrhYn4gU4-vXZbxNOjPh__dElq/view?usp=drive_link) |
| P22 | Field accepts characters outside requirements | [❌ FAILED](https://drive.google.com/file/d/1f4ZMgvmx6QXi5joyGAW_kkYCrtUO5Qi9/view?usp=drive_link) |
| P23 | Valid card and code enable "Add" button | ✅ PASSED |
| P24 | "Add" button enabled with invalid card + valid code | [❌ FAILED](https://drive.google.com/file/d/1UGq6BjBMh8Xf26JD-dKnxOSzRi4fs2hb/view?usp=drive_link) |
| P25 | "Add" button enabled with valid card + invalid code | [❌ FAILED](https://drive.google.com/file/d/1Gp3G61uu_ejVT5FN9j77tuh7oK9Q4lit/view?usp=drive_link) |
| P26 | "Add" button enabled with invalid card and invalid code | [❌ FAILED](https://drive.google.com/file/d/1icmYGOz4nk5zr5x5VKg3qc_lQWNHIwX5/view?usp=drive_link) |
| P27 | Without input, button remains disabled | ✅ PASSED |

---

### Tab 3 — Test Cases: "Book" Button Logic
 
| ID | Brief Description | Result |
|----|--------------------|-----------|
| R1 | Booking with all fields correctly completed | ✅ PASSED |
| R2 | "License added" window missing when booking without license | [❌ FAILED](https://drive.google.com/file/d/1tHOhaYP_R17KOUnukZykuRjfdslRQGmE/view?usp=drive_link) |
| R3 | "Card added" window missing when booking without payment | [❌ FAILED](https://drive.google.com/file/d/1wXvOsSVHzI92jTLKceWwL4UpwW4zp4iU/view?usp=drive_link) |
| R4 | "Book" button remains active after deleting addresses | [❌ FAILED](https://drive.google.com/file/d/1rLwqLoA6upigAH4Q-ydLHIstVUz-ISzV/view?usp=drive_link) |
| R5 | All fields empty and addresses deleted | 🔒 BLOCKED |
 
---

### Tab 4 — Test Cases: Booking Feature Logic (Rental)
 
| ID | Brief Description | Result |
|----|--------------------|-----------|
| T1 | Booking with From/To fields completed works correctly | ✅ PASSED |
| T2 | Booking cancellation does not work correctly | [❌ FAILED](https://drive.google.com/file/d/17xNHvyItt4BXYSmSseYaCxOO5eiO2dRn/view?usp=drive_link) |
| T3 | Choosing not to cancel returns to "Car booked" screen | 🔒 BLOCKED |

---

## 🐛 Bug Summary by Severity
 
| Severity | Qty | IDs |
|------------|-----|-----|
| 🔴 Blocker | 7 | L7, P24, P25, P26, R2, R3, R4, T2 |
| 🟠 Major | 18 | L4, L5, L8, L9, L10, L13-POP, L14-POP, L16-POP, P4, P8, P9, P12, P15, P20, P21, P22, R3, L15 |
| 🟡 Minor | 8 | L2, L12, L13, L14, L11-CDM, L12-CDM, L15-POP, L17-POP, P10 |

---

## 📊 Results Distribution

```text
✅ PASSED      ░░░░░░░░░░░░░░░░░░░░░  ~35%
❌ FAILED      ████████████████████   ~54%
🔒 BLOCKED     ░░░░░░                  ~8%
⚠️ N/A         ░░                      ~3%
```

---

## 📁 Bug Reports

Each failed bug has an individual PNG report containing:

- **ID** — identifier from column A of the spreadsheet
- **Summary** — objective description of the issue
- **Environment** — browser, resolution, and component
- **Steps to Reproduce** — step-by-step reproduction instructions
- **Expected Result** — expected behavior
- **Actual Result** — observed behavior
- **Priority** — High / Medium / Low / Critical
- **Severity** — Blocker / Major / Minor

---

## 🛠️ Technologies and Tools

Figma  
Google Chrome DevTools  
Firefox Developer Tools  
Jira  
Git/GitHub

---
 
## 👤 Author

Project developed as part of the **QA (Quality Assurance)** training program — TripleTen.

---

### ✅ Assignment Approved

![Project Approval](https://drive.google.com/file/d/1l--Egh-m6dZV4n6woCF_ijHBirmgA1jp/view?usp=drive_link)

---

## 📄 Licença
 
Este repositório é de uso educacional. Os dados e capturas de tela pertencem ao ambiente de testes do curso.
 

