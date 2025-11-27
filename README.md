# Sample Superstore Power BI Dashboard


## Problem Statement

An interactive Power BI report providing a complete analysis of sales, profit, and regional performance using the Sample Superstore dataset.

The Sample Superstore Report offers an end-to-end analytical breakdown of business performance across regions, categories, sub-categories, states, and years.
It helps users identify:

- Top-selling and low-performing products
- Regional revenue contributions
- Yearly growth trends
- Profitability insights
- Category and segment distribution
- State-specific business performance

This dashboard supports data-driven decision-making for supply chain, marketing, sales strategy, and product management.


### Steps followed 

- Step 1 : Load the data into Power BI Desktop, the file was in csv format.
- Step 2 : Opened power query editor and in view tab, under Data preview section, check "column distribution", "column quality" and "column profile" options.
- Step 3 : By default, column profile will be opened only for 1000 rows, so you will need to select "column profiling based on entire dataset".
- Step 4 : It was observed that in none of the columns errors and no empty values were present.
- step 6 : New measure named "Targeted Profit" made to extract the 1.45 times the actual profit to showcase the target.
  
           a) DAX for Targeted Profit = SUM(Orders[Profit])*1.45
- Step 8 : Visual filters (Slicers) were added for the field named "States".
- Step 10 : Three card visuals were added to the canvas/dashboard, representing "Total Sales", "Total Quantity",  and "Total Profit".
- Step 11 : Crated a table for the view of "Categories", "Sub-Categories", "Total Profit" and " Total Sales".
- step 12 : Added a Guage to get the Targeted profit and Actual profit, Targated Profit measure was added to this Guage in Target valule section.
- step 13 : Line Chart was added to get the Total sales by region and year.
- step 14 : Funnel chart to get the insights on sales by sub-categories.
- step 15 : Three donut charts were added to get the details on Total sales by region, Count of categories by region and Count of segment by region respectively.



  # Report Snapshot (Power BI DESKTOP)

 
![Dashboard_upload](https://github.com/rahulgowda2003/Netflix-Sample-Data-Dashboard/blob/main/Netflix%20Dashboard%20Screenshot.png)

# Insights

a) Key Metrics (KPIs)

KPI	Value

- Total Sales	: 9994
- Total Quantity : 38K
- Total Profit : 286.40K

These metrics provide a quick, high-level snapshot of store performance.

b) Slicers

State Filter

A state-level slicer allowing users to drill down into specific region-level insights.
Includes all U.S. states such as:

- Alabama
- Arizona
- Arkansas
- California
- Colorado
- Connecticut
- Delaware
- Florida
- Georgia
- Idaho

…and many more.

Users can select single or multiple states, or use Select All.

c) Visualizations in the Dashboard

1] Table – Total Profit and Total Sales by Sub-Category and Category

A detailed profitability and revenue breakdown:

Sub-Category	  Category	Total Profit	Total Sales
Accessories	    Technology	41,936.64	775
Appliances	    Office Supplies	18,138.01	466
Art	Office      Supplies	6,527.79	796
Binders	        Office Supplies	30,221.76	1523
Bookcases	      Furniture	-3,472.56	228
Chairs	        Furniture	26,590.17	617
Copiers	        Technology	55,617.82	68
Envelopes	      Office Supplies	6,964.18	254
Fasteners	      Office Supplies	949.52	217
Furnishings	    Furniture	13,059.14	957
Labels	        Office Supplies	5,546.25	364
Machines	      Technology	3,384.76	115
Paper	          Office Supplies	34,053.57	1370
Phones	        Technology	44,515.73	889
Storage	Office Supplies	24,578.89	905
Supplies	Office Supplies	3,023.24	47
Art	Office Supplies	6,527.79	27
Envelopes	Office Supplies	6,964.18	16
Labels	Office Supplies	5,546.25	12
Fasteners	Office Supplies	949.52	3
Grand Totals

Total Profit: 286,397.02

Total Sales: 9,994

2️⃣ Line Chart – Total Sales by Year and Region

Years: 2014, 2015, 2016, 2017
Regions: Central, East, South, West

Insight:
Sales increased steadily from 2014–2017, with East and West showing the steepest upward trends.

3️⃣ Donut Chart – Total Sales by Region
Region	Sales	Share
West	725K	32%
South	679K	30%
Central	501K	22%
East	392K	17%

Insight:
The West region contributes the most to total sales.

4️⃣ Bar Chart – Total Sales by Sub-Category

Ranked sales performance:

Sub-Category	Sales
Phones	286K
Chairs	224K
Storage	207K
Tables	203K
Binders	203K
Machines	189K
Accessories	167K
Copiers	150K
Bookcases	115K
Appliances	108K
Furnishings	92K
Paper	78K
Supplies	47K
Art	27K
Envelopes	16K
Labels	12K
Fasteners	3K
5️⃣ Donut Chart – Count of Category by Region

West: 3K (32%)

South: 3K (28%)

Central: 2K (23%)

East: 2K (16%)

6️⃣ Donut Chart – Count of Segment by Region

Similar distribution pattern:

West: 32%

South: 28%

Central: 23%

East: 16%

7️⃣ Gauge Chart – Total Profit vs Targeted Profit

Current Profit: 286.40K

Target: approx. 572.79K

Gauge visual shows progress toward profit goal.

🌍 Key Insights
✔ Regional Performance

West region leads in both total sales and product distribution.

East and Central contribute significantly but lag behind.

✔ Sub-Category Analysis

Highest performers: Phones, Chairs, Storage, Tables

Low performers: Fasteners, Labels, Envelopes, Art

✔ Profitability Trends

Copiers, Chairs, Accessories show strong profit margins.

Bookcases show negative profit, indicating loss potential.

✔ Yearly Trends

Steady rise from 2014–2017 across all regions, confirming consistent business growth.
