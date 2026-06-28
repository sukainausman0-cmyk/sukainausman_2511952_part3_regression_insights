# Part 3: Regression-Based Business Insights & Model Interpretation

## Business Problem Summary

A retail leadership team wants to understand which factors are associated with monthly sales performance across stores. The goal is to support decisions about marketing spend, inventory availability, discounting, staffing, and store prioritization.

## Dataset Description

The dataset is stored in `data/business_regression_data.xlsx`. It contains store-month records with region, store type, marketing spend, footfall, discount percentage, inventory availability, customer rating, staff count, and monthly sales.

## Variables

Dependent variable: `monthly_sales`.

Potential independent variables: `marketing_spend`, `footfall`, `avg_discount_pct`, `inventory_availability_pct`, `customer_rating`, `staff_count`, `region`, and `store_type`.

Numerical variables: marketing spend, footfall, average discount percentage, inventory availability percentage, customer rating, staff count, and monthly sales.

Categorical variables: region and store type.

Variables that may need transformation: region and store type require dummy variables. Percent variables should be checked for consistent numeric formatting.

Variables that may be less useful: store_id and month are identifiers/time labels for this basic model and are not used directly as regression predictors.

## Regression Approach

Two simple regressions were created with `monthly_sales` as the dependent variable: one using marketing spend and one using footfall. A multiple regression model was then created using marketing spend, footfall, discount percentage, inventory availability, customer rating, and dummy variables.

## Dummy Variable Approach

Dummy variables were created for region and store type. South is the reference region. HighStreet is the reference store type. Reference categories are excluded to avoid redundancy.

## Model Comparison Summary

The multiple regression model has the strongest explanatory power and is selected as the final model. It is more useful than the simple models because it evaluates several drivers at the same time.

## Final Model Selected

Final model: multiple regression using marketing spend, footfall, average discount percentage, inventory availability percentage, customer rating, region dummies, and store type dummy variables.

## Business Recommendation

Leadership should focus on increasing qualified footfall, improving inventory availability, and using marketing spend where it is likely to generate measurable traffic. Discounting should be used carefully because the regression does not show it as a simple positive sales driver.

## Assumptions and Limitations

Regression identifies association, not automatic causation. The model does not include store size, local competition, product mix, campaign quality, weather, or seasonality. Results should be validated through business experiments before major spending decisions.

## Screenshots Included

- `screenshots/simple_regression_output.png`
- `screenshots/multiple_regression_output.png`
- `screenshots/residuals_preview.png`
- `screenshots/model_comparison_preview.png`
