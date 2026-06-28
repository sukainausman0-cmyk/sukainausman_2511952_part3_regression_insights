# Residual Analysis

Residual = actual monthly_sales minus predicted monthly_sales from the selected multiple regression model.

## Largest Positive Residuals

| Store | Month | Region | Store type | Actual sales | Predicted sales | Residual |
|---|---|---|---|---:|---:|---:|
| S004 | 2026-04 | West | HighStreet | 383470 | 376745 | 6725 |
| S045 | 2026-09 | North | Suburban | 453667 | 446992 | 6675 |
| S069 | 2026-09 | North | Suburban | 428908 | 422441 | 6467 |
| S093 | 2026-09 | North | Suburban | 416630 | 410206 | 6424 |
| S033 | 2026-09 | North | Suburban | 397297 | 391320 | 5977 |

These stores performed better than expected. Possible reasons include local events, stronger store execution, better product mix, or promotional activity not captured in the dataset.

## Largest Negative Residuals

| Store | Month | Region | Store type | Actual sales | Predicted sales | Residual |
|---|---|---|---|---:|---:|---:|
| S085 | 2026-01 | North | HighStreet | 464229 | 474672 | -10443 |
| S013 | 2026-01 | North | HighStreet | 387176 | 396653 | -9477 |
| S043 | 2026-07 | East | HighStreet | 405157 | 414145 | -8988 |
| S019 | 2026-07 | East | HighStreet | 417436 | 426379 | -8943 |
| S061 | 2026-01 | North | HighStreet | 374288 | 382905 | -8617 |

These stores underperformed relative to model expectations. Leadership should review stockouts, staffing execution, competitor activity, local demand shifts, and whether high discounts are masking weak conversion. Residuals are investigation leads rather than proof of operational failure.
