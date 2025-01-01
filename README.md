# Dynamic Retail Dashboard in Excel

### Overview

The **Dynamic Retail Dashboard** is an advanced Excel tool for visualizing and analyzing retail data. By leveraging Power Query and interactive features, it connects to datasets hosted on GitHub, performs data transformations, and delivers insights through dynamic charts and Key Performance Indicators (KPIs). This tool addresses key business challenges and empowers decision-makers with actionable insights.

---

### **Datasets Used**

#### 1. **Orders Table**
   - Details customer orders, including product data, shipping information, and financial metrics.

   **Sample Data**:
   | Order ID          | Returned | Order Date | Ship Date | Ship Mode   | Customer Name  | Segment    | Country       | Market | Sales   | Profit  | Discount |
   |-------------------|----------|------------|-----------|-------------|----------------|------------|---------------|--------|---------|---------|----------|
   | CA-2012-124891    | No       | 31-07-2020 | 31-07-2020 | Same Day    | Rick Hansen    | Consumer   | United States | US     | 2309.65 | 762.18  | 0        |
   | IN-2013-77878     | Yes      | 05-02-2021 | 07-02-2021 | Second Class | Justin Ritter  | Corporate  | Australia     | APAC   | 3709.40 | -288.77 | 0.1      |
   | IN-2013-71249     | No       | 17-10-2021 | 18-10-2021 | First Class | Craig Reiter   | Consumer   | Australia     | APAC   | 5175.17 | 919.97  | 0.1      |

#### 2. **Returns Table**
   - Tracks returned orders and their respective markets.

   **Sample Data**:
   | Returned | Order ID           | Market   |
   |----------|--------------------|----------|
   | Yes      | MX-2013-168137     | LATAM    |
   | Yes      | US-2011-165316     | LATAM    |
   | Yes      | ES-2013-1525878    | EU       |
   | Yes      | CA-2013-118311     | United States |

#### 3. **People Table**
   - Lists sales representatives and the regions they manage.

   **Sample Data**:
   | Person            | Region   |
   |-------------------|----------|
   | Anna Andreadi     | Central  |
   | Chuck Magee       | South    |
   | Kelly Williams    | East     |
   | Matt Collister    | West     |
   | Deborah Brumfield | Africa   |

---

### **Problem Statements and Solutions**

#### 1. **Key Performance Indicators (KPIs)**
   - **Objective**: Display metrics like Total Sales, Total Profit, Orders Count, and Profit Margin dynamically.

   **Solution**:
   - Import the **Orders Table** via **Power Query**.
   - Create calculated fields:
     - **Profit Margin**: `Profit / Sales`
     - **Order Count**: `Count of Order ID`
   - Summarize key metrics using formulas:
     - **Total Sales**: `=SUM(Sales)`
     - **Total Profit**: `=SUM(Profit)`
   - Use symbols to enhance readability in the KPI table (e.g., 💰 for Total Sales).

#### 2. **Trend Analysis (Sales & Profit)**
   - **Objective**: Track sales and profit trends over time.

   **Solution**:
   - Group data by Year and Month using a **Pivot Table**.
   - Plot Sales and Profit on a **Line Chart**.
   - Add interactive **Slicers** for filtering by categories or markets.

#### 3. **Profit by Category**
   - **Objective**: Identify the most and least profitable categories.

   **Solution**:
   - Create a **Pivot Table** with Categories and Profits.
   - Visualize using a **Bar Chart**.
   - Add Slicers for dynamic filtering by region or time period.

#### 4. **Segment-Wise Sales Share**
   - **Objective**: Show the percentage share of sales for each customer segment.

   **Solution**:
   - Use a **Pivot Table** with Segments and Sales.
   - Calculate percentage share dynamically.
   - Present the data using a **Donut Chart** with labeled values.

#### 5. **Geographic Sales Analysis**
   - **Objective**: Highlight sales performance by country.

   **Solution**:
   - Create a **Pivot Table** with Countries and Sales.
   - Use Conditional Formatting to highlight high-performing regions.
   - Visualize using a **Map Chart**.

#### 6. **Top and Bottom Subcategories**
   - **Objective**: Identify the top 5 and bottom 5 subcategories by sales.

   **Solution**:
   - Rank subcategories using a **Pivot Table**.
   - Visualize top 5 and bottom 5 using separate **Column Charts** with distinct color schemes.

#### 7. **Yearly Sales Trends**
   - **Objective**: Monitor sales trends over years.

   **Solution**:
   - Group order data by Year in a **Pivot Table**.
   - Display trends using a **Line Chart**.
   - Add filters for deeper analysis.

---

### **Dynamic Features**

- **Interactive Charts**: Updates automatically based on slicer selections.
- **Power Query Automation**: Ensures efficient data cleaning and transformation.
- **Slicer Filters**: Provides intuitive filtering by year, region, category, and more.

---

### **Extensions and Future Scope**

- **Return Analysis**: Evaluate return rates by category and market.
- **Customer Profitability**: Highlight top and bottom customers by profitability.
- **Market Comparison**: Benchmark performance across different regions.
- **Detailed Product Insights**: Drill down into individual product performance.

---

### **Impact**

The **Dynamic Retail Dashboard** offers:
- A streamlined view of retail performance.
- Enhanced decision-making through data-driven insights.
- Tools for identifying growth opportunities and areas needing improvement.

---

### **Visual Examples**

The dashboard includes:
- KPI visualizations.
- Time-series charts for trends.
- Geo-charts for regional sales.
- Pie charts for segment analysis.

Screenshots of the working dashboard are available in the repository for reference.


