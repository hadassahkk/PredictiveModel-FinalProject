# Predictive Modeling for Apartment Selling Prices in Queens, NY

## Overview
This repository contains the final project for Math 342W Data Science at Queens College. The project aims to develop a predictive model for apartment selling prices in Queens, NY, specifically focusing on condos and co-ops priced up to $1 million. Utilizing data from the Multiple Listing Service (MLS), this model seeks to offer more accurate predictions than those provided by platforms like Zillow.

## Abstract
The objective of this project is to predict apartment selling prices in Queens, NY. By employing extensive data cleaning, feature engineering, and the application of several machine learning techniques such as OLS, regression trees, and random forests, this project provides insights into the factors influencing apartment prices in this region. Among the techniques explored, the random forest model was found to be the most effective.

## Data
The data for this study was sourced from MLS, harvested through Amazon’s MTurk, comprising 2,330 entries initially, focusing on apartment sales in Queens from February 2016 to February 2017. After cleaning and preprocessing, the dataset was narrowed down to 528 observations with 23 columns, which included both categorical and numeric features.

## Featurization
Significant transformations were applied to the dataset to enhance its usability in modeling:
- **Binning and Categorization**: For instance, the 'approx year built' was binned into 20-year periods, and categorical factors were created for features like kitchen type and fuel type.
- **Binary Columns**: Columns for features such as 'cats allowed' and 'dogs allowed' were transformed into binary factors.
- **Seasonal Variations**: The 'season of sale' column was created to capture the impact of seasonal variations on apartment prices.

## Modeling Techniques
Three main modeling techniques were used:
1. **Regression Tree Modeling**: Identified key predictors such as square footage, number of full bathrooms, and co-op/condo status.
2. **Linear Modeling**: Provided a straightforward statistical approach to predict selling prices using features like square footage and location coordinates.
3. **Random Forest Modeling**: Emerged as the most effective model, handling complex interactions between features without needing a pre-defined structure.

## Performance Results
The models were evaluated using R² and RMSE metrics. The random forest model displayed superior out-of-sample accuracy, indicating its robustness and reliability for predictive purposes.

## Discussion
The models provided insightful results into apartment pricing dynamics in Queens. However, the performance could be enhanced with more comprehensive data. Future research should focus on gathering more complete datasets and exploring more sophisticated feature engineering and modeling techniques.

## References
- Eric Hurst, US ZIP Code Latitude and Longitude, (2013). [GitHub repository](https://gist.github.com/erichurst/7882666)

## Code
The project includes various R scripts for data loading, cleaning, and modeling. Detailed instructions and code can be found in the repository.
