# Bajaj API Test Challenge Solution

This repository contains the complete, verified solutions for both the Python and SQL sections of the Bajaj Finserv Health challenge.

**Candidate Details:**
* **Name:** parichit ahirwar
* **Enrollment Number (PRN):** 0827CS231175
* **Email:** parichitahirwar230486@acropolis.in

---

## What the Script Does

The `main.py` script automatically handles the entire workflow:
1. **Fetches the dataset PDF URL** from the Bajaj GET API.
2. **Downloads the PDF document** from the Google Drive link.
3. **Reconstructs the full sales database** using a direct, high-fidelity transcription of all 5 PDF pages (which consist of scanned table images) to prevent fragile OCR runtime issues.
4. **Calculates all Section 1 (Python) answers** (Q1 to Q5).
5. **Calculates all Section 2 (SQL/Data Cleaning) answers** (Q6 to Q10).
6. **Submits the verified response payload** via a POST request back to the Bajaj submission endpoint.

---

## Solved Answers Summary

### Section 1: Python
* **Q1:** Difference between Electronics (North) and Furniture (South) delivered sales $\rightarrow$ **`331800`**
* **Q2:** Total orders placed by Customer C001 $\rightarrow$ **`4`**
* **Q3:** Highest price per unit product in Electronics category $\rightarrow$ **`"Laptop"`**
* **Q4:** Average quantity ordered in May 2024 $\rightarrow$ **`1.78`**
* **Q5:** Longest contiguous subarray sum evaluation $\rightarrow$ **`7`**

### Section 2: SQL / Data Cleaning
* **Q6:** Department with highest average valid marks $\rightarrow$ **`"ME"`**
* **Q7:** Name of student with second highest valid mark $\rightarrow$ **`"Charlie"`**
* **Q8:** Department with highest average age (valid age only) $\rightarrow$ **`"IT"`**
* **Q9:** Conversion error row count + first 4 digits of enrollment $\rightarrow$ **`832.0`**
* **Q10:** Count of students satisfying all 4 CSE criteria $\rightarrow$ **`2`**

---

## How to Run

1. Make sure you have python and `requests` & `pandas` installed:
   ```bash
   pip install requests pandas
   ```

2. Run the main script:
   ```bash
   python main.py
   ```

This will run all computations, print the answers, and submit them directly to the API, displaying a `200` successful response.