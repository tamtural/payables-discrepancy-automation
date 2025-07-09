# Payables-Discrepancy-Automation
This project automates the reconciliation of billing and payables data, highlighting mismatches and exporting the results to a structured Excel file. Built for operational efficiency, it’s especially useful when auditing large datasets across multiple sources.

---

##Features
- Uploads billing, payables, and member reference data
- Calculates discrepancies between expected and actual payouts
- Highlights off-balance transactions
- Produces an Excel report with formatting and summary analysis
- Built to run smoothly in **Google Colab** or locally as a `.py` script

---

## Requirements
- Python 3.7+
- `pandas`, `openpyxl`, `xlsxwriter`

To install dependencies:
```bash
pip install pandas openpyxl xlsxwriter
```

---

##Files
| File | Description |
|------|-------------|
| `Payables_Reconciliation.py` | Main Python script with full reconciliation logic |
| `sample_billing.csv` | Sample billing transactions |
| `sample_payables.csv` | Sample payables from the system |
| `sample_members.csv` | Sample member-product reference table |

---

##How to Use (Colab or Local)
1. Run the script
2. Choose report type: `weekly` or `monthly`
3. Upload the 3 required CSVs when prompted:
   - Billing
   - Payables
   - Member reference file
4. Receive a formatted Excel file with:
   - `Billing File`
   - `Off-Balances`
   - `Full Analysis`

---

##Notes
- Thresholds:
  - Weekly: ±$0.20
  - Monthly: ±$1.00
- The logic assumes grouped totals by `Member ID` and `Product ID`
- This is a generalized version of a real-world automation and uses dummy data only

---

##Why This Project?
This automation was built to reduce manual reconciliation time, flag mismatches across disparate files, and generate audit-ready reports with minimal effort. It's especially useful in operations or financial workflows where transaction validation is critical.

---

##Author
Built by [tamtural](https://github.com/tamtural) as part of an automation portfolio project.
LinkedIn: Tamarl Christie

Feel free to reach out with questions!
