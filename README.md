# 🍔 Food Calories & Workout Burn Analysis Dashboard

## 📊 Project Overview

The **Food Calories & Workout Burn Analysis Dashboard** is an
interactive Power BI project designed to analyze the nutritional content
of fast-food meals and understand the relationship between calorie
consumption, customer demographics, and physical activity.

The dashboard provides insights into calories, macronutrients, fast-food
chains, customer age groups, and estimated workout time required to burn
consumed calories.

## 🎯 Project Objectives

-   Analyze calorie consumption across different fast-food chains.
-   Compare nutritional values such as protein, carbohydrates, fat,
    sugar, and sodium.
-   Explore food consumption patterns across customer demographics.
-   Understand the relationship between calorie intake and net caloric
    surplus.
-   Compare estimated calorie-burning time across different physical
    activities.
-   Provide interactive insights using Power BI visualizations and
    filters.

## 🛠️ Tools & Technologies

-   **Power BI Desktop** -- Dashboard development and data visualization
-   **Power Query** -- Data loading and transformation
-   **DAX** -- Measures and calculations
-   **CSV** -- Dataset format

## 📁 Dataset

The dashboard is designed around the `fast_food_cheat_meal_workout_burn`
dataset.

Key fields include:

  -----------------------------------------------------------------------
  Category                            Fields
  ----------------------------------- -----------------------------------
  Order information                   `order_id`, `fast_food_chain`,
                                      `meal_category`, `item_count`

  Calories                            `total_calories`,
                                      `thermic_effect_calories`,
                                      `net_caloric_surplus`

  Nutrition                           `fat_grams`, `saturated_fat_grams`,
                                      `carb_grams`, `sugar_grams`,
                                      `protein_grams`, `sodium_mg`

  Customer details                    `consumer_gender`, `consumer_age`,
                                      `consumer_weight_kg`,
                                      `fitness_level`

  Workout estimates                   `walking_burn_time_min`,
                                      `cycling_burn_time_min`,
                                      `running_burn_time_min`,
                                      `hiit_burn_time_min`

  Additional metric                   `daily_calorie_allowance_pct`,
                                      `workout_shock_tier`
  -----------------------------------------------------------------------

*Note: Actual dataset size and numerical findings are not stated here
because they have not been verified from the source data.*

## 📈 Dashboard Features

### 1. Nutritional Analysis

-   Total calories consumed
-   Total protein, carbohydrates, fat, and sugar
-   Nutritional comparison across food categories

### 2. Fast-Food Chain Analysis

-   Total calories by fast-food chain
-   Protein and sugar comparison by chain
-   Customer order distribution

### 3. Customer Demographics

-   Food consumption by age
-   Gender-based analysis
-   Fitness-level filtering
-   Meal-category filtering

### 4. Calorie & Workout Analysis

-   Calories compared with net caloric surplus
-   Estimated walking, cycling, running, and HIIT burn times
-   Workout shock tier comparison

## 📊 Dashboard Visualizations

The Power BI report includes:

-   KPI-style metric cards
-   Bar and column charts
-   Line charts
-   Scatter plots
-   Stacked area charts
-   Detailed data tables
-   Interactive slicers

### Interactive Filters

Users can filter the report by:

-   Fast Food Chain
-   Meal Category
-   Gender
-   Fitness Level

## 🧮 DAX Measures

The template includes measures for the following calculations:

``` dax
Total Calories =
SUM('FOOD & CUSTOMER'[total_calories])
```

``` dax
Total Protein =
SUM(fast_food_cheat_meal_workout_burn[protein_grams])
```

``` dax
Total Carbs =
SUM(fast_food_cheat_meal_workout_burn[carb_grams])
```

``` dax
Total Fat =
SUM(fast_food_cheat_meal_workout_burn[fat_grams])
```

``` dax
Total Sugar =
SUM(fast_food_cheat_meal_workout_burn[sugar_grams])
```

``` dax
Total Orders =
DISTINCTCOUNT(fast_food_cheat_meal_workout_burn[order_id])
```

## 🚀 How to Use This Project

1.  Download or clone this repository.
2.  Open `Food Calories Dashboard.pbit` using Power BI Desktop.
3.  When prompted, connect the source data or update the data source to
    your dataset.
4.  Confirm that the imported table and column names match the model.
5.  Apply the changes and refresh the data.
6.  Explore the dashboard using the interactive slicers and charts.

**Important:** A `.pbit` file is a Power BI template, not a regular
exported dashboard or a CSV dataset. You need to connect the source data
before the report can display populated results.

## 💡 Key Business Questions

-   Which fast-food chain contributes the highest calorie intake?
-   Which food categories contain more fat, sugar, and protein?
-   How does calorie consumption vary by customer age and gender?
-   What is the relationship between calories consumed and net caloric
    surplus?
-   How much estimated exercise time is required to burn the calories
    consumed?

## 🎓 Skills Demonstrated

-   Data Visualization
-   Business Intelligence
-   Power BI Dashboard Development
-   Data Modeling
-   DAX Measures
-   Power Query
-   Data Analysis
-   Interactive Reporting

## 👨‍💻 Author

**Muhammed Nihal**

Aspiring Data Analyst \| Data Science Enthusiast

------------------------------------------------------------------------

⭐ If you find this project useful, feel free to star the repository!
