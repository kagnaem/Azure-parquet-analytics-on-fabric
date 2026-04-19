# Dashboard Summary and Business Insights

This document focuses only on the final Power BI dashboards. It explains the headline KPIs, the main chart patterns, and the business meaning of the results. It is intentionally shorter and more presentation-focused than the full project README and the notebook.

## Dashboard Scope
The dashboard summarizes **6 months of NYC yellow taxi trip data from 2019** prepared through the Bronze -> Silver -> Gold workflow in Microsoft Fabric.

## Headline Figures
- **Total Revenue:** 931,794,015.82
- **Total Trips:** 51,538,953
- **Average Fare:** 12.87
- **Average Trip Distance:** 2.96
- **Average Tip Amount:** 2.10
- **Average Trip Duration:** 14.04 minutes
- **Average Revenue Per Mile:** 11.24

## Operational Summary: What the Main Charts Show

### 1. Total Revenue by Pickup Date
Revenue peaks strongly in the early part of the period and then settles into a lower but stable range. This suggests that demand or pricing conditions were unusually strong at the beginning of the selected window, followed by a more consistent operating pattern across the remaining months.

### 2. Total Trips by Pickup Date
Trip volume follows a similar pattern: a very high early period followed by a drop and then a relatively steady trend. This indicates that activity remains resilient even after the initial surge fades.

### 3. Total Revenue by Pickup Weekday
Weekday revenue is strongest late in the workweek:
- **Thursday:** about 152M
- **Friday:** about 146M
- **Wednesday:** about 144M
- **Tuesday:** about 136M
- **Saturday:** about 125M
- **Monday:** about 118M
- **Sunday:** about 112M

This shows that Thursday and Friday are the most valuable days in revenue terms, while Sunday performs the weakest.

### 4. Total Trips by Pickup Weekday
Trip counts follow a similar pattern:
- **Thursday:** about 8.2M trips
- **Friday:** about 7.9M trips
- **Wednesday:** about 7.9M trips
- **Tuesday:** about 7.5M trips
- **Saturday:** about 7.3M trips
- **Monday:** about 6.4M trips
- **Sunday:** about 6.3M trips

The similarity between weekday revenue and weekday trip counts suggests that overall revenue is driven largely by demand volume rather than only by large changes in average trip value.

### 5. Total Revenue by Payment Type
Revenue is heavily concentrated in card-based transactions:
- **Credit card:** about 717.55M, roughly **77.01%**
- **Cash:** about 208.13M, roughly **22.34%**
- **No charge / Dispute:** very small share

This implies that digital payment behavior dominates the revenue profile of the selected period.

### 6. Total Trips by Payment Type
Trip counts also show payment concentration:
- **Credit card:** about 37M trips, roughly **72.58%**
- **Cash:** about 14M trips, roughly **26.95%**
- **No charge / Dispute:** very small share

The payment mix reinforces the idea that card usage is the standard operating mode for the majority of rides.

## Forecast Dashboard: What It Means

### Trips Forecast
The trips forecast suggests short-term stabilization around the recent lower range rather than a return to the very high early-period levels. The widening confidence band shows increasing uncertainty as the forecast extends outward.

### Revenue Forecast
Revenue forecasting follows a similar pattern. The model suggests revenue is likely to remain around its recent operating range in the short term, but the widening forecast interval means the projection should be interpreted as directional rather than exact.

## Key Takeaways
- **Credit card payments dominate the business**, both in total trips and in total revenue.
- **Thursday and Friday are the strongest days** for taxi activity and revenue generation.
- **Sunday is the weakest day** in both revenue and trip volume.
- **The business shows an early peak followed by stabilization**, rather than continuous decline.
- **Revenue and trip patterns move together**, which suggests that demand volume is the main driver of business performance in this period.
- **Forecasting supports short-term planning**, but the uncertainty range means it should be treated as a guide rather than a precise prediction.

## Business Conclusion
From an operational perspective, the dashboard suggests that the taxi business in this 6-month window is driven by strong weekday demand, especially late in the workweek, and by a customer base that relies primarily on credit card payments. The pattern of stabilization after the initial peak indicates a mature and relatively steady operating environment. For decision-making, this means resource planning, service readiness, and revenue monitoring should focus especially on midweek and late-week performance, while forecasting should be used for short-term trend direction rather than long-range certainty.

## Reference
This summary is based on the final dashboard outputs included in the project PDF:
- `docs/Quick summary NYC Taxi.pdf`
