# 🛒 nopCommerce Manual QA Portfolio

**A complete, end-to-end manual testing project built on the nopCommerce demo e-commerce platform.**  
Prepared by a QA Engineer with 3 years of manual testing experience.

---

## 👤 About This Project

This portfolio demonstrates real-world manual QA skills across the full testing lifecycle — from test planning and test design through execution, defect reporting, and traceability. It was built on the publicly available nopCommerce demo site with no backend access, simulating a real-world black-box testing engagement.

| | |
|---|---|
| **Application Under Test** | https://demo.nopcommerce.com/ |
| **Platform Type** | E-Commerce (ASP.NET Core) |
| **Testing Type** | Manual Functional Testing |
| **Modules Covered** | 21 Frontend Modules |
| **Total Test Cases** | 99 |
| **Total Test Scenarios** | 160 |
| **Defects Found** | 18 raised → 12 confirmed valid |

---

## 📁 Folder Structure

```
nopCommerce_QA_Portfolio/
│
├── 📄 README.md
│
├── 📁 01_Test_Plan/
│   └── nopCommerce_Test_Plan.docx
│
├── 📁 02_Test_Design/
│   ├── Test_Scenarios.xlsx
│   └── Test_Cases.xlsx
│
├── 📁 03_Bug_Evidence/
│   ├── BUG-001_Duplicate_Email/
│   ├── BUG-002_GuestCheckout_DuplicateEmail/
│   ├── BUG-003_RewardPoints_NegativeTotal/
│   ├── BUG-005_ForgotPassword_NoMessage/
│   ├── BUG-008_Cart_ZeroQty_NotHandled/
│   ├── BUG-009_Sort_PriceOrder_Blocked/
│   ├── BUG-011_Coupon_Stacking_Blocked/
│   ├── BUG-012_Newsletter_WrongMessage/
│   ├── BUG-013_Compare_WrongNotification/
│   ├── BUG-015_Review_Keyboard_Accessibility/
│   ├── BUG-016_RewardPoints_EmptyState/
│   └── BUG-018_Forums_Timezone/
│   ⚠️  Add annotated screenshots here per Screenshot_Evidence_Log.xlsx
│
├── 📁 04_Execution_Evidence/
│   ├── Login/
│   ├── Register/
│   ├── AddToCart/
│   ├── Checkout/
│   ├── Search/
│   ├── Wishlist/
│   └── Logout/
│
├── 📁 05_CrossBrowser_Evidence/
│   ├── Chrome/
│   ├── Firefox/
│   ├── Edge/
│   └── Mobile/
│
└── 📁 06_Reports/
    ├── nopcommerce_portfolio_FINAL_v2.xlsx
    └── Screenshot_Evidence_Log.xlsx
```

---

## 📋 Documents at a Glance

| # | Document | File | What It Contains |
|---|---|---|---|
| 1 | **Test Plan** | `01_Test_Plan/nopCommerce_Test_Plan.docx` | 14-section master plan — strategy, scope, risks, schedule, defect management, entry/exit criteria, sign-off |
| 2 | **Test Scenarios** | `02_Test_Design/Test_Scenarios.xlsx` | 160 high-level scenarios (the *"what to test"*) across 21 modules — with priority and test type |
| 3 | **Test Cases** | `02_Test_Design/Test_Cases.xlsx` | 99 detailed test cases — Test Case ID, Scenario, Title, Pre-requisites, Steps, Test Data, Expected Result |
| 4 | **Dashboard** | `06_Reports/...FINAL_v2.xlsx → Dashboard` | One-page KPI summary — modules, pass rate, defect stats, go/no-go |
| 5 | **Test Execution Report** | `06_Reports/...FINAL_v2.xlsx → Test Execution Report` | Module-wise results, daily log, defect severity breakdown, recommendation |
| 6 | **Bug Report** | `06_Reports/...FINAL_v2.xlsx → Bug Report` | 18 defects — full steps to reproduce, expected vs actual, severity, status, re-test comments |
| 7 | **RTM** | `06_Reports/...FINAL_v2.xlsx → RTM` | 99 requirements traced to 99 test cases with execution status and defect references |
| 8 | **Screenshot Log** | `06_Reports/Screenshot_Evidence_Log.xlsx` | 39 screenshots to capture — filenames, folder paths, annotation tips |

---

## 🌐 Modules Tested

| # | Module | Scenarios | Test Cases | Priority |
|---|---|---|---|---|
| 1 | Register | 12 | 6 | 🔴 Critical |
| 2 | Login | 11 | 5 | 🔴 Critical |
| 3 | Logout | 5 | 2 | 🔴 Critical |
| 4 | Forgot Password | 5 | 3 | 🟠 High |
| 5 | Search | 10 | 5 | 🟠 High |
| 6 | Wishlist | 9 | 6 | 🟠 High |
| 7 | Add to Cart | 13 | 8 | 🔴 Critical |
| 8 | Product Catalog | 12 | 8 | 🟠 High |
| 9 | Product Details | 9 | 6 | 🟠 High |
| 10 | Checkout | 11 | 7 | 🔴 Critical |
| 11 | My Account | 9 | 6 | 🟠 High |
| 12 | Order History | 5 | 4 | 🟠 High |
| 13 | Compare Products | 5 | 4 | 🟡 Medium |
| 14 | Newsletter | 5 | 4 | 🟡 Medium |
| 15 | Contact Us | 5 | 3 | 🟡 Medium |
| 16 | Gift Cards | 5 | 3 | 🟠 High |
| 17 | Discount & Coupons | 5 | 3 | 🟠 High |
| 18 | Reward Points | 5 | 3 | 🟡 Medium |
| 19 | Product Reviews | 7 | 4 | 🟡 Medium |
| 20 | Blog | 5 | 4 | 🟢 Low |
| 21 | Forums | 7 | 5 | 🟢 Low |
| | **TOTAL** | **160** | **99** | |

---

## 📊 Execution Results (Final v2.0)

| Metric | Value |
|---|---|
| Total Test Cases Planned | 99 |
| Total Test Cases Executed | 99 (100%) |
| Passed | 87 |
| Failed | 9 |
| Blocked | 3 |
| **Pass Rate** | **88%** |

> **Blocked** means the test case could not be executed due to demo environment limitations (no reward points balance, no coupon codes, insufficient products for pagination). The test cases are valid — only the environment is limiting.

---

## 🐛 Defect Summary

### Valid Confirmed Bugs (12)

| Bug ID | Module | Severity | Title | Status |
|---|---|---|---|---|
| BUG-001 | Register | 🔴 SEV 2 — Critical | Duplicate email registration allowed with no error | Open |
| BUG-002 | Checkout | 🔴 SEV 2 — Critical | Guest checkout with existing email — no warning shown | Open |
| BUG-003 | Reward Points | 🔴 SEV 2 — Critical | Reward points can reduce order total below zero | Open *(cannot reproduce in demo — no reward points balance available)* |
| BUG-005 | Forgot Password | 🟠 SEV 3 — Major | Password recovery shows no success/failure message | ✅ Fixed |
| BUG-008 | Add to Cart | 🟠 SEV 3 — Major | Qty update to 0 left item in cart at $0.00 | ✅ Fixed |
| BUG-009 | Product Catalog | 🟠 SEV 3 — Major | Sort by price breaks across pagination pages | Open *(cannot reproduce — all products fit one page in demo)* |
| BUG-011 | Discount & Coupons | 🟠 SEV 3 — Major | Same coupon applied twice — discount stacks | Open *(cannot reproduce — no coupon codes in demo)* |
| BUG-012 | Newsletter | 🟡 SEV 4 — Minor | Already-subscribed email shows wrong success message | ✅ Fixed |
| BUG-013 | Compare Products | 🟡 SEV 4 — Minor | Second click on 'Add to compare' shows wrong notification | Deferred |
| BUG-015 | Product Reviews | 🟡 SEV 4 — Minor | Star rating not keyboard accessible | ✅ Fixed |
| BUG-016 | Reward Points | 🟡 SEV 4 — Minor | Reward points page blank with no empty-state message | Deferred |
| BUG-018 | Forums | 🟢 SEV 5 — Trivial | Forum timestamps show UTC instead of local timezone | Deferred |

### Invalid / Won't Fix (6)

> These were raised during initial testing but confirmed as working correctly on re-test.

| Bug ID | Module | Why Closed |
|---|---|---|
| BUG-004 | Add to Cart | Re-tested — attribute validation IS working correctly |
| BUG-006 | Search | Re-tested — special characters handled, 'no results' shown |
| BUG-007 | Checkout | Re-tested — back button correctly retains billing address |
| BUG-010 | Gift Cards | Re-tested — invalid gift card code shows error correctly |
| BUG-014 | Wishlist | Re-tested — product correctly added after login redirect |
| BUG-017 | Blog | Re-tested — browser tab title correctly shows 'Blog' |

> **Note on Blocked vs Bug Status:** "Blocked" is a *test execution status*, not a bug status. BUG-003, BUG-009, and BUG-011 remain **Open** in the bug report with notes explaining the demo environment limitation. The corresponding test cases (TC_RWD_002, TC_CAT_002, TC_DSC_001) are marked **Blocked** in the Test Execution Report and RTM.

---

## 🛠️ Tools Used

| Tool | Purpose |
|---|---|
| Google Chrome 124 | Primary execution browser |
| Mozilla Firefox 125 | Cross-browser testing |
| Microsoft Edge 124 | Cross-browser testing |
| Chrome DevTools (F12) | Console error capture, network tab, mobile emulation |
| Microsoft Excel | Test cases, bug report, RTM, execution report |
| Microsoft Word | Test plan |
| Snipping Tool / Greenshot | Screenshot capture and annotation |
| nopCommerce Demo Site | Application under test |

---

## ⚠️ Known Environment Constraints

| Constraint | Impact |
|---|---|
| Site resets every hour | Test data does not persist — accounts and orders are cleared hourly |
| No email inbox access | Password recovery and newsletter email flows cannot be fully verified |
| No payment gateway | Checkout limited to Check/Money Order — no card or PayPal testing |
| Shared public demo | Other users may modify data concurrently — test data pollution possible |
| No backend access | Black-box testing only — no DB or admin panel validation |
| Limited product data | Some scenarios (sort across pages, reward points, coupons) blocked due to insufficient demo data |

---

## 📸 Screenshots

All bug evidence and execution screenshots are organised under `03_Bug_Evidence/` and `04_Execution_Evidence/`.

Every screenshot should have:
- ✅ URL bar visible in the capture
- ✅ Annotated with red arrows or callout boxes pointing to the issue
- ✅ Named exactly as listed in `Screenshot_Evidence_Log.xlsx`
- ✅ Stored in the correct subfolder

---

## 💼 How to Present This in Interviews

**Opening line when asked about a project:**
> *"I built a complete manual QA portfolio on the nopCommerce demo e-commerce site. I wrote a full test plan, designed 160 test scenarios and 99 test cases across 21 modules, executed all of them, found and reported 18 defects — 12 of which were confirmed valid — and produced a full execution report and RTM. Everything is documented and traceable."*

**Best documents to open first:**

1. **Dashboard tab** — 30-second overview of the entire project
2. **Bug Report → BUG-001 or BUG-002** — show a critical bug with clear reproduction steps
3. **Test Cases** — show your test case writing style
4. **RTM** — when asked *"how do you ensure full requirement coverage?"*
5. **Test Plan** — when asked *"do you understand the QA process end to end?"*

**Common interview questions this project answers:**

| Question | Where to point |
|---|---|
| "Walk me through your test plan" | `01_Test_Plan/nopCommerce_Test_Plan.docx` |
| "How do you write a bug report?" | `Bug Report` sheet → any SEV 2 bug |
| "What is severity vs priority?" | Bug Report columns + Test Plan Section 8 |
| "How do you ensure test coverage?" | `RTM` sheet — 100% requirement traceability |
| "Have you done exploratory testing?" | Test Plan Section 2.1.4 |
| "What types of testing have you done?" | Functional, regression, exploratory, cross-browser, UI/UX |
| "What do you do when you can't reproduce a bug?" | BUG-003/009/011 — open with environment note, TC marked Blocked |
| "What if a bug turns out to be not a bug?" | BUG-004/006/007/010/014/017 — Won't Fix with re-test evidence |

---

## 📝 Document Version History

| Version | Date | Changes |
|---|---|---|
| v1.0 | 15-May-2026 | Initial release — all documents created |
| v2.0 | 16-May-2026 | Bug report updated per re-test review — 6 bugs closed as Invalid, 3 corrected to Open with environment notes, RTM and execution report recalculated |

---

*Prepared by: QA Engineer | 3 Years Manual Testing Experience*  
*Portfolio Project: nopCommerce Demo — https://demo.nopcommerce.com/*
