# Model Equations

## Simple Regression Equations

Marketing model:
monthly_sales = 329230.43 + 3.84 * marketing_spend

Footfall model:
monthly_sales = 262941.18 + 19.77 * footfall

## Multiple Regression Equation

monthly_sales = 64063.28 + 2.89 * marketing_spend + 18.76 * footfall - 815.76 * avg_discount_pct + 1097.08 * inventory_availability_pct + 7698.33 * customer_rating + 25114.37 * region_North + 15485.42 * region_East + 16262.74 * region_West + 19273.91 * store_type_Mall

## Coefficient Explanation

Marketing spend, footfall, inventory availability, and customer rating have positive coefficients, meaning higher values are associated with higher expected monthly sales when other included variables are held constant. Average discount has a negative coefficient, suggesting heavier discounting may be linked to weaker underlying sales or lower realized value.

## Dummy Variables

Dummy variables were created for region and store_type. South is the reference category for region, so region_North, region_East, and region_West compare those regions against South. HighStreet is the reference category for store_type, so store_type_Mall compares Mall stores against HighStreet stores. One category is left out for each categorical variable to avoid redundancy.

## Final Model Selected

The multiple regression model is selected because it uses several business drivers together, includes dummy variables, and has the highest R-squared (0.9862).
