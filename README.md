# Sales and Profit Performance Analysis
## Sales and Profit Performance Dashboard

### 1. Data Modeling & Relationships
The foundation of this dashboard is built using **Power Pivot**. I established a Star Schema to ensure efficient data filtering across multiple tables.
* **Fact Table:** `Orders` (contains numerical values like Sales, Profit, and Discount).
* **Dimension Tables:** `Users` and `Returns`.
* **Relationships:** Created **One-to-Many ($1:\infty$)** relationships between the primary keys in the dimension tables and the foreign keys in the Orders table.

### 2. Data Transformation (Power Query)
Before building the visuals, the data was cleaned and transformed:
* **Data Typing:** Assigned correct formats (Currency for Sales/Profit, Percentages for Discounts).
* **Calculated Columns:** Created custom columns in Power Pivot to handle specific aggregations, such as identifying specific date hierarchies.

### 3. Core Visualizations & Analysis
The dashboard analyzes key performance indicators (KPIs) through several chart types:

* **Top 10 Products (Clustered Column Chart):** Compares `Sum of Profit` against `Max of Sales` to identify high-volume vs. high-margin products.
* **Regional Profitability (Area Chart):** A visual representation of `Average Profit` across Central, East, South, and West regions.
* **Shipping & Logistics (Pie Chart):** Breakdown of `Sum of Sales` by `Ship Mode` (Regular Air, Express Air, Delivery Truck).
* **Trend Analysis (Line Chart):** Sub-category wise sales count to identify which product lines are the most active.

### 4. Interactive Elements (Slicers & Timelines)
To make the dashboard dynamic, I implemented a robust filtering pane on the right side:
* **Slicers:** Added slicers for `Order Priority`, `Customer Segment`, `State or Province`, `Region`, and `Product Container`.
* **Timeline:** Included an `Order Date` timeline to allow users to drill down into specific months or years.
* **Report Connections:** Linked all slicers to every Pivot Chart on the dashboard to ensure a unified view when a filter is applied.

### 5. UI/UX Design
* **Consistency:** Used a unified color palette (Blue/White/Grey) to maintain a professional look.
* **Alignment:** Grouped slicers systematically on the right to maximize the "real estate" for the charts.
* **Readability:** Removed gridlines and used custom chart titles for clarity.

<img width="1620" height="624" alt="Screenshot 2025-11-10 223418" src="https://github.com/user-attachments/assets/ab8df015-ce6c-4bcb-8b8b-8d28328fbad3" />
<img width="1885" height="640" alt="Screenshot 2025-11-10 220942" src="https://github.com/user-attachments/assets/17ce3f3b-2d79-4aef-a386-fe1d9dfdba15" />
<img width="1887" height="651" alt="Screenshot 2025-11-10 220926" src="https://github.com/user-attachments/assets/68f3045a-eb5e-464d-bdcd-103e77fbf4ba" />
<img width="1883" height="658" alt="Screenshot 2025-11-10 220753" src="https://github.com/user-attachments/assets/be7ed32d-d931-41b5-9fc9-688415847c2d" />
<img width="1883" height="632" alt="Screenshot 2025-11-10 220723" src="https://github.com/user-attachments/assets/97afa8b2-0307-4860-99e5-02519bba53e5" />
<img width="1885" height="638" alt="Screenshot 2025-11-10 220704" src="https://github.com/user-attachments/assets/504acaf2-0040-44e3-9205-0556f37b413e" />
<img width="1884" height="657" alt="Screenshot 2025-11-10 220641" src="https://github.com/user-attachments/assets/b0b46847-3936-4e80-9f97-c5da1e74e070" />
<img width="1524" height="678" alt="Screenshot 2025-11-10 183808" src="https://github.com/user-attachments/assets/f607b41c-524e-4864-b452-8fd8f897c712" />
