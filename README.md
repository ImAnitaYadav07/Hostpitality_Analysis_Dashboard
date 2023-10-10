# Revenue Insight of Hospitality Domain
<b>Domain :<b/>Hostpitality<br>
<b>Function :<b/>Revenue

## Background

AtliQ Grands owns multiple five-star hotels across India. They have been in the hospitality industry for the past 20 years. Due to strategic moves from other competitors and ineffective decision-making in management, AtliQ Grands are losing its market share and revenue in the luxury/business hotels category. As a strategic move, the managing director of AtliQ Grands wanted to incorporate “Business and Data Intelligence” to regain their market share and revenue.

As a data analyst I have created new interactive dashboard using their sample data and a mock-up dashboard to work on the following task.

* To create the metrics according to the metric list.
* To create a dashboard according to the mock-up provided by stakeholders.
* To create relevant insights that are not provided in the metric list/mock-up dashboard.

## Files

* Booking date - [dim_date.csv](Hostpitality_Analysis_Dashboard/dim_date.csv)
* Hotels [dim.csv](Hostpitality_Analysis_Dashboard/dim_hotels.csv) 
* Hotal Room Type [dim_rooms](Hostpitality_Analysis_Dashboard/dim_date.csv)
* Matrics List - [Matrics list.xlsx](Hostpitality_Analysis_Dashboard/matrics list.xlsx)
* Revenue Insight Dashbord [Dashboard Starter Jupyter Notebook](Hostpitality_Analysis_Dashboard/hospitality dashboard.pbix)

### Rental Analysis

The first step to building the dashboard is to work out all erros, null values and all the calculations and visualizations.

WoW - Week-on-Week (WoW) is a type of business metric that measures changes in a specific variable over a period of one week compared to the previous week. It is a common way of tracking business performance over time and is particularly useful for analyzing trends and identifying areas where improvements can be made.

### Visualisation of key matrices and DAX Calculation- 

   
```
   Revenue = SUM(fact_bookings[revenue_realized])
```
```
    RevPAR = DIVIDE([Revenue],[Total Capacity])
```
```
   DSRN = RevPAR = DIVIDE([Revenue],[Total Capacity])
```
```
   ADR = DIVIDE( [Revenue], [Total Bookings],0)
```
```
   Realisation % = 1- ([Cancellation %]+[No Show rate %])
```
```
   Occupancy % = DIVIDE([Total Succesful Bookings],[Total Capacity],0)
```

### Trend By Key Matrics - 

1. Revenue Trend by Week
   <img align='right' src="Hostpitality_Analysis_Dashboard/RevenueWOW.png" width="600" height="200" padding = 50px>
2. RevPAR Trebd by Week and Day Type
    <img align='right' src="Hostpitality_Analysis_Dashboard/RevByWeek.png" width="600" height="200">
3. DSRN by Week
    <img align='right' src="Hostpitality_Analysis_Dashboard/DSRNbyWeek.png" width="600" height="200">
4. Occupancy % by Week and Day Type
    <img align='right' src="Hostpitality_Analysis_Dashboard/OccupencyByWeek.png" width="600" height="200">
5. ADR by Week
     <img align='right' src="Hostpitality_Analysis_Dashboard/ADRbyWeek.png" width="600" height="200">
6.  Realisation % by Week and Day Type
   <img align='right' src="Hostpitality_Analysis_Dashboard/RealisationWeek.png" width="500" height="200">
   
<hr style="width:80%">

### Revenue By Category - 
<img align='right' src="Hostpitality_Analysis_Dashboard/.png" width="600" height="200">

### Realisation % and ADR by Platform - 
<img align='right' src="Hostpitality_Analysis_Dashboard/.png" width="600" height="200">

### Properties By key Matrics - 
<img align='right' src="Hostpitality_Analysis_Dashboard/.png" width="800" height="500">

## MockUp Dashboard -
<img src="Hostpitality_Analysis_Dashboard/Mockup_Dashboard.png" width="800" height="500">

## Updated Dashboard -

final Dashboard - [Revenue insight Dashboard](https://app.powerbi.com/links/ugSfV8GChZ?ctid=c3261a2c-fdd4-42d9-aa75-3d2ff751da4c&pbi_source=linkShare)]

<img src="Hostpitality_Analysis_Dashboard/Revenue_Dashboard.png" width="800" height="500">
