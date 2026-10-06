# Cross-Browser Compatibility Testing: E-Commerce Web Application

**Internship:** Codecraft Infotech, Quality Assurance
**Task:** 02, Conduct Compatibility Testing for a Basic Web Page
**Tester:** Shabana
**Test Date:** 5 October 2026
**Application Under Test:** Sauce Demo (https://www.saucedemo.com), a public e-commerce demo site

---

## 1. Objective

Verify that the e-commerce demo application renders and behaves consistently across major browsers and device sizes, and document any layout issues, broken links or functional discrepancies, with recommended fixes.

## 2. Scope

**Flows tested (8):**
1. Login
2. Inventory (product listing and sorting)
3. Product details
4. Cart (add and remove items)
5. Checkout: customer information
6. Checkout: order overview
7. Checkout: order complete
8. Navigation menu (All Items, About, Reset App State, Logout)

**Test user:** `standard_user`

## 3. Test Environment

| Browser | Version | Platform |
|---|---|---|
| Google Chrome | 141.0 | Windows |
| Mozilla Firefox | 143.0 | Windows |
| Microsoft Edge | 141.0 | Windows |
| Apple Safari |  18.6 | iOS (iPhone 12, real device) | 

**Responsive widths:** Desktop (full screen), 768 px (tablet), 375 px (mobile), tested using responsive emulation

## 4. Test Checks

For every flow and browser:
- Page loads completely, with no missing images or fonts
- Layout is intact, with no overlapping elements or horizontal scrolling
- Navigation links and menu work correctly; no broken links found (menu, About, cart and product links verified)
- Buttons and forms (sort, add to cart, remove, checkout form) function as expected
- Price calculations are accurate (item total + tax = total)
- Responsive layout adapts at 768 px and 375 px

## 5. Compatibility Matrix

| Flow | Chrome | Firefox | Edge | Safari |
|---|---|---|---|---|
| Login | Pass | Pass | Pass | Pass |
| Inventory and sorting | Pass | Pass | Pass | Pass |
| Product details | Pass | Pass | Pass | Pass |
| Cart | Pass | Pass | Pass | Pass |
| Checkout: information | Pass | Pass | Pass | Pass |
| Checkout: overview | Pass | Pass | Pass | Pass |
| Checkout: complete | Pass | Pass | Pass | Pass |
| Navigation menu | Pass | Pass | Pass | Pass |

**Responsive check (768 px and 375 px):** Pass

## 6. Defect Log

| ID | Browser / Device | Page | Steps to Reproduce | Expected | Actual | Severity | Screenshot |
|---|---|---|---|---|---|---|---|
| | | | | | | | |

**No functional or layout defects were identified** for the `standard_user` flows across the tested browsers and device widths.

## 7. Observations and Recommendations

- The application behaves consistently across all four browsers; no browser-specific fixes are required.
- Price calculations are accurate on both the overview and confirmation pages ($29.99 + $2.40 tax = $32.39).
- **Recommendation:** run this suite on each release as a regression check.
- **Recommendation:** extend coverage to additional browser versions and real devices.
- **Recommendation:** add automated cross-browser tests (for example Selenium or Playwright) to cover these flows.

## 8. Summary

| Metric | Result |
|---|---|
| Flows tested | 8 |
| Browsers tested | 4 |
| Defects found | 0 |
| Pass rate | 100% |

**Conclusion:** The application is compatible with Chrome, Firefox, Edge and Safari, and its layout is responsive across desktop, tablet and mobile widths.

## 9. Evidence

Screenshots are in the repository root, named by browser and page (for example chrome_inventory.png).

