# PAN Number Validation using PySpark

This project performs data cleaning and validation of Indian PAN (Permanent Account Number) values using PySpark on Databricks.

The goal is to identify **Valid**, **Invalid**, and **Missing** PAN numbers based on defined format and business rules.

---

## ✅ What the Project Does

- Cleans PAN numbers (trim spaces, uppercase)
- Handles missing or blank PAN values
- Removes duplicate PAN entries
- Validates PAN using:
  - Regex pattern (AAAAA9999A)
  - No repeated adjacent alphabets or digits
  - No alphabet or digit sequence (e.g., ABCDE, 1234)
- Classifies each PAN as:
  - **Valid PAN**
  - **Invalid PAN**
  - **Missing PAN**
- Generates a summary report

---

## ✅ PAN Validation Rules

A PAN is valid only if:

- Total length = **10 characters**
- First 5 characters: **A–Z**
- Next 4 characters: **0–9**
- Last character: **A–Z**
- No adjacent repeated alphabets (e.g., AABCD… ❌)
- No adjacent repeated digits (e.g., 1123 ❌)
- No sequence in alphabets (ABCDE, BCDEF ❌)
- No sequence in digits (1234, 2345 ❌)

Example of valid PAN: **AHGVE1276F**

---

## ✅ Summary Report Contains

- Total records processed  
- Total valid PANs  
- Total invalid PANs  
- Total missing PANs  

---

## ✅ Technologies Used

- PySpark  
- Databricks  
- Python 3  

---

## ✅ How to Run

1. Upload dataset into Databricks Workspace Files  
2. Import the notebook (`PAN_Validation_PySpark.ipynb`)  
3. Run the notebook end-to-end  
4. Check the results and summary output  

---

## ✅ Project Files

- `notebooks/PAN_Validation_PySpark.ipynb`
- `data/PAN_Number_Validation_Dataset.xlsx`
- Summary report output (CSV/Delta)

---

## ✅ Author
**Yuva Kumar**

