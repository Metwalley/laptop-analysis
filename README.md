# Laptop Price Analysis

## Project Overview
This project focuses on cleaning and analyzing a dataset of laptops, aiming to extract meaningful insights about pricing, specifications, and trends. The dataset contains 1,303 laptop entries with details such as brand, specifications, and price.

## Dataset
- **Source:** Provided dataset (`laptop_data.csv`)
- **Size:** 1,303 rows, 12 columns
- **Key Features:**
  - `Company`, `TypeName`, `Inches`, `ScreenResolution`, `Cpu`, `Ram`, `Memory`, `Gpu`, `OpSys`, `Weight`, `Price`

## Data Cleaning
The dataset underwent the following preprocessing steps:
1. **Dropped Unnecessary Columns**
   - Removed `Unnamed: 0` as it was an index column.
2. **Screen Resolution Processing**
   - Extracted `Resolution_Width` and `Resolution_Height` from `ScreenResolution`.
3. **CPU Processing**
   - Split `Cpu` into `CPU Brand`, `CPU Series`, and `CPU Frequency`.
4. **RAM Standardization**
   - Converted `Ram` values from string (e.g., "8GB") to integer (e.g., `8`).
5. **Storage Processing**
   - Extracted `Storage Capacity` (converted TB to GB for consistency).
   - Extracted `Storage Type` (HDD, SSD, Hybrid, Flash Storage, etc.).
6. **GPU Processing**
   - Split `Gpu` column into `Gpu_Brand` and `Gpu_Model`.

## Analysis & Insights
- **Feature Correlations:** Explored relationships between specifications and price.
- **Brand Analysis:** Investigated how different brands position their laptops in the market.
- **Storage vs. Price:** Evaluated the impact of storage type and capacity on pricing.
- **Resolution & Screen Size Impact:** Analyzed how display features correlate with cost.

## Technologies Used
- **Languages:** Python
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Regex

## Usage
### Installation
Ensure you have the required dependencies installed:
```bash
pip install pandas numpy matplotlib seaborn
```

### Running the Notebook
Execute the Jupyter Notebook:
```bash
jupyter notebook laptop_data.ipynb
```

## Results & Findings
The analysis provides insights into pricing trends based on specifications, allowing better decision-making for consumers and manufacturers.

## Future Improvements
- More advanced feature engineering for predictive modeling.
- Visualizations to enhance understanding of price distribution.

## Author
Developed as part of a data cleaning and analysis project.
