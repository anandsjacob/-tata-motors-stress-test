
# Business Stress Testing & Survival Simulator: Tata Motors

A forward-looking financial scenario model built on Tata Motors' consolidated financials — moving beyond a conventional descriptive dashboard into the kind of stress-testing typically associated with FP&A (Financial Planning & Analysis) or business analyst work.

---

## Project Overview

This project moves beyond a conventional descriptive dashboard into financial scenario modeling. Instead of asking "what happened," it asks a forward-looking business question:

**"How much financial stress can Tata Motors withstand before its profitability or cash flow becomes seriously compromised?"**

---

## Data Source

Three years of consolidated financial statements (FY2022-23, FY2023-24, FY2024-25) were extracted directly from Tata Motors' Integrated Annual Reports — Profit & Loss, Balance Sheet, Cash Flow Statement, and segment-level reporting (Commercial Vehicles, Passenger Vehicles/EV, and Jaguar Land Rover).

---

## Methodology

**1. Baseline construction**
Built a clean historical financial base (revenue, cost structure, EBITDA, debt, and free cash flow) from the raw filings, including a methodological correction to properly account for Tata Motors' significant R&D capitalization practices, ensuring EBITDA margins reflected industry-realistic figures (~12-13%) rather than an understated run-rate.

**2. Segment-level modeling**
Rather than treating "Tata Motors" as a single revenue line, the model separates CV, PV/EV, and JLR, since each carries a materially different risk profile — JLR alone represents ~70% of consolidated revenue and the majority of segment profit.

**3. Driver-based scenario engine**
Designed four forward-looking scenarios (Base, Optimistic, Stress, Extreme Stress) across nine key business drivers: volume growth by segment, pricing, material cost ratio, wage/opex inflation, R&D capitalization rate, interest rates, and capex intensity — built to reflect realistic operating leverage (i.e., fixed costs remaining "sticky" even as revenue contracts).

**4. Output metrics**
Each scenario produces a full projected P&L and cash flow: Revenue, EBITDA, EBIT, PAT, Net Margin, Interest Coverage Ratio, Free Cash Flow, and Net Debt/EBITDA — with an automated rules-based verdict (Comfortable / Manageable / Stressed / Critical) based on solvency thresholds.

**5. Tooling**
Built first as a fully formula-driven Excel model (Historicals → Assumptions → Scenario Model → Dashboard), then rebuilt as an interactive Power BI report with a live scenario selector, DAX-driven measures, and a color-coded Interest Coverage gauge — allowing a user to toggle between scenarios and see the financial impact update in real time.

---

## Key Finding

The model identifies JLR-specific risk (regulatory shifts, tariffs, luxury demand softness) as Tata Motors' single largest financial vulnerability — a more material threat to consolidated profitability than domestic CV/PV demand fluctuations, since JLR's scale means even moderate stress there disproportionately erodes group-level EBIT and interest coverage.

---

## Why This Stands Out

Most portfolio projects report historical performance. This one uses the same data to answer a decision-oriented question a CFO or board would actually ask, delivered as a live, interactive tool rather than a static report — demonstrating financial modeling literacy alongside standard data analytics tooling (Excel, Power BI, DAX).

---

## Repository Structure
├── excel/
│ └── Tata_Motors_Stress_Test_Model.xlsx # Historicals, Assumptions, Scenario Model, Dashboard
├── powerbi/
│ └── Tata_Motors_Stress_Test.pbix # Interactive scenario selector + DAX measures
└── README.md

---

## Skills Demonstrated

`Financial statement analysis` · `Scenario modeling` · `FP&A methodology` · `Excel (driver-based modeling, formula-driven forecasting)` · `Power BI (DAX, dynamic scenario selectors, gauge visuals)` · `Segment-level risk analysis` · `Solvency ratio analysis (Interest Coverage, Net Debt/EBITDA)`

---

## Notes

This project was built entirely from publicly available Integrated Annual Report filings. All figures and scenarios are presented for analytical and educational purposes and do not constitute financial advice or an official Tata Motors risk assessment.
