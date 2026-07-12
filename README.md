# Three-Statement Financial Model & Scenario Analysis: Blu Containers

An advanced, dynamic 3-statement financial forecasting model built to analyze the debt sustainability, liquidity constraints, and operational scaling of **Blu Containers Company** over a 5-year projection horizon (2023–2027). 

This model features fully integrated financial statements, automated credit facilities, and a macro-driven scenario engine designed for strategic decision-making and credit analysis.

---

## Project Architecture
### 1. Assumptions & Scenario Controls
This section establishes the operational core and macroeconomic drivers of the model. It features a centralized scenario switch that dynamically alternates variables across three cases: **Base Case** (Research Forecast), **Best Case** (+4% Pricing / High Growth), and **Worst Case** (-4% Pricing / High Inflation). 

* Volume Constraints:** Sales volume growth is modeled at 5.0% for 2023 and 4.0% thereafter. Crucially, the model incorporates an absolute production capacity wall at **420,000 units/year**, which forces unconstrained growth to cap out and hit 100% capacity utilization by 2027 under the Base Case.
* Cost Structures:** Variable inputs (Raw Materials at $226/unit and Utilities at $66.2/unit) and fixed overheads ($69.0M total in 2023) scale annually based on scenario-specific inflation rates.

![Scenario Assumptions Control](images/votre_capture_des_hypotheses.png)


### 2. Income Statement Analysis
The Income Statement tracks the top-line performance and structural profitability of Blu Containers. It highlights how vulnerable the company's margins are to pricing cycles, even when sales volumes are rising.

* **The 2024 Margin Squeeze:** Under the Base Case, a sharp cyclical dip in gross sales price to **$725/unit** (down from $800 in 2023) drives a revenue contraction to $233.6M. Consequently, EBITDA collapses by 36.2% down to **$47.1M**, compressing EBITDA margins from 29.3% to a low of **20.2%**.
* **Profitability Recovery:** Performance peaks in 2025 when pricing rebounds to $825/unit, lifting EBITDA to **$86.5M** (30.7% margin) before capacity constraints flatten the upside in 2027.

![EBITDA Scenario Comparison](images/ebitda_scenarios.png)


### 3. Balance Sheet & Capital Structure
The Balance Sheet demonstrates full structural integrity, with an integrated macro control check ensuring assets perfectly equal liabilities and equity (`Check = 0.000`) across all projection years and scenario toggles.

* **Capital Structure Evolution:** By isolating permanent funding sources (Term Debt, Revolver, and Equity), the chart below highlights the firm's organic deleveraging profile in the Base Case. The annual $25.0M mandatory amortization steadily reduces the Senior Debt wall, while retained earnings steadily expand the equity base.
* **Tax Timing Differences:** Rather than applying a flat tax rate, the model accounts for a permanent **$5.0M annual structural reduction** from accounting EBT to government taxable EBT, accurately tracking the accumulation of Deferred Income Tax Liabilities.

![Capital Structure Base Case](images/capital_structure.png)


### 4. Net Income Performance
The Net Income highlights the final cash return available for equity holders after adjusting for interest and taxes across all economic cycles.

* **Scenario Divergence:** The chart illustrates the massive impact of operating leverage. In the Worst Case, persistent inflation and a 14% margin drop crush Net Income to $5.0M by 2027, whereas the Best Case captures the full upside of higher pricing with no added interest burdens.

![Net Income Scenario Comparison](images/net_income_scenarios.png)


### 5. Debt & Credit Liquidity Schedule
This schedule represents the most sophisticated financial engineering element of the model, mapping out capital structure sustainability and liquidity runway.

* **Mandatory Amortization:** The company is burdened by a fixed, mandatory Senior Secured Term Debt repayment of **$25.0M every single year**, steadily reducing the term loan balance from $200M to $75M over the horizon.
* **The Revolver Mechanism:** To handle the 2024 cash crunch caused by lower EBITDA and fixed debt payments, the model deploys an automated **Bank Revolving Credit Facility (6.0% interest)**. The Revolver peaks at a **$7.7M drawdown in 2024** to fund the cash shortfall, before an automated *cash sweep* uses 2025's excess cash flows to pay the facility back down to $1.2M.

![Revolver Credit Utilization](images/revolver_scenarios.png)


### 6. Scenario Analysis Insights
While the **Base Case** highlights a temporary $7.7M liquidity crunch in 2024, the model proves resilient across other environments:
* **Best Case (+4% Pricing):** Stronger pricing eliminates the need for any major Revolver drawdown, allowing the company to build a substantial cash buffer by 2027.
* **Worst Case (-4% Pricing & High Inflation):** Severe margin compression occurs. Profitability drops, forcing a continuous reliance on the Revolving Credit Facility to sustain the mandatory $25M annual debt service.

*To explore these outcomes dynamically, users can simply open the file and toggle the **Scenario Switch** on the model sheet.*
