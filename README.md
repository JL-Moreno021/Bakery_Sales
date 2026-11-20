# Bakery Sales Project

## [Bakery Sales, Customer & Inventory Analytics Datas](https://www.kaggle.com/datasets/sdcloud/historical-bakery-sales-dataset)
    Synthetic two-year bakery retail dataset for sales analysis, demand forecasting

### Project Data
>---
[Data Dictionary](Data_Dictionary.md) 

#### Transaction Information
* Order ID, Customer ID, Store ID, Date, Time, Product, Quantity, Discount Percentage, Promotion Type, Customer Rating

#### Customer Information
* Customer ID, Age, Gender, Segment, Loyalty Member

#### Branch Table
* Store ID, Date, Product, Units Produced, Stock Available

#### Product Table
* Product, Category, Unit PRice, Cost Price, Shelf Life Days, Storage Type, Peroshability

#### Factors Table
* Date, Season, Festival, Weather, Temperature

#### Derived Values
|Column|Values|
---|---
Date|Year, Month, Day<br>Day of Week, Weekend
Time|Hour
Selling Price| (Unit Price - Cost Price) * Quantity
Total Bill|Selling Price * Quantity
Promotion Applied|Discount Percentage > 0
Units Sold| SUM(Quantity)
Unsold Units|Units Produced - Units Sold
Waste Percent| (Unsold Unit / Units Produced) * 100
Profit|Total Bill - (Cost Price * Quantity)
>---