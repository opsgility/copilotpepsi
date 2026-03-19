---
lab:
  title: 'Exercise 3: Excel — Analyze Data & Visualize Insights'
  description: 'Use Copilot in Excel to analyze sales and operations data, create charts, generate formula columns, and uncover trends.'
  duration: 45 minutes
  level: 100
  islab: true
  primarytopics:
    - Microsoft 365 Copilot
    - Excel
---

# Exercise 3: Excel — Analyze Data & Visualize Insights (45 min)
---

Copilot in Excel helps you turn raw data into actionable insights through natural language. Ask questions about your data, generate charts, create formula columns, and uncover patterns — all without writing formulas yourself.

**Before you start:**
- Data must be formatted as an **Excel Table** (select data range, then **Insert > Table**)
- **AutoSave** must be turned on (file must be saved to OneDrive)
- Select **Copilot** in the Excel ribbon to open the Copilot pane

>**Note:** Copilot in Excel has transitioned from **App Skills** to **Agent Mode**. If the Copilot menu shows **Chat** and **App Skills**, select App Skills. If your version only shows Copilot Chat, select **Tools > Agent Mode** to work directly in the workbook.

---

### Task 1: Analyze sales performance data (20 min)

1. Open **GJ_Q4_Sales_Performance.xlsx** from your OneDrive (**GJ-Workshop** folder). It will open in **Excel for the web**.

    ```
    https://excel.cloud.microsoft/
    ```

2. Take a moment to review the data. The spreadsheet contains columns for:
    - Region, Territory, Sales Rep
    - Product Category, Brand
    - Monthly revenue (October, November, December)
    - Q4 Total, Q4 Target, Variance
    - Account Type (Retail, Convenience, Foodservice)

3. Ensure the data is formatted as a Table (if not, select the data range and go to **Insert > Table**).

4. Select **Copilot** in the **Home** tab of the Excel ribbon. Enter:

    ```
    Summarize the key trends in this Q4 sales data. Which regions are performing above target? Which are below? What product categories are driving the most revenue?
    ```

5. Review the analysis. Ask a follow-up:

    ```
    Create and insert a bar chart comparing total Q4 revenue by region. Sort from highest to lowest.
    ```

6. Ask Copilot to dig deeper:

    ```
    Which sales reps had the biggest positive variance vs. target? And which had the biggest negative variance? Show me the top 5 and bottom 5.
    ```

7. Now ask Copilot to help with formulas:

    ```
    Add a new column called "Performance Rating" that rates each rep as "Exceeds" if their variance is above 5%, "Meets" if between -5% and 5%, and "Below" if more than -5% below target.
    ```

---

### Task 2: Analyze warehouse operations data (15 min)

1. Open **GJ_Warehouse_Ops_Report.xlsx** from your OneDrive.

2. Review the data. This spreadsheet tracks:
    - Warehouse Location
    - Month, Week
    - Cases Shipped, Cases Damaged, On-Time Delivery %
    - Labor Hours, Overtime Hours
    - Incidents Reported

3. Select **Copilot** in the **Home** tab of the ribbon and enter:

    ```
    Analyze this warehouse operations data. Which warehouses have the highest damage rates? Is there a correlation between overtime hours and damage rates? Summarize the key findings.
    ```

4. Ask for a visualization:

    ```
    Create and insert a line chart showing the trend of on-time delivery percentage by warehouse location across all months.
    ```

5. Ask Copilot for actionable insights:

    ```
    Based on this data, which warehouse should be prioritized for operational improvement? What specific metrics support that recommendation?
    ```

6. Ask for one more analysis:

    ```
    Create and insert a pivot table showing average cases shipped, damage rate, and on-time delivery percentage by warehouse location. Which location has the best overall performance?
    ```
>**Warning:** Copilot in Excel may occasionally struggle with complex multi-step requests. If it can't complete a request, try breaking it into smaller parts (e.g., "Create the chart" separately from "Add the formula column").

---

### Task 3: Quick analysis for your department (10 min)

Using either the sales or warehouse data, ask Copilot a question relevant to your role:

**Accounting / Finance:**
> "Calculate the total revenue by product category and show the percentage contribution of each category to overall Q4 revenue."

**HR / L&D:**
> "Which warehouses have the highest overtime hours? Create a summary I could use to discuss workload balancing with operations leaders."

**IT:**
> "Are there patterns in the incident data that suggest a technology-related root cause? Which locations and time periods have the most incidents?"

**Field Sales:**
> "Which account types (Retail, Convenience, Foodservice) are growing fastest? Create a chart showing Q4 revenue by account type."

**Operations / Supply Chain:**
> "Rank the warehouses by efficiency — consider cases shipped per labor hour, damage rate, and on-time delivery. Which warehouse is most efficient overall?"

Pick one, submit it, and iterate to refine the output.

<!-- ---

### Advanced: Python in Excel with Copilot (bonus, 10 min)

> [!NOTE]
> Python in Excel is available in Excel for Windows (Microsoft 365 Insiders and rolling out broadly). If your version supports it, you can use Copilot to generate Python code that runs directly in your workbook for advanced analytics.

If Python in Excel is available in your environment:

1. Open **GJ_Q4_Sales_Performance.xlsx** in **Excel for Windows** (desktop app).

2. Select a cell outside the data table. In the **Formulas** tab, select **Insert Python**.

3. Open the **Copilot** pane in the **Home** tab and enter:

    ```
    Using Python, create a correlation analysis between Q4 Total revenue and Variance for each region. Show the results as a heatmap.
    ```

4. If Copilot generates Python code, review it and select **Apply** to run it in the workbook.

5. Try another advanced analysis:

    **Using Python, perform a simple linear regression to predict which sales reps are likely to miss their targets next quarter based on their Q4 trend. Show the results as a scatter plot with a trend line.**

> [!TIP]
> Python in Excel is powerful for statistical analysis, machine learning, and custom visualizations that go beyond standard Excel charts. Copilot can generate the Python code for you — no programming experience required. -->