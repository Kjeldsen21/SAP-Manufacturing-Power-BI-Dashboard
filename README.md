# SAP Manufacturing & Power BI Dashboard
## Description
A group project completed as part of BMI803: Business Processes, featuring an end-to-end BI pipeline built on a SAP ERP manufacturing simulation. Raw transactional data was extracted from SAP focusing on 6 tables, conducted data modelling in Power BI, and used to develop a 3-page executive dashboard.

Led a team of 6 with role focused on data analysis. Project weighed 25% of the final grade. Received an A.


## Project Pipeline
SAP ERP Simulation → Data Extraction → Power BI Data Model → Dashboard Creation


## Data Model

| Table | Type | Key Fields |
|---|---|---|
| **Sales** | Fact | Area, City, Country, Distribution Channel, Cost |
| **Production** | Dimension | Material Description, Month, Round |
| **Purchase Order** | Dimension | Raw Material Type, Quantity |
| **Pricing Conditions** | Dimension | Material Description, Pricing, Round |
| **Supplier Pricing** | Dimension | Raw Material Price, Raw Materials, Round |
| **Company Valuation** | Fact | Company Valuation, Profit |
| **Measures Table** | DAX Calculated | 16 custom measures |

All tables connected via one-to-many relationships using shared `ID` and `Date` keys.


## Dashboard Pages

| Page | Contents |
|---|---|
| **Executive Dashboard** | KPI cards with sparklines, company valuation trend, revenue by SKU, area revenue per round |
| **Sales Channel** | Distribution channel split, regional breakdown, customer order table |
| **Production** | Production output per round, raw material procurement analysis, purchase order breakdown |

![Executive Dashboard](https://github.com/Kjeldsen21/SAP-Manufacturing-Power-BI-Dashboard/blob/main/Power%20BI%20Screenshots/Executive%20Dashboard.png)
![Sales Channel](https://github.com/Kjeldsen21/SAP-Manufacturing-Power-BI-Dashboard/blob/main/Power%20BI%20Screenshots/Sales%20Channel.png)
![Production](https://github.com/Kjeldsen21/SAP-Manufacturing-Power-BI-Dashboard/blob/main/Power%20BI%20Screenshots/Production.png)
![Data Model](https://github.com/Kjeldsen21/SAP-Manufacturing-Power-BI-Dashboard/blob/main/Power%20BI%20Screenshots/PowerBISAPDataModel.png)


## Summary & Findings

The project ran across 4 rounds spanning 3 months of production,
generating €8.16M in total revenue at an 81.6% profit margin. Analysis of the
data produced the following key findings:

**Revenue & Regional Performance**
- West region was the top contributor at €3.09M (37.9%), followed by North
  at €2.80M (34.3%) and South at €2.27M (27.8%).
- Lower Saxony was the highest-performing sub-region at €666K, with Hamburg
  second at €474K.
- South region underperformed by over €820K vs the top region, indicating
  an opportunity for targeted commercial activity through revised marketing or pricing strategies.

**Sales Channel**
- Grocery Chains drove 56.5% of revenue vs 43.5% for Independent Grocers.
- The split is healthy and not over-reliant on a single channel.

**Product Mix**
- Revenue was nearly evenly split between SKUs — Blueberry Muesli (50.1%)
  vs Nut Muesli (49.9%)
- Production yields diverged in Round 4 wherein Nut Muesli dropped to 36.9%
  while Blueberry Muesli continued to grow, suggesting a demand shift.

**Procurement**
- Oats and Wheat each accounted for 35% of ingredient orders, with Nuts and
  Blueberries at approx. 15% each.
- Bulk front-loading on Day 1 (320K packaging units) creates working capital
  exposure if demand patterns shift mid-cycle.

## Key Numbers

| Metric | Value |
|---|---|
| Total Revenue | €8.16M |
| Total Profit | €6.66M |
| COGS | €1.50M |
| Units Sold | 1.42M |
| Top Region | West — €3.09M (37.9%) |
| Top Sub-Region | Lower Saxony — €666K |
| Distribution Channel Split | Grocery Chains: 56.5% vs. Independent Grocers: 43.5% |


## DAX Measures
`Total Revenue` · `Total Profit` · `COGS` · `Production Cost` · `Total Qtty Sold` · `Contribution Margin %` · `Prev. Month Profit` · `Prev. Month Revenue` · `Prev. Month Qtty Sold` · `Profit % Change` · `Revenue % Change` · `Qtty Sold % Change` · `Sparkline (COGS)` · `Sparkline (Profit)` · `Sparkline (Qtty)` · `Sparkline (Revenue)`


## Skills Demonstrated
- SAP ERP navigation and manufacturing simulation
- Relational data modelling (star schema, one-to-many relationships)
- DAX measures and calculated columns 
- Executive dashboard development suitable across multiple stakeholder audiences
- UI/UX Design for intuitive dashboard experience
- Supply chain and procurement analysis
- Team leadership and project coordination


## Tools Used
`SAP ERP` `Microsoft Power BI`
