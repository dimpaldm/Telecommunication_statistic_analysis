# Telecommunication_statistic_analysis
This project analyzes a dataset of mobile phone specifications to extract insights related to screen resolution, memory, battery power, camera quality, and pricing. The goal is to perform statistical computations and visualize key features to support decision-making.
## Dataset Description
The dataset contains information about various phone models, including:

- **PID**: Phone ID

- **Blue**: Bluetooth availability (Yes/No)

- **Wi_Fi**: WiFi availability (Yes/No)

- **Tch_Scr**: Touchscreen availability (Yes/No)

- **Ext_Mem**: External memory support (Yes/No)

- **Px_h, Px_w**: Screen pixel height and width

- **Scr_h, Scr_w**: Screen height and width in physical units

- **PC, FC**: Primary and Front camera resolutions (in Megapixels)

- **Int_Mem**: Internal memory (in GB)

- **Bty_Pwr**: Battery power (in mAh)

- **RAM**: RAM capacity (in GB)

- **Depth, Weight**: Phone dimensions and weight

- **Price**: Phone price in currency units

## Key Analyses Performed

**1. Data Cleaning and Transformation**

- Converted categorical features (Yes/No) to numerical values (1/0).

- Created new features for analysis:

- Px (Total Screen Resolution) = Px_h * Px_w

- Scr_d (Screen Diagonal Size) using the Pythagorean theorem.

- Megapixels (Total Camera Resolution) = PC + FC

**2. Statistical Analysis**

- Calculated mean, median, and standard deviation for numerical features.

- Computed the coefficient of variation (std/mean) for all numerical columns.

**3. Logical Condition for selection**

- con2: Phones with screen resolution ≥ median resolution.

- con3: Phones with screen size ≥ upper quartile size.

- con4: Phones with camera resolution ≥ mean PC and FC.

- con5: Phones with memory, battery power, and RAM above mean or median thresholds.

**4. Data Visualization**

- Histograms with mean and median for:

- Screen Resolution (Px_h, Px_w)

- Screen Size (Scr_d)

- Camera Quality (PC, FC, Megapixels)

- Memory, Battery, and RAM

- Visualized the distribution of phone specifications to identify trends.

## How to Use##

Install dependencies if needed:

- pip install pandas matplotlib seaborn

Run the Jupyter Notebook (TelecommunicationData_StatisticAnalysis.ipynb).

Explore the insights and visualizations generated.

## Conclusion ##
This analysis helps in understanding the relationship between mobile specifications and pricing, guiding potential buyers or manufacturers in making informed decisions.

