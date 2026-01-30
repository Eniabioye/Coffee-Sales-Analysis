
# What I Learned Building the Same Dashboard Twice: A Coffee Sales Analytics Project



## Project Overview

This project documents and compares two Excel-based coffee sales dashboards built using the same dataset but different approaches. The first dashboard was created independently without guidance, while the second was built by following an online tutorial.
The purpose of the project was to evaluate both approaches, identify strengths and limitations, and extract best practices for future data analytics projects.

## Data Structure and Preparation

### Self-Built Dashboard Approach

The dataset consisted of three sheets: Orders, Customers, and Products.
I began by checking for duplicates across all sheets, then loaded the data into Power Query. Using Order ID, Customer ID, and Product ID as unique keys, I merged the tables into a single dataset.

I created Year and Month fields from the Order Date to support time-based analysis. Data standardization followed, where coffee types (e.g., Rob, Ara) and roast types (D, M, L) were expanded into full descriptive names. Product sizes were converted into kilograms for consistency.
A Total Sales column was calculated as:

Total Sales = Unit Price × Quantity

Key learning: Raw data is rarely analysis-ready and must be cleaned, standardized, and structured before meaningful insights can be generated.

### Guided Project Approach

In the guided project, the data structure differed slightly. Instead of merging tables upfront, the tutor used XLOOKUPand INDEX–MATCH to retrieve customer and product details into the Orders table.
Coffee and roast types were categorized using IF formulas, and sales metrics were calculated similarly.

Key learning: This approach emphasized Excel formula mastery rather than data modeling or transformation.


## Dashboard Design and Analysis

Both dashboards produced the same core business insights:

Sales trends over time

Best-performing coffee types

Top revenue-generating countries

Top five customers

Common tools used included pivot tables, timelines, slicers, line charts, and bar charts.

Key learning: Different data preparation techniques can still lead to identical analytical outcomes if the underlying logic is sound.


## Comparison and Reflections

The Power Query approach proved more scalable, efficient, and professional. It supports large datasets, enables one-click refreshes, reduces formula-related errors, and documents every transformation step. This mirrors real-world data analyst workflows.

The formula-based approach, however, offers immediate transparency and is easier to trace step-by-step, making it suitable for small datasets and one-time analyses.


## Conclusion:
Formulas are ideal for small, quick, and highly transparent analyses, while Power Query is better suited for large datasets, recurring updates, and production-level dashboards. In real-world projects, both approaches are often used together.


## Final Advice

For beginners building dashboards:

Attempt the project independently first.

Research, experiment, and learn through trial and error.

Then follow a guided tutorial and compare approaches.

Build a final version that combines the strengths of both methods.

There is no single “right” way to analyze data—only the right technique for the problem at hand.
