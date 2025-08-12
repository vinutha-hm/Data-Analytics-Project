Crop Production Data Analysis

Overview:
This project analyzes Indian crop production trends using Python for exploratory data analysis (EDA) and Power BI for interactive dashboards.
The goal is to identify patterns in crop yield, area cultivated, and production across different states, districts, crops, and seasons over multiple years.

Project Structure:
bash
Copy
Edit

Crop-Production-Analysis
├── cleaned_crop_production.csv     # Cleaned dataset used for analysis
├── Crop_production_project.pbix    # Power BI dashboard file
├── notebooks/                      # Jupyter/Colab notebooks for EDA
├── README.md                       # Project documentation
└── requirements.txt                # Python dependencies

Dataset Description
File: cleaned_crop_production.csv

Column Name	Description
State_Name	Name of the state
District_Name	Name of the district
Crop_Year	Year of crop data
Season	Agricultural season (e.g., Kharif, Rabi)
Crop	Name of the crop
Area	Cultivated area (in hectares)
Production	Crop production quantity (in tonnes)

Analysis Workflow
Python EDA & Visualization
Tools: pandas, matplotlib, seaborn, plotly
Steps:
Loaded dataset from CSV.
Checked for missing/null values and ensured data consistency.
Extracted useful features (e.g., Year, Season, State-wise summaries).

Visualized:
Year-wise crop production trends
Seasonal production patterns
Top 10 crops by production
State-wise crop production distribution
Power BI Dashboard
Imported cleaned dataset.

Created measures:
Total Production = SUM(Production)
Total Area = SUM(Area)
Average Yield = DIVIDE(SUM(Production), SUM(Area))

Visuals:
Production trends by year
Top producing crops
Seasonal production share
State-wise production map

Filters: State, Year, Season, Crop

Key Insights:
Identified top producing states for major crops.
Found seasonal variations in production.
Highlighted crops with highest and lowest yields.
Compared production efficiency across states.

Tech Stack:
Python → Pandas, Matplotlib, Seaborn, Plotly
Power BI → Interactive dashboards, DAX measures
CSV → Data storage

Usage
Python
bash
Copy
Edit
git clone https://github.com/yourusername/Crop-Production-Analysis.git
cd Crop-Production-Analysis
pip install -r requirements.txt
jupyter notebook notebooks/eda.ipynb
Power BI
Open Crop_production_project.pbix in Power BI Desktop.

Interact with slicers and filters to explore data.

Future Work:
Integrate rainfall and climate data for deeper insights.

Build ML models to predict future crop yields.

Automate dashboard updates with live data sources.
