# Penn State Alumni Event Performance Analysis & Strategic Forecasting

This project delivers a data-driven framework for understanding, optimizing, and strategically planning future alumni events. By analyzing historical performance from 2022-2025, it provides actionable insights into attendance, financial outcomes (income, expenses, net raised), and operational efficiencies, culminating in a robust forecast for the 2026 event. **The primary objective is to equip stakeholders with critical information to make informed business decisions, improve event profitability, and enhance alumni engagement.**

## Table of Contents

- [Project Overview](#project-overview)
- [Business Objectives & Impact](#business-objectives-&-impact)
- [Data Sources](#data-sources)
- [Analysis Workflow](#analysis-workflow)
- [Key Business Insights from EDA](#key-business-insights-from-eda)
- [2026 Strategic Forecast](#2026-strategic-forecast)
- [Interactive Dashboard for Decision Support](#interactive-dashboard-for-decision-support)
- [Setup and Usage](#setup-and-usage)

## Project Overview

This project is designed to transform raw multi-year alumni event data into strategic intelligence. It focuses on identifying performance trends, understanding financial drivers, and providing forward-looking projections to support **proactive decision-making for future event planning, resource allocation, and fundraising strategies**. The analysis ensures that event organizers can move beyond reactive management to a data-informed approach, maximizing both engagement and financial returns.

## Business Objectives & Impact

The core business objectives addressed by this project include:

*   **Optimized Resource Allocation**: By understanding historical cost efficiencies and attendance trends, resources (budget, staffing, inventory) can be allocated more effectively for future events.
*   **Enhanced Fundraising Strategy**: Detailed analysis of income streams, particularly auction performance, identifies high-leverage opportunities to maximize net funds raised.
*   **Improved Event Profitability**: Insights into revenue per attendee and cost per attendee directly inform pricing strategies, expense control, and overall financial health of events.
*   **Strategic Planning for Growth**: Forecasts for attendance and financial metrics provide a foundational baseline for setting realistic goals, evaluating strategic initiatives, and assessing potential risks for the 2026 event and beyond.
*   **Data-Driven Decision-Making**: Moving away from intuition, this project provides concrete data and projections to justify strategic shifts, allocate budgets, and measure success.

## Data Sources

The project consolidates and cleans data from various Excel files (2022-2025) into structured CSVs, forming a unified view of event performance:

*   `attendance_ticket.csv`: Core attendance figures and ticket sales revenue.
*   `income_expense.csv`: Comprehensive breakdown of all income and expenditure.
*   `beverage_inventory.csv`: Cost and consumption patterns of event beverages, informing procurement.
*   `marketing_channels.csv`: Performance of different marketing efforts, aiding future campaign optimization.
*   `auction_items.csv`: Auction item success rates and revenue generation, crucial for fundraising.
*   `unified_kpi.csv`: Aggregated Key Performance Indicators (KPIs) for holistic year-over-year comparison.

## Analysis Workflow

The project follows a systematic approach to ensure data integrity and actionable insights:

1.  **Data Cleaning & Preprocessing**: Raw data from disparate Excel sources is standardized, validated, and transformed.
2.  **Data Unification**: Cleaned yearly dataframes are concatenated into single, comprehensive datasets.
3.  **KPI Calculation**: Key financial and operational metrics are derived and aggregated (e.g., attendance, total income, net raised, revenue/cost per attendee).
4.  **Exploratory Data Analysis (EDA)**: Visualizations and statistical summaries reveal historical trends, patterns, and anomalies, highlighting areas of success and concern.
5.  **Scenario-Based Forecasting**: Projections for 2026 attendance, revenue per attendee, and cost per attendee are developed under Conservative, Expected, and Optimistic scenarios, providing a range for strategic planning.
6.  **Interactive Dashboard**: A dynamic Plotly dashboard synthesizes historical data and future forecasts, offering an intuitive tool for stakeholders.

## Key Business Insights from EDA

The exploratory analysis uncovered several critical business insights:

*   **Attendance Stability**: While attendance grew significantly up to 2024, the slight dip in 2025 suggests a plateau. *This informs marketing efforts to maintain engagement and explores new avenues for growth rather than relying on past momentum.*
*   **Shifting Profitability Drivers**: Total income peaked in 2023, largely due to strong auction performance, but high expenses offset net gains. In contrast, 2024 and 2025 saw improved *net raised* figures due to tighter expense control, even with lower total income. *This highlights the business value of cost efficiency over raw revenue growth in certain periods.*
*   **Revenue Efficiency Volatility**: Revenue per attendee declined significantly in 2024 despite record attendance, implying that higher attendance doesn't automatically translate to higher per-attendee spending. A partial recovery in 2025 suggests improved monetization strategies. *This underscores the need for continuous optimization of pricing and revenue mix.*
*   **Sustained Cost Efficiency**: Post-2023, cost per attendee substantially reduced and stabilized. *This demonstrates successful operational improvements and allows management to focus more on revenue generation rather than reactive cost cutting.*
*   **Auction Performance: High-Impact, High-Volatility**: Auction revenue was a major income contributor but showed a sharp decline in 2024-2025. *This identifies the auction as a critical, yet volatile, element of the fundraising strategy, requiring focused attention on item sourcing and bidder engagement for future events.*
*   **Negligible Beverage Cost Impact**: Beverage costs remained a minor factor in overall expenses. *This suggests less strategic focus is needed here, freeing up resources for higher-impact areas.*

## 2026 Strategic Forecast

The scenario-based forecast for 2026 provides actionable intelligence for strategic planning:

*   **Attendance Forecast (Expected: ~235 attendees; Range: 223-254)**:
    *   *Decision Support*: Helps determine venue capacity, catering needs, staffing levels, and initial budget allocations. The range allows for robust contingency planning.
*   **Revenue per Attendee Forecast (Expected: ~$49; Range: $44.16-$56.43)**:
    *   *Decision Support*: Informs pricing strategies, marketing efforts for high-value segments, and auction item selection. Improving this metric is identified as a key driver for increased profitability.
*   **Cost per Attendee Forecast (Expected: ~$29-30; Range: $27.72-$32.10)**:
    *   *Decision Support*: Provides a baseline for expense management, supplier negotiations, and identifying potential areas for further cost optimization without compromising event quality.
*   **Projected Net Funds Raised**:
    *   *Decision Support*: The combined forecasts provide clear financial projections under different conditions, enabling stakeholders to set realistic fundraising targets and evaluate the overall financial viability and success of the 2026 event. The significant upside potential in the optimistic scenario, driven by revenue per attendee, highlights strategic investment areas.

**NOTE:**
- The 2026 forecast was developed using a scenario-based approach, combining linear trend extrapolation, recent historical averages, and business judgment.
- Attendance was projected by blending a linear trend from historical data (2022-2025) with recent average attendance, resulting in an expected 235 attendees.
- Revenue per attendee was forecasted by giving more weight to recent performance (2024-2025) to account for shifts in monetization strategies, leading to an expected $49 per attendee.
- Cost per attendee was also based on recent stabilized cost patterns (post-2023) due to improved operational efficiencies, with an expected $29-$$29-$30 per attendee.
- These individual forecasts were then combined across conservative, expected, and optimistic scenarios to project the Net Funds Raised for 2026.


## Interactive Dashboard for Decision Support

A Plotly-based interactive dashboard (`alumni_event_dashboard.html`) visually summarizes the project's findings and forecasts. This tool enables stakeholders to:

*   Quickly grasp historical trends and 2026 projections.
*   Compare different scenarios for attendance, revenue, and costs.
*   Understand the financial implications of various strategic choices at a glance.
*   Facilitate data-driven discussions and consensus building among the event planning committee.

## Setup and Usage

To replicate the analysis and generate the dashboard:

1.  **Environment**: Google Colab (Python 3.x).
2.  **Data**: Place raw Excel files (e.g., `Attendance and Ticket 2022.xlsx`, `Income_Expense_2022.xlsx`, etc.) into `/content/data/raw/` within the Colab environment.
3.  **Dependencies**: `pandas`, `numpy`, `matplotlib`, `plotly` (already handled in notebook).
4.  **Execution**: Run all code cells sequentially. The cleaned datasets will be saved to `data/cleaned/`, and the dashboard HTML will be generated at `data/cleaned/alumni_event_dashboard.html`.

## Interactive Dashboard

Take a look at the event performance overview below, or click the image to explore the full interactive dashboard.
[Tailgate_event_trend_dashboard](Tailgate_event_trend_dashboard.html)

