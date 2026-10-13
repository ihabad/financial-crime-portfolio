# Ihab Diab — AML / KYC & Financial Crime Practice Portfolio

**Entry-level AML/KYC · Transaction Monitoring · Fraud Operations**

This portfolio demonstrates structured analytical practice with **entirely synthetic customer and transaction records**. These are **independent simulated case studies**, not professional bank investigations, actual suspicious activity reports, or employer work. The workbook and sample narratives are provided as reproducible learning artifacts, not evidence of regulatory competence.

## Featured projects

| Project | What it demonstrates | Files |
|---|---|---|
| **01 — Transaction Monitoring (TM-01)** | Comparing cash activity to a fictional customer profile; identifying anomalies without equating them to wrongdoing | [Case report](reports/01_Transaction_Monitoring_Case_Study.pdf) · [Excel workbook](workbooks/AML_Transaction_Monitoring_Practice.xlsx) |
| **02 — Business KYC / CDD (KYC-01)** | Reviewing ownership disclosures, identifying information gaps, recommending follow-up | [Case report](reports/02_KYC_CDD_Case_Study.pdf) |
| **03 — Fraud / Account Takeover (FRD-01)** | Reconstructing an event timeline and documenting an escalation rationale | [Case report](reports/03_Account_Takeover_Case_Study.pdf) |

## Transaction-monitoring practice workbook

The Excel workbook contains **120 synthetic transactions and 8 invented customer profiles**. It includes linked VLOOKUP formulas, practice-only review flags, and a sample case log. Open it in desktop Excel to recalculate formulas; use table filters to isolate case activity and sort dates or amounts. The underlying files are also provided as [transactions.csv](data/transactions.csv) and [customers.csv](data/customers.csv).

**Reproduce TM-01:** filter Customer ID to `C001`, inspect Aug 12–15, total the four specially identified cash deposits ($37,700), compare with the *fictional* customer profile, and read the decision rationale.

**Critical compliance note:** The workbook flags are **illustrative review heuristics only**, not SAR/CTR thresholds or assertions of structuring. Activity must be assessed in context. No real customer information is used.

## Skills practiced or illustrated

- Transaction review and pattern comparison with expected customer activity
- Excel filtering, sorting and customer-profile lookups (VLOOKUP)
- Documenting observations, missing information and escalation recommendations
- Customer due diligence questions and ownership review
- Fraud event-timeline reconstruction

## Repository map

```text
README.md
data/
  customers.csv
  transactions.csv
workbooks/
  AML_Transaction_Monitoring_Practice.xlsx
reports/
  01_Transaction_Monitoring_Case_Study.pdf
  02_KYC_CDD_Case_Study.pdf
  03_Account_Takeover_Case_Study.pdf
templates/
  Case_Review_Checklist.md
```

## About

**Ihab Diab** — aspiring entry-level AML/KYC / Financial Crime Analyst. Background in customer account operations, quality control, and information systems.

> Portfolio constructed with AI-assisted sample data and draft reports for training. Before describing any case as independently completed, reproduce the analysis, verify the findings, revise the narrative yourself, and be prepared to discuss the work in an interview.

## Extended practical tutorials: Excel and KYB / CDD / EDD

- [Excel VLOOKUP, filtering and PivotTable walkthrough](guides/Excel_VLOOKUP_PivotTable_Guide.md) explains exact-match customer risk lookups, transaction filtering, and how to create an actual Excel PivotTable. The workbook now has a `VLOOKUP Walkthrough` sheet and a `Pivot Summary Example` sheet (precomputed aggregate, **not** an embedded native PivotTable).
- [Know Your Business (KYB), CDD and EDD walkthrough](guides/KYB_CDD_EDD_Guide.md) extends the business investigation to legal-entity verification, ownership/control, information gaps, risk indicators, and circumstances that could warrant enhanced due diligence.
- [KYB, CDD and EDD case-study report](reports/04_KYB_CDD_EDD_Case_Study.pdf) is an additional fictional learning artifact; not a real onboarding file or sanctions screen.

These additions are educational demonstrations and must be independently practiced and validated before representing them as personally completed casework.
