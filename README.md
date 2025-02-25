# UK_Crime_Statistics_2024

**Introduction**  

With crime prevention and law enforcement being top priorities, the recently appointed Police and Crime Commissioners (PCCs) of England and Wales require a comprehensive understanding of crime hotspots across their respective territories. This insight is crucial for the strategic allocation of resources, effective deployment of personnel, and the implementation of targeted crime reduction initiatives.  

To support data-driven decision-making in law enforcement, this project undertakes an in-depth analysis of crimes reported across various police jurisdictions in the UK—excluding Scotland and Northern Ireland—between January and December 2024. By leveraging crime data, this analysis aims to identify trends, patterns, and geographical concentrations of criminal activity, offering a robust foundation for policy formulation and resource optimization.  

Through data aggregation, visualization, and statistical modeling, this report highlights key crime categories, seasonal fluctuations, and high-risk areas, equipping PCCs with actionable intelligence to enhance public safety and community security.

**Data Source**

The dataset for this project was obtained from the **UK Police Data Bank**. [Access it here](https://data.police.uk/data/).  

The **2024 crime data** was structured into **12 folders**, each representing a month of the year. Within each folder, there were approximately **43 CSV files**, corresponding to the various police counties across **England and Wales**.  

In total, the dataset comprised **513 CSV files**, containing detailed records of crimes reported to the police across **England and Wales** throughout **2024**.

### **Data Exploration**  

The raw dataset, as downloaded, required extensive preprocessing to make it suitable for analysis. Several key aspects of the dataset are noteworthy:  

- The dataset comprises **513 CSV files**, each containing thousands of records, making it substantial in size.  
- All files share an identical structure, facilitating efficient cleaning and merging.  
- At least **four critical columns** hold the necessary data for this analysis.  
- The dataset includes more information than required, necessitating the removal of redundant columns to streamline the analysis.  

### **Data Cleaning**  

To ensure the dataset was properly structured and optimized for analysis, the following data cleaning steps were undertaken:  

- **Merging Files**: A Python script executed in **Google Colab** was used to seamlessly merge all **513 CSV files** into a single dataset.
![Python Script to merge the files](https://github.com/user-attachments/assets/bc0693ae-5f41-4b9e-9143-4f6b28d2dbfb)

- **Column Selection**: Only relevant columns were retained, eliminating unnecessary data.  
- **Data Type Validation**: Each column’s data type was assessed and adjusted to ensure consistency and appropriateness.  
- **Handling Missing Values**: All null values were addressed, resulting in a **complete dataset with no missing entries**.
- **Creating a new column for "City"**: I used a DAX formula to extract the city names from the "LSOA name" column
![DAX to get City Column](https://github.com/user-attachments/assets/ffad8441-ceca-4ad7-bc7d-08d59c91478f)



These preprocessing steps ensured a clean, well-structured dataset, primed for in-depth analysis and visualization.
