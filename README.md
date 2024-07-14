# Car Sales Dashboard - Power BI Project

## About Company
Our company, a car dealership, aims to enhance sales performance tracking and analysis through an efficient Car Sales Dashboard in Power BI.

## Objective
Design and develop a dynamic, interactive Car Sales Dashboard to visualize critical KPIs, enabling data-driven decision-making and understanding sales performance trends over time.

## Problem Statement 1: KPI’s Requirement
### Sales Overview:
- Year-to-Date (YTD) Total Sales
- Month-to-Date (MTD) Total Sales
- Year-over-Year (YOY) Growth in Total Sales
- Difference between YTD Sales and Previous Year-to-Date (PTYD) Sales

### Average Price Analysis:
- YTD Average Price
- MTD Average Price
- YOY Growth in Average Price
- Difference between YTD Average Price and PTYD Average Price

### Cars Sold Metrics:
- YTD Cars Sold
- MTD Cars Sold
- YOY Growth in Cars Sold
- Difference between YTD Cars Sold and PTYD Cars Sold

## Problem Statement 2: Charts Requirement
1. **YTD Sales Weekly Trend:** Display a line chart illustrating the weekly trend of YTD sales. The X-axis should represent weeks, and the Y-axis should show the total sales amount.
2. **YTD Total Sales by Body Style:** Visualize the distribution of YTD total sales across different car body styles using a Pie chart.
3. **YTD Total Sales by Color:** Present the contribution of various car colors to the YTD total sales through a pie chart.
4. **YTD Cars Sold by Dealer Region:** Showcase the YTD sales data based on different dealer regions using a map chart to visualize the sales distribution geographically.
5. **Company-Wise Sales Trend in Grid Form:** Provide a tabular grid that displays the sales trend for each company. The grid should showcase the company name along with their YTD sales figures.
6. **Details Grid Showing All Car Sales Information:** Create a detailed grid that presents all relevant information for each car sale, including car model, body style, color, sales amount, dealer region, date, etc.

## Data Available
### Car Data:
- Car ID
- Date
- Customer Name
- Gender
- Annual Income
- Dealer Name
- Company
- Model
- Engine
- Transmission
- Color
- Price ($)
- Dealer No
- Body Style
- Phone
- Dealer Region

### Calendar Table (Created):
- Date
- Month
- Week
- Year

### DashBoard 

![home1](/Users/hansimgluck/Desktop/powerbi/project_bild.png)
![home2](/Users/hansimgluck/Desktop/powerbi/303842888-a2efe884-ad4d-4f66-b2a6-205b01120b4a.png)

**Problem Statement 1: KPI’s**

**Sales Overview:**
- **YTD Total Sales:** $371.2M
    - **Formula:** `SUM('Car Data'[Total Sales])`
- **MTD Total Sales:** $54.28M
    - **Formula:** `CALCULATE(SUM('Car Data'[Total Sales]), DATESMTD('Calendar Table'[Date]))`
- **YOY Growth in Total Sales:** 23.6%
    - **Formula:** `[Sales Difference]/[PTYD Total Sales]`
- **Difference between YTD Sales and PTYD Sales:** $70.8M
    - **Formula:** `[YTD Car Sales]-[PTYD Car Sales]`

**Average Price Analysis:**
- **YTD Average Price:** $28.0k
    - **Formula:** `TOTALYTD([Avg Price],'Calendar Table'[Date])`
- **MTD Average Price:** $28.26k
    - **Formula:** `TOTALMTD([Avg Price],'Calendar Table'[Date])`
- **YOY Growth in Average Price:** -0.79%
    - **Formula:** `[Avg Price Diff]/[PTYD Avg Price]`
- **Difference between YTD Average Price and PTYD Average Price:** $0.22k loss
    - **Formula:** `[YTD Avg Price]-[PTYD Avg Price]`

**Cars Sold Metrics:**
- **YTD Cars Sold:** 13.3K
    - **Formula:** `SUM('Car Data'[YTD Car Solds])`
- **MTD Cars Sold:** 1.92k
    - **Formula:** `CALCULATE(SUM('Car Data'[MTD Cars Sold]), DATESMTD('Calendar Table'[Date]))`
- **YOY Growth in

 Cars Sold:** 19.73%
    - **Formula:** `car_data[Cars Sold Diff]/[YTD Car Solds]`
- **Difference between YTD Cars Sold and PTYD Cars Sold:** 3K
    - **Formula:** `[YTD Car Solds]-[PTYD Car Solds]`
 
**Problem Statement 2: Charts**


**YTD Sales Weekly Trend:**
![WeeklyTrend](/Users/hansimgluck/Desktop/powerbi/303842485-006c793b-0266-49ee-b6c2-19d0bdd4e7f8.png)


**YTD Total Sales by Body Style:**
![YTDTotalSales](/Users/hansimgluck/Desktop/powerbi/303842583-2afe3465-c089-4a6c-96c5-99cb43f448a2.png)


**YTD Total Sales by Color:** 
![YTDTotalSalesByColor](/Users/hansimgluck/Desktop/powerbi/303842588-0864e0f0-3c0b-472a-a5c0-b6d00182ea39.png)


**YTD Cars Sold by Dealer Region:** 
![DealerRegion](/Users/hansimgluck/Desktop/powerbi/303842587-38574caf-6ce0-44cc-9760-75b516647d6c.png)


**Company-Wise Sales Trend in Grid Form:** 
![AllCarSales](/Users/hansimgluck/Desktop/powerbi/303842480-171f7629-8380-4f30-bf26-b44f13bad065.png)


**Details Grid Showing All Car Sales Information:** 
![details](/Users/hansimgluck/Desktop/powerbi/303842888-a2efe884-ad4d-4f66-b2a6-205b01120b4a.png)




## Done by
   - Mustafa Öztemiz
