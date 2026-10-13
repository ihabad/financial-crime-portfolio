# Excel analysis walkthrough — VLOOKUP, filtering, PivotTables

**Training exercise only.** All names and transactions in this repository are synthetic. The included `Pivot Summary Example` sheet is a reproducible aggregate, **not a native PivotTable object**; create your own PivotTable using the instructions below.

## 1. VLOOKUP: connect transactions to a customer profile

1. Open `workbooks/AML_Transaction_Monitoring_Practice.xlsx`.
2. In `Customers`, note: column A = `Customer_ID`, D = `Risk_Rating`, F = `Expected_Monthly_Activity_USD`.
3. Open `VLOOKUP Walkthrough`. Cell D2 uses:

```excel
=VLOOKUP(A2,Customers!$A$2:$F$9,4,FALSE)
```

- `A2` is the exact customer ID.
- `Customers!$A$2:$F$9` is the lookup range; `$` fixes it while copying.
- `4` returns column 4, Risk_Rating.
- `FALSE` enforces an exact ID match.

4. To return the expected monthly activity instead, use:

```excel
=VLOOKUP(A2,Customers!$A$2:$F$9,6,FALSE)
```

5. Change the input customer ID temporarily and verify the result, then restore it. Unknown IDs produce `#N/A`, which should be investigated rather than ignored.

## 2. Filter and inspect a pattern

1. On `Transactions`, open the filter dropdown for `Customer_ID` and select `C001`.
2. Sort by `Date` ascending; inspect August 12–15, 2026.
3. Compare the relevant cash deposits with the fictional customer profile. Four case-specific deposits total **$37,700**. This is an observation, **not proof of structuring, wrongdoing, or a regulatory reporting requirement**.
4. Document customer context, observed pattern, missing information, and a proportionate review recommendation.

## 3. Build a genuine PivotTable in desktop Excel

1. Click anywhere in the `Transactions` dataset, then choose **Insert → PivotTable → New Worksheet**.
2. Drag `Customer_ID` to **Rows** and `Type` to **Columns**.
3. Drag `Transaction_ID` to **Values**. Set it to **Count**.
4. Drag `Amount_USD` to **Values** and set it to **Sum**; format as currency.
5. Filter `Customer_ID` to `C001` to compare transaction counts and total amounts by type.
6. Use the workbook's `Pivot Summary Example` sheet as a check on customer/type totals. This sheet itself is **not** a native PivotTable.

## 4. Questions to answer independently

- Which transactions deviate from the fictional customer's expected pattern, and why?
- What benign explanations could exist?
- What information would you request before recommending escalation?
- How would a false-positive review differ from an unresolved risk alert?

## Disclosure

AI-assisted educational practice material. It is not a real bank investigation, professional casework, or an actual SAR/STR filing. A learner should reproduce the formulas and analysis and write their own conclusions before claiming personal proficiency.
