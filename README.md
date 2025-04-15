#Power BI Dashboard: Production Performance & Cost Analysis
This repository contains all the DAX functions and formulas used to create the Production Performance & Cost Analysis Power BI dashboard. The dashboard aims to visualize and analyze key production metrics such as production costs, defects, and production efficiency across different production lines.

#Project Overview
The Power BI dashboard provides the following insights:

Production Volume: Displays the total quantity of products produced per manufacturing date.

Production Cost Analysis: Breaks down the total production cost into material, labor, and overhead costs.

Defect Tracking: Tracks the number of defects per product and production line.

Production Line Efficiency: Compares the performance and output of different production lines.

By utilizing various DAX functions, the dashboard is able to perform complex calculations, such as aggregating costs, calculating averages, and identifying trends across time.

#DAX Functions
In this repository, you'll find the following DAX measures that were used to power the visualizations and insights in the Power BI dashboard:# Power-BI-Dashboard-Production-Performance-Cost-Analysis

Total Difects = SUM(ManufacturingData[Defects])

Total Labor Cost = SUM(ManufacturingData[Labour_Cost])

Total Material Cost = SUM(ManufacturingData[Material_Cost])

Total Overhead Cost = SUM(ManufacturingData[Overhead_Cost])

Total Production Cost = SUM(ManufacturingData[Production_Cost])

Total Quantity Produced = SUM(ManufacturingData[Quantity_Produced])

Production Efficiency = (SUM(ManufacturingData[Quantity_Produced]) - SUM(ManufacturingData[Defects])) / SUM(ManufacturingData[Quantity_Produced])

Aveage Production Cost = AVERAGE( ManufacturingData[Production_Cost])

Average Defects = AVERAGE(ManufacturingData[Defects])

Average Defects per Product = AVERAGE(ManufacturingData[Defects])

Average Material Cost = AVERAGE(ManufacturingData[Material_Cost])

Average Overhead Cost = AVERAGE(ManufacturingData[Overhead_Cost])

Cost per Unit Produced = DIVIDE(SUM(ManufacturingData[Production_Cost]),SUM(ManufacturingData[Quantity_Produced]))

Defect Rate per Production Line = DIVIDE(SUM(ManufacturingData[Defects]),SUM(ManufacturingData[Quantity_Produced]))

#How to Use
Clone or download this repository to your local machine.

Open the Power BI file (.pbix) and import the dataset used for the dashboard.

In Power BI, go to the Modeling tab and paste the DAX formulas into the New Measure field.

Visualize the measures in your Power BI reports by dragging them onto your canvas and applying appropriate charts or tables.

#Dependencies
Power BI Desktop: To view and interact with the dashboard.

DAX: Data Analysis Expressions for creating dynamic calculations.

Dataset: The data set used contains information about product production, costs, defects, and production lines.

#Contributing
Feel free to fork this repository and contribute by adding more DAX measures or improving the existing code. Any suggestions or improvements are welcome.

