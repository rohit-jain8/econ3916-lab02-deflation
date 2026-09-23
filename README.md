# econ3916-lab02-deflation
Deflating Economic Data — Nominal vs. Real

Objective

Analyze how inflation changes the interpretation of wages and consumer prices by converting nominal economic series into constant 2020 dollars.

Methodology

Pulled monthly Consumer Price Index and average hourly earnings data from FRED's public CSV endpoint with pandas.

Built a reusable deflate_series() function to convert nominal values into constant-dollar values using annual-average CPI.

Aligned semiannual Big Mac observations with the most recent available monthly CPI using .asof().

Compared nominal and inflation-adjusted wage and Big Mac price trends with matplotlib.

Built an interactive ipywidgets explorer for changing the base year and switching between nominal and real series.

Key Findings

Nominal average hourly earnings increased from $2.50 in January 1964 to $32.53 in August 2026.

In constant 2020 dollars, average hourly earnings increased much more modestly, from approximately $20.92 to $25.20.

From April 2000 to July 2026, the US Big Mac price increased approximately 178% in nominal terms but only 43% in real terms; CPI increased approximately 95% over the same dates.

Changing the base year rescales the level of a real series but does not change its growth rate.
