# Maven-Hotel-Group-Dashboard-Project

Hi 👋, and welcome to the **Maven-Hotel-Group-Dashboard-Project** repository!  
First of all, a huge thanks to **Maven Analytics** for guiding me to build this dashboard project using Excel. This project demonstrates how to create a dashboard for transforming some interesting insights into a visualization. In this imaginary case, I'm playing the role as a Data Visualization Specialist for Maven Hotel Group (MHG), a Portuguese hotel chain with resorts in Lisbon and Algarve.

---

## Table of Contents

1. [Project Overview](#project-overview)
2. [Business Objective](#business-objective)
   - [Seasonality Analysis](#seasonality-analysis)
   - [Revenue Loss Analysis](#revenue-loss-analysis)
   - [Lead Time Impact Analysis](#lead-time-impact-analysis)
   - [Strategic Overbooking Opportunity](#strategic-overbooking-opportunity)
3. [Creating Dashboard](#creating-dashboard)
   - [Visualizing Seasonality Analysis with a Combo Chart](#visualizing-seasonality-analysis-with-a-combo-chart)
   - [Visualizing Revenue Loss Analysis with a Combo Chart](#visualizing-revenue-loss-analysis-with-a-combo-chart)
   - [Visualizing Lead Time Impact Analysis with a Stacked Bar Chart](#visualizing-lead-time-impact-analysis-with-a-stacked-bar-chart)
   - [Visualizing Strategic Overbooking Opportunity with a Bar Chart](#visualizing-strategic-overbooking-opportunity-with-a-bar-chart)
   - [Integrating Charts with Text into a Dashboard](#integrating-charts-with-text-into-a-dashboard)
4. [Conclusion](#conclusion)

---

## Project Overview

This project involves:
1. Creating a dashboard based on key insights during exploratory data analysis.
2. Utilized pivot charts for effective visualization.
3. Leverage the dashboard with text to clearly communicate key insights and business recommendations.

---

## Business Objective

First, let's take a look at this image below:  
![](https://github.com/Mufalta/Excel-Maven-Hotel-Group-Dashboard-Project/blob/main/images/An-Email.png)

As you can see, we received an email from our teammate Billy, a Business Analyst, requesting our help to build a dashboard for reporting purposes. He also included the dataset along with some interesting insights he discovered. Okay, so our next step is to open the file he attached in the email:

![](https://github.com/Mufalta/Excel-Maven-Hotel-Group-Dashboard-Project/blob/main/images/Excel.png)

In the Excel file, there are two sheets: one contains the dataset, and the other contains the analysis prepared by our teammate. Next, we’re going to spend most of our time working in the analysis worksheet. As you can see, we clearly have a lot to figure out, so it’s better to break it down into several parts.

---

### Seasonality Analysis

![](https://github.com/Mufalta/Excel-Maven-Hotel-Group-Dashboard-Project/blob/main/images/Seasonality-Analysis.png)

In this section, we analyzed seasonality to identify patterns in cancellation rates and average daily rates. During July and August, we observe a spike in both cancellation rates and average daily rates, indicating that while customers are willing to pay higher rates during summer, they are also more likely to cancel.

---

### Revenue Loss Analysis

![](https://github.com/Mufalta/Excel-Maven-Hotel-Group-Dashboard-Project/blob/main/images/Revenue-Loss-Analysis.png)

In this section, we analyzed revenue loss. The data shows that July and August account for nearly $1,000,000 in revenue losses due to high cancellation rates, even though these months generate the highest revenue.

---

### Lead Time Impact Analysis

![](https://github.com/Mufalta/Excel-Maven-Hotel-Group-Dashboard-Project/blob/main/images/Lead-Time-Impact-Analysis.png)

In this section, we examined the relationship between lead time and cancellations. The data reveals that reservations booked more than 30 days in advance have significantly higher cancellation rates, with 859 cancellations compared to only 175 for bookings within 0–30 days. This indicates that long lead-time reservations are the primary contributors to revenue loss.

---

### Strategic Overbooking Opportunity

![](https://github.com/Mufalta/Excel-Maven-Hotel-Group-Dashboard-Project/blob/main/images/Strategic-Overbooking-Opportunity.png)

In this section, we discovered a tactical opportunity to offset cancellation-related losses:
- **Short lead-time** bookings (0–30 days) have a lower cancellation rate (20%) and higher average daily rates ($191).
- **Long lead-time** bookings (>30 days) have a higher cancellation rate (38%) and lower average daily rates ($169).

---

## Creating Dashboard

After understanding the business objective from those four key indicators, it’s now time to build the dashboard. However, before that, it’s best to first create the appropriate chart types for each key indicator identified in the previous analysis. Once we have the right charts for each indicator, we can seamlessly combine them into a comprehensive dashboard.

---

### Visualizing Seasonality Analysis with a Combo Chart

![](https://github.com/Mufalta/Excel-Maven-Hotel-Group-Dashboard-Project/blob/main/images/Seasonality-Analysis-Combo-Chart.png)

This will be our first chart, so let’s start by looking at the pivot table we created for the seasonality analysis. In this pivot table, we have two metrics: the **cancellation rate** and the **average daily rate**. We want all the data from this pivot table to be reflected in the chart. Since we have two metrics to display, using a combo chart will be the perfect choice.

---

### Visualizing Revenue Loss Analysis with a Combo Chart

![](https://github.com/Mufalta/Excel-Maven-Hotel-Group-Dashboard-Project/blob/main/images/Revenue-Loss-Analysis-Combo-Chart.png)

After creating our first chart, let’s move on to the next one, which is the revenue loss analysis pivot table. Similar to the previous data, this pivot table has two metrics: the **revenue** and the **revenue loss**. We can still use a combo chart here, but since the revenue loss data is on a negative scale, it’s better to display both revenue and revenue loss as columns for clear comparison.

---

### Visualizing Lead Time Impact Analysis with a Stacked Bar Chart

![](https://github.com/Mufalta/Excel-Maven-Hotel-Group-Dashboard-Project/blob/main/images/Lead-Time-Impact-Analysis-Stacked-Bar-Chart.png)

Next, we’re going to create a chart for the data in the lead time impact analysis pivot table. This time, we’ll use a different chart type because we want to visualize the composition of cancellations by lead time. A stacked bar chart is the perfect choice here, as it shows proportions clearly while taking up less space than a pie chart.

---

### Visualizing Strategic Overbooking Opportunity with a Bar Chart

![](https://github.com/Mufalta/Excel-Maven-Hotel-Group-Dashboard-Project/blob/main/images/Strategic-Overbooking-Opportunity-Bar-Chart.png)

Finally, we have the last insight to visualize: the data in the strategic overbooking opportunity pivot table. Here, we have two metrics categorized by lead time: the **cancellation rate** and the **average daily rate**. For this purpose, we will create two separate bar charts, one for the cancellation rate by lead time, and another for the average daily rate by lead time.

---

### Integrating Charts with Text into a Dashboard

All right, so far we’ve created different types of charts based on the analysis Billy had prepared. However, we still have a problem: **there’s no context** provided for each chart. For example, in the first chart, how can we know that the line chart represents as cancellation rate and the column chart represents as average daily rate?. To make these charts meaningful, we need to add context with clear text labels. Once we’ve added this context, we can combine the charts into a dashboard.

![](https://github.com/Mufalta/Excel-Maven-Hotel-Group-Dashboard-Project/blob/main/images/Dashboard.png)

---

## Conclusion

Now, it’s time to walk through what our dashboard is telling us:

### 📈 Seasonality Analysis

We started by analyzing cancellation rates and average daily rates across months. The first chart shows that both cancellation rates and prices spike during the summer months (July and August), indicating seasonality. For example, in August 2017, the cancellation rate peaked at 39%, while the average daily rate reached its highest point. This pattern suggests that while we can charge higher prices during peak seasons, we also face higher cancellation rates.

### 💸 Revenue Loss Analysis

Next, we examined revenue and revenue losses across each month. We found that the highest revenue months (July and August) are also the months with the largest revenue losses from cancellations, with losses totaling ~$1 million in July and August 2016. This means that while summer brings in more bookings, cancellations heavily impact our revenue during these months.

### ⏳ Lead Time Impact Analysis

We then explored the impact of lead time on cancellations, with bookings made within 30 days accounting for 17% of cancellations. This indicates that early bookings have a much higher cancellation risk, contributing significantly to our revenue losses.

### 🎯 Strategic Overbooking Opportunity

Finally, we looked into opportunities for strategic overbooking. We found that same-month bookings (0-30 days) have a lower cancellation rate (20%) and higher average daily rates ($191) compared to early bookings (38% cancellation rate and $169 ADR). This insight suggests that by overbooking during the summer, we can replace high-risk early bookings with low-risk, high-value same-month bookings, reducing cancellations while increasing revenue.
