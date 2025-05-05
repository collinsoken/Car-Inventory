# Excel Data Analysis Project: Car Inventory

## **Project Overview**

This project involves cleaning, organizing, and analyzing a raw dataset of car inventory provided in a CSV file. The cleaned and analyzed data is presented in an Excel file. The goal was to transform the raw data into a structured and insightful format for better understanding and decision-making.

![Screenshot 2025-05-05 215432](https://github.com/user-attachments/assets/6c954da4-8791-4905-a244-9a8bd84231af)


### **Raw Data (CSV File)**

The raw dataset contained numerous issues, including:

- Missing values in key columns such as `Make`, `Model`, `Manufacture Year`, and `Miles/Year`.
- Lack of uniformity in data formatting.
- Absence of calculated fields like `Miles/Year` and `New Car ID`.
- Redundant or empty rows at the end of the dataset.


### **Cleaned Data (Excel File)**

The Excel file represents the cleaned and analyzed version of the dataset. Key improvements include:

1. **Data Cleaning:**
    - Filled missing values for columns like `Make`, `Model`, and `Manufacture Year` using logical inference or external references.
    - Removed redundant rows and unnecessary blank spaces.
    - Standardized column values for consistency (e.g., color names, driver names).
2. **Data Transformation:**
    - Calculated new fields:
        - **`Miles / Year`:** Derived by dividing total miles (`Miles`) by the car's age (`Age`).
        - **`New Car ID`:** Created by appending the first three letters of the car's color to its original ID for easier identification.
    - Added a `Covered?` column to indicate whether the car's mileage is within its warranty limit.
3. **Data Validation:**
    - Verified that all cars have valid entries for critical fields like `Manufacture Year`, `Miles`, and `Color`.
    - Ensured logical consistency between columns (e.g., cars with mileage exceeding warranty limits marked as "NO" in the `Covered?` column).
4. **Data Organization:**
    - Sorted data by relevant parameters such as manufacture year, mileage, or driver names for better readability.
    - Grouped cars by make and model to identify trends or patterns.

### **Techniques and Approaches**

The following steps were taken to ensure a high-quality analysis:

1. **Exploratory Data Analysis (EDA):**
    - Identified missing values, outliers, and inconsistencies in the raw dataset.
2. **Data Cleaning Tools:**
    - Used Excel functions like `IF`, `VLOOKUP`, `INT`, `YEAR`, string functions, and conditional formatting to clean and enrich the data.
3. **Data Transformation:**
    - Applied formulas to calculate derived metrics such as `Miles / Year`.
    - Generated unique IDs using string manipulation functions like `CONCATENATE`.
4. **Visualization:**
    - Created pivot table to summarize key insights, such as average mileage per year by car model and driving pattern for each driver.

### **Key Insights from Analysis**

- Cars older than 20 years tend to have higher mileage but are often out of warranty coverage.
- The average mileage per year varies significantly based on car model.
- Certain drivers operate cars with lower than average mileage per year, indicating potential use cases like short commutes.


### **Conclusion**

The Excel file provides a structured view of the car inventory with actionable insights derived from the raw data. This transformation highlights the importance of cleaning and analyzing data for better decision-making.

This project demonstrates proficiency in handling messy datasets, applying logical transformations, and presenting clean, insightful results using Excel tools.
