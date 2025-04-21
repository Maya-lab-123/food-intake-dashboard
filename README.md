# Food Intake Dashboard

**Author:** Marzia Sevieri  
**Affiliation:** Data Technician Trainee, MSc Market Analytics & BSc Nutritional Sciences  
**Date:** April 2025

---

## Overview

This repository contains a Power BI dashboard designed to analyse daily food intake data for a sample of users, compared against UK reference intake values. The interactive report allows exploration of macronutrient and micronutrient consumption patterns, meal‑type breakdowns, and single‑item contributions to total energy intake.

## Repository Structure

```
├── Project_April.pbix                  # Power BI Desktop report file
└── Materials for the April final project/
    ├── data_exports/                  # Raw and processed CSV data files
    ├── screenshots/                   # Example visuals and annotations
    └── notes/                         # DAX formulas, methodology, and analysis notes
```

## Key Features

- **Daily Intake vs UK Reference**  
  Cards and gauge visuals showing grams and % of target for Carbs, Fat, Protein, Fibre, Sugar, Sodium, and total Calories.
- **Trend Analysis**  
  Line chart of average kcal intake per meal over the year.
- **Top Contributors**  
  Table listing food items by their kcal contribution and percentage of total intake.
- **Nutrient Intake by Meal Type**  
  
  - Stacked bar charts of macronutrients by food category for each meal type (Breakfast, Lunch, Dinner, Snacks).
  - Bar chart of sugar intake by category.
  - Distribution donut chart showing proportion of kcal by food category.

## Data Model

- **DimDate**: Calendar table with Date field.  
- **DimUser**: User dimension with User_ID.  
- **Food_Intakes**: Fact table of individual intake records including User_ID, Date, Meal_Type, Food_Item, Food_Category, and nutrient columns (Calories, Protein, Carbs, Fat, Fibre, Sugars, Sodium).  
- **Meal_Targets**: User-defined kcal targets per meal type.  
- **Nutrient_Targets**: Daily target values and % targets for each nutrient.

All tables are related on `User_ID` and `Date` keys.

## How to Use

1. Install Power BI Desktop (February 2025 or later).  
2. Open `Project_April.pbix`.  
3. Use the **Filters** pane to select date ranges and user IDs.  
4. Navigate the **Report** view to explore dashboards; view or adjust DAX measures in the **Data** view.

## Requirements

- Windows 10/11 or compatible OS  
- [Power BI Desktop](https://powerbi.microsoft.com/)  

## Contact

For questions or feedback:  
📧 marzia.sevieri@gmail.com

---

*Thank you for reviewing the Food Intake Dashboard!*

