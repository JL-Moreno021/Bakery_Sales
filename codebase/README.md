# Preliminary Investigation
    This section of the project focuses on understanding the structure of the data, its contents, and format

## Data Structure

**Shape:**

    Columns: 40
    Rows: 19321

**Data Types:**
| | |
---|---
Float|temperature, unit price, cost price, discount percentage, selling price, total bill, waste percentage, profit
Int|customer age, year, month, day, hour, quantity, shelf life days, units produced, units sold, unsold units, stock available, customer rating
String|order id, customer id, customer gender, customer segment, loyalty member, date, day of week, weekend, time, season, festival, weather, product, category, payment method, promotion applied, promotion type, storage type, perishability, store id

**_Variable Assumptions_**
Column|Assumption
---|---
Temperature| $C^o$ measure (Fahrenheit ($F^o$) and Kelvin $K$ results to negative temperature when converted to Celsius ($C^o$))
Currency| Rupee (₹) - Indian bakery found in Category

## Initial Findings
Column|Findings|Solution
---|---|---
Date|in string format|convert to datetime
Time|in string format|convert to datetime
Festival|16006 Missing values|Imput with "Unavailable"
Promotion Type|13826 Missing values|Imput with "Unavailable"
