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

### **Visualization and Analysis in Power BI**

## **Key Findings**

1. **Overall Crime Statistics**

- A total of 5.83 million crimes were reported across 43 police counties and 332 cities in England and Wales in 2024.

- The Metropolitan Police Service recorded the highest number of crimes, reporting 1.14 million incidents, which accounted for approximately 19.5% of all reported crimes.

- Among cities, Birmingham (153K), Leeds (112K), and Westminster (105K) were identified as the top three cities with the highest number of reported crimes.

2. **Crime Categories and Trends**

- Violence and sexual offences constituted the largest category, with 1.99 million reported cases, making up 34% of all crimes.

- Anti-social behavior (895K), shoplifting (481K), and criminal damage & arson (437K) were the next most prevalent crimes.

- Theft-related offences, including shoplifting (481K), other theft (420K), and vehicle crime (341K), remain a significant concern.

- A relatively lower number of cases were recorded in categories such as possession of weapons (53K) and bicycle theft (56K).

3. **Monthly Crime Trends**

- Crime levels fluctuated throughout the year, with a peak in June (530K reported crimes).

- Other high-crime months included April (521K) and August (516K), suggesting possible seasonal influences.

- The lowest crime rate was observed in December (438K), potentially due to increased law enforcement presence during the holiday season.

4. **Geographic Distribution of Crime**

- London (Metropolitan Police Service) experienced the highest crime rate, accounting for nearly one-fifth of all reported crimes.

- Other high-crime counties included West Midlands Police (342K), West Yorkshire Police (309K), and Thames Valley Police (198K).

- Several cities and regions reported significantly lower crime levels, which may indicate effective law enforcement strategies or lower population density.

## **Conclusions**

- Urban areas are the primary hotspots for crime, with London, Birmingham, and Leeds reporting the highest number of incidents. This suggests a need for increased law enforcement presence and community engagement in these areas.

- Violence and sexual offences remain a critical concern, highlighting the necessity for targeted intervention programs, victim support services, and preventive measures.

- The spike in crime during summer months suggests the need for enhanced policing efforts during these periods to mitigate potential surges in criminal activity.

- Shoplifting, vehicle crime, and burglary pose persistent challenges, calling for improved security infrastructure, surveillance, and crime deterrence strategies.

## **Recommendations**

1. **Strategic Resource Allocation**: Increase police presence and community policing in high-crime urban areas, particularly in London, Birmingham, and Leeds.

2. **Enhanced Surveillance and Security Measures**: Implement additional CCTV surveillance and street lighting improvements in high-risk areas to deter criminal activity.

3. **Targeted Intervention Programs**: Develop specialized task forces to address violent crimes and anti-social behavior through proactive community engagement.

4. **Crime Prevention Campaigns**: Conduct awareness programs on crime prevention, particularly for shoplifting and vehicle-related crimes, to reduce victimization.

5. **Seasonal Policing Strategies**: Strengthen policing efforts during peak crime months (June, April, August) to curb potential spikes in criminal activities.

6. **Data-Driven Decision-Making**: Continue leveraging crime data analytics to assess crime patterns and enhance predictive policing strategies.

By implementing these recommendations, law enforcement agencies and policymakers can develop more effective crime prevention strategies, ensuring a safer and more secure environment for residents across England and Wales.
