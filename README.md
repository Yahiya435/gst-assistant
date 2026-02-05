# AI GST Expert Assistant

## Company Profile
- **Type:** Private Limited Company
- **Turnover:** ₹2 Crore (₹20,000,000)
- **GST Regime:** Regular (not composition)
- **Filing:** Monthly GSTR-1 & GSTR-3B

---

## Core Modules

### 1. GST Registration & Setup
```
Inputs Required:
- PAN Number
- Company Name & Address
- CIN Number
- Director Details (DIN, Aadhaar)
- Bank Account (IFSC, Account Number)
- Email & Phone (for OTP)

Output:
- GSTIN Generation
- Registration Certificate (PDF)
- E-way bill portal access
```

### 2. Monthly GSTR-3B (Summary Return)
```
Monthly Obligations:
- Outward Supply Summary
- Input Tax Credit (ITC) Claim
- Tax Liability Calculation
- Cash/Credit Payment

Key Calculations:
- Output Tax = Sales × Tax Rate (5%/12%/18%/28%)
- ITC = Purchases × Tax Rate (eligible portion)
- Net Tax = Output - ITC
```

### 3. Monthly GSTR-1 (Outward Supplies)
```
Details Required:
- B2B Invoices (taxable supplies to registered persons)
- B2C Invoices (taxable supplies to unregistered)
- Export Invoices (with/without payment)
- Credit/Debit Notes
- Advances Received (taxable)

Format:
| Invoice No | Date | GSTIN | Value | Tax Rate | Tax Amount |
```

### 4. Input Tax Credit (ITC) Tracking
```
Eligible ITC:
- Purchases for business use
- Capital goods (depreciable)
- Input services

Ineligible ITC:
- Personal use purchases
- Entertainment expenses > ₹5000
- Motor vehicles (unless for resale)
- GST paid under wrong GSTIN

ITC Verification:
- Match purchase invoices with GSTR-2A
- Flag mismatches
- Suggest recovery actions
```

### 5. E-way Bill Generation
```
Required For:
- Transport > ₹50,000 value
- Inter-state movement
- Intra-state movement (some states)

Inputs:
- Document Type (Invoice/Bill/Challan)
- From/To State
- Vehicle Number (for road)
- HSN Code
- Tax Rate
```

### 6. GST Payment & Liability Tracking
```
Payment Components:
- Output Tax Liability
- Interest (18% p.a. if late)
- Late Fees (₹50/day for GSTR-1, ₹20/day for GSTR-3B)

Payment Modes:
- Cash (electronic cash ledger)
- Credit (ITC from electronic credit ledger)
```

### 7. Compliance Calendar
```
Monthly Deadlines:
- GSTR-1: 11th of next month
- GSTR-3B: 20th of next month
- E-way Bill: Generated before transport

Quarterly (if turnover < ₹5Cr):
- GSTR-1: 31st of next quarter
- GSTR-3B: 22nd/24th of next quarter
```

---

## Sample Calculation (₹2Cr Turnover)

### Scenario: Monthly Sales Breakup
```
Product Sales:
- Product A (12%): ₹8,00,000
- Product B (18%): ₹6,00,000
- Product C (5%): ₹4,00,000
- Exports (0%): ₹2,00,000

Total: ₹20,00,000
```

### Output Tax Calculation
```
| HSN | Rate | Sales | Output Tax |
|-----|------|-------|------------|
| A   | 12%  | ₹8L   | ₹96,000    |
| B   | 18%  | ₹6L   | ₹1,08,000  |
| C   | 5%   | ₹4L   | ₹20,000    |
| Exp | 0%   | ₹2L   | ₹0         |
|-----|------|-------|------------|
| TOTAL|    | ₹20L  | ₹2,24,000  |
```

### ITC Calculation
```
Purchases:
- Raw Materials (12%): ₹4,00,000 → ITC: ₹48,000
- Machinery (18%): ₹2,00,000 → ITC: ₹36,000 (capital, depreciable)
- Services (18%): ₹1,50,000 → ITC: ₹27,000

Total ITC: ₹1,11,000
```

### Net GST Liability
```
Output Tax: ₹2,24,000
Less ITC:    ₹1,11,000
─────────────────────
Net Payable: ₹1,13,000

Cash Payment: ₹1,13,000
(Or use credit ledger)
```

---

## GST Rates Quick Reference

| Category | Rate | Examples |
|----------|------|----------|
| Essential | 0% | Rice, wheat, milk, newspapers |
| Low | 5% | Sugar, spices, tea, coffee |
| Moderate | 12% | Butter, ghee, processed food |
| Standard | 18% | Most goods/services |
| Luxury | 28% | Cars, tobacco, aerated drinks |

---

## Common Mistakes to Avoid

1. **Missing ITC on capital goods** - Can claim up to ₹5L as credit
2. **Wrong HSN codes** - Leads to mismatches
3. **Late filing fees** - ₹50/day GSTR-1 + ₹20/day GSTR-3B
4. **Interest on late payment** - 18% p.a. on delayed tax
5. **Not reconciling GSTR-2A** - ITC claimed but not in supplier's return

---

## Quick Actions Checklist

- [ ] Verify all purchase invoices have correct GSTIN
- [ ] Match ITC in GSTR-2B with purchase register
- [ ] File GSTR-1 by 11th
- [ ] File GSTR-3B by 20th
- [ ] Generate E-way bills before transport
- [ ] Pay tax liability before next month's filing
- [ ] Maintain all invoices for 6 years

---

## Next Steps

1. Enter your actual sales data
2. Upload purchase invoices
3. Run ITC reconciliation
4. Generate filing summary
5. Calculate tax liability
6. File returns

---

**Your AI GST Expert is ready to help!** 🚀

Ask me anything about:
- "Calculate my GST liability"
- "What's my ITC eligibility?"
- "Generate GSTR-1 format"
- "Explain this tax concept"
- "Check my compliance status"
