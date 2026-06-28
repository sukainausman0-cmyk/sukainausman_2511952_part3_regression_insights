# Model Comparison

| Model name | Variables used | R-squared | Significant variables | Business usefulness | Limitations |
|---|---|---:|---|---|---|
| Simple Model 1 - Marketing Spend | monthly_sales ~ marketing_spend | 0.1276 | marketing_spend p=0.00021 | Shows sales rise as marketing spend increases. | Does not control for traffic, inventory, discount, region, or store type. |
| Simple Model 2 - Footfall | monthly_sales ~ footfall | 0.7794 | footfall p=0 | Shows customer traffic is strongly associated with sales. | Footfall may itself be caused by location, seasonality, campaigns, or store size. |
| Multiple Regression - Final Model | monthly_sales ~ marketing_spend + footfall + avg_discount_pct + inventory_availability_pct + customer_rating + region/store dummies | 0.9862 | Marketing, footfall, inventory, rating, discount, and selected dummies are most useful. | Best model because it compares drivers while holding other factors constant. | Association only; omits store size, competition, seasonality, and campaign quality. |

The multiple regression model is selected as the final model because it has the strongest explanatory power and provides the most useful business interpretation.
