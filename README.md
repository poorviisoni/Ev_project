# Electric Vehicle Market Performance & Insights

**Capstone project \| Data Analytics with Tableau**

This project explores an electric-vehicle (EV) market dataset and
presents its patterns through Tableau visualizations and an interactive
dashboard. The analysis focuses on manufacturer sales, vehicle
categories, battery technologies, driving range, customer ratings,
manufacturing countries, and estimated environmental indicators.

> **Dataset notice:** The Kaggle dataset used for this project is
> synthetically generated. Results in this repository describe the
> supplied dataset only and should not be interpreted as verified
> real-world EV market statistics.

## Project objectives

-   Explore and prepare the supplied EV dataset for analysis.
-   Compare annual sales across manufacturers and vehicle categories.
-   Examine the distribution of battery technologies.
-   Compare average driving range across vehicle categories.
-   Review customer ratings and manufacturing-country patterns.
-   Present the findings in a Tableau dashboard.

## Tools and technologies

-   **Tableau Public / Tableau** --- data visualization and dashboard
    development.
-   **CSV** --- source data format.
-   **Kaggle** --- dataset source.
-   **GitHub** --- project file storage and sharing.

## Dataset

The project uses the **Electric Vehicle Market Classification Dataset**
from Kaggle.

The downloaded archive included:

-   `ev_market_train.csv` --- 200,000 rows and 37 fields; used as the
    primary analysis file.
-   `ev_market_test.csv` --- 100,000 rows and 37 fields; retained
    separately.

Relevant fields include:

-   `manufacturer`
-   `manufacturing_country`
-   `market_region`
-   `category`
-   `battery_type`
-   `battery_capacity_kwh`
-   `range_km`
-   `price_usd`
-   `annual_sales_units`
-   `customer_rating`
-   `co2_saved_tons_per_year`

Check the dataset's Kaggle licence and terms before redistributing the
raw data in a public repository.

## Data preparation

The training CSV was connected to Tableau. Field types were reviewed so
that categorical fields could be used as dimensions and numeric fields
as measures.

The original `price_usd` field should remain a decimal number to
preserve cents. A separate rounded calculated field can be created in
Tableau when whole-number display is needed:

``` text
ROUND([Price Usd], 0)
```

Missing values should be investigated rather than automatically replaced
with zero.

## Dashboard contents

The Tableau dashboard presents summary KPI cards and comparisons,
including:

-   Total manufacturers
-   Total models
-   Total sales
-   Average customer rating
-   Average driving range
-   Sales by vehicle category
-   Manufacturer market-share comparison
-   Customer rating by category
-   Battery-type distribution
-   Sales trend by model year
-   Sales by manufacturing country

Filters shown in the dashboard allow users to explore the data by
category, manufacturer, and manufacturing country.

## Key findings from the training dataset

The following are dataset-level observations calculated from
`ev_market_train.csv`:

1.  **Manufacturer sales:** AmpereWorks has the highest total
    `annual_sales_units` in the training file.
2.  **Vehicle category:** Two-Wheeler Scooter has the highest category
    sales total in the training file.
3.  **Battery technology:** NMC is the most frequent battery type in the
    training file, followed by LFP.
4.  **Driving range:** Luxury Sedan has the highest average `range_km`
    among the vehicle categories.
5.  **Customer rating and environmental indicator:** The overall mean
    customer rating is approximately 4.09/5. Electric Bus has the
    highest category-average value for `co2_saved_tons_per_year` in this
    file.

These observations are based on synthetic records and are not claims
about actual global sales, market share, or measured real-world
emissions reductions.

## Repository contents

Add or maintain the following files in this repository as they become
available:

``` text
ev_market_dashboard/
├── README.md
├── Tableau/
│   └── EV_Market_Dashboard.twbx
├── Dataset/
│   └── ev_market_train.csv
├── Documentation/
│   └── EV_Market_Performance_Insights_Project_Report.docx
└── Screenshots/
    └── dashboard.png
```

The folder names above are a suggested organization. Update the paths
and filenames to match the files actually committed to this repository.
Do not upload the dataset publicly unless its licence and your project
rules permit it.

## How to view the project

1.  Open the packaged Tableau workbook (`.twbx`) using a compatible
    version of Tableau.
2.  If the workbook asks for a data connection, follow Tableau's prompts
    and reconnect the supplied CSV file.
3.  Explore the dashboard using its filters.
4.  Review the project report for the development process and findings.

## Project links

-   **GitHub repository:**
    https://github.com/en25cs3010676-source/ev_market_dashboard
-   **Tableau workbook:** See the packaged workbook in the repository.
-   **Demo video:** Add the shareable demo-video link here after
    recording and uploading it.

## Author

**Piyush Verma**

BTech Capstone Project --- Electric Vehicle Market Performance &
Insights

------------------------------------------------------------------------

*Before final submission, verify that the workbook, report, screenshots,
and any permitted dataset files are present in the repository. Replace
the demo-video placeholder with your actual link.*
