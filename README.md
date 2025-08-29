# Analyzing Gamezone's Revenue Drivers and Marketing Efficiency

# Project Background
**Gamezone**, founded in 2018, is a global retailer of new and refurbished gaming products, operating primarily through its online store and mobile app. The company leverages a variety of marketing channels to drive customer acquisition and sales.

Despite possessing extensive sales data, this information has historically been underutilized. This project conducts a comprehensive analysis of that data to uncover actionable insights aimed at enhancing Gamezone’s commercial strategy and operational efficiency.

The primary objective of this analysis is to identify key revenue drivers and evaluate the effectiveness of marketing efforts. The findings will support strategic decision-making to optimize marketing spend, improve platform performance, and maximize product profitability.
Insights and recommendations are provided across the following key business areas:

- **Sales Performance and Trends:** Historical and seasonal analysis of revenue, order volume, and Average Order Value (AOV) from 2019 to 2021.
- **Marketing Channel Effectiveness:** Evaluation of revenue contribution and customer value by marketing channel to guide budget allocation.
- **Platform Comparison:** Assessment of sales performance and customer behavior across the Mobile App and Online Store.
- **Product Analysis:** Identification of top-performing and underperforming products, including analysis of new versus refurbished sales mix.

The SQL queries used to inspect and clean the data for this analysis can be found here [link].

Targed SQL queries regarding various business questions can be found here [link].

An interactive Tableau dashboard used to report and explore sales trends can be found here [link].



# Data Structure & Initial Checks

The company’s main database structure, shown below, consists of a single table: gamezone_orders_data, containing a total of 21,864 records. This dataset represents order information, with each record corresponding to a unique order. The most important columns are usd_price, product_name, purchase_ts, and ship_ts. Additional information includes the platform used to place the order and geographical details such as the customer’s country. The data covers a period from 2019 to 2021.

<img width="282" height="255" alt="Data_structure" src="https://github.com/user-attachments/assets/c71d01fb-aa8e-4336-8d36-9d82e8355712" />

Before starting the analysis, a series of checks were performed to ensure data quality and to become familiar with the dataset. The SQL queries used for inspection and quality control can be found here.

# Executive Summary

### Overview of Findings

Explain the overarching findings, trends, and themes in 2-3 sentences here. This section should address the question: "If a stakeholder were to take away 3 main insights from your project, what are the most important things they should know?" You can put yourself in the shoes of a specific stakeholder - for example, a marketing manager or finance director - to think creatively about this section.

[Visualization, including a graph of overall trends or snapshot of a dashboard]



# Insights Deep Dive
### Category 1:

* **Main insight 1.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 2.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 3.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 4.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.

[Visualization specific to category 1]


### Category 2:

* **Main insight 1.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 2.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 3.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 4.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.

[Visualization specific to category 2]


### Category 3:

* **Main insight 1.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 2.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 3.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 4.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.

[Visualization specific to category 3]


### Category 4:

* **Main insight 1.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 2.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 3.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 4.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.

[Visualization specific to category 4]



# Recommendations:

Based on the insights and findings above, we would recommend the [stakeholder team] to consider the following: 

* Specific observation that is related to a recommended action. **Recommendation or general guidance based on this observation.**
  
* Specific observation that is related to a recommended action. **Recommendation or general guidance based on this observation.**
  
* Specific observation that is related to a recommended action. **Recommendation or general guidance based on this observation.**
  
* Specific observation that is related to a recommended action. **Recommendation or general guidance based on this observation.**
  
* Specific observation that is related to a recommended action. **Recommendation or general guidance based on this observation.**
  


# Assumptions and Caveats:

Throughout the analysis, multiple assumptions were made to manage challenges with the data. These assumptions and caveats are noted below:

* Assumption 1 (ex: missing country records were for customers based in the US, and were re-coded to be US citizens)
  
* Assumption 1 (ex: data for December 2021 was missing - this was imputed using a combination of historical trends and December 2020 data)
  
* Assumption 1 (ex: because 3% of the refund date column contained non-sensical dates, these were excluded from the analysis)
