# BUG-001: Infinite Skeleton Loader Persists After Hotel Results Load

## Overview

During exploratory testing of a travel booking application's hotel search module, a loading-state issue was observed.

Hotel results were displayed successfully; however, skeleton loading placeholders continued to remain visible even after the hotel data was loaded and rendered.

---

## Defect Information

| Field           | Value              |
| --------------- | ------------------ |
| Bug ID          | BUG-001            |
| Category        | UI / Loading State |
| Severity        | Medium             |
| Priority        | Medium             |
| Reproducibility | 100%               |
| Status          | Reported           |

---

## Investigation Performed

* API Response Validation
* Network Request Analysis
* DOM Validation
* Cross-Browser Testing
* Wait-Time Validation
* Filter Validation
* Business Impact Assessment

---

## Key Findings

### Finding 1

HotelSearch API returned a successful response (HTTP 200).

### Finding 2

Hotel data was successfully rendered on the page.

### Finding 3

DOM validation confirmed hotel elements were present.

### Finding 4

Loading placeholders remained visible even after successful rendering.

### Finding 5

Issue was reproduced across multiple browsers.

---

## Business Impact

### Direct Impact

Users can still search and view hotels successfully.

### Indirect Impact

* Creates confusion regarding page loading status.
* May reduce user confidence.
* Negatively affects user experience.

---

## Skills Demonstrated

* Exploratory Testing
* Browser DevTools
* API Testing
* Network Analysis
* Defect Investigation
* Root Cause Hypothesis
* Professional Bug Reporting

---

## Evidence

See the `/evidence` folder and attached PDF report for screenshots and detailed investigation.

---

## Report

BUG-001_EaseMyTrip_Infinite_Skeleton_Loader.pdf

---

## Conclusion

The investigation confirmed that hotel data was successfully retrieved and rendered. However, loading placeholders remained visible after content rendering, indicating a potential issue in frontend loading-state management. The issue impacts user experience but does not block hotel search functionality.

---

## Disclaimer

This investigation was conducted using publicly accessible functionality during normal application usage. No intrusive, unauthorized, or security-related testing was performed.