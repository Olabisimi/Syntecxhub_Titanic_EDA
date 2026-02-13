# Syntecxhub_Titanic_EDA
Titanic dataset exploratory data analysis (EDA) including survival analysis by gender, class, age, lifeboat access, body recovered, and embarked port with charts and summary insights.

Exploratory Data Analysis (EDA) of the Titanic dataset to understand survival patterns.  
Analysis includes survival by gender, passenger class, age groups, body recovered, lifeboat access, and embarkation port with visualizations and summary insights.

## Analysis Steps

1. **Data Cleaning**
   - Renamed columns for clarity (e.g., Pclass → Passenger_Class, Sex → Gender)  
   - Handled missing values:
     - Age filled with median
     - Embarked filled with mode
   - Created new binary column `Body_Recovered` to indicate recovered bodies  
   - Dropped irrelevant columns (Ticket, Cabin, Home_Destination)  
   - Survival_Status updated to “Yes”/“No”

2. **Age Buckets** created for analysis:
   - Child (0–12), Teen (13–19), Adult (20–39), Middle_Aged (40–59), Senior (60+)

3. **Survival Analysis**
   - By Gender  
   - By Passenger Class  
   - By Age Group  
   - By Body Recovered  
   - By Boat (Access)  
   - By Embarked Port

4. **Visualization**
   - Stacked bar charts for categorical comparisons
   - 
5. **Export**
   - All visualizations saved as PNG  
   - Summary insights saved as Survival_Summary.txt
   - 
## Summary Insights

- **Gender:** Females had a substantially higher survival rate (~73%) compared to males (~19%).  
- **Passenger Class:** First Class passengers had the highest survival (~62%), Third Class the lowest (~26%).  
- **Age:** Children (0–12) survived more (~57%) than adults (~36%). Teens and Middle-Aged adults had moderate survival.  
- **Body Recovered:** Passengers with body recovered (1) did not survive; blanks (0) indicate survivors (~42% survival).  
- **Boat Access:** Lifeboat access greatly increased survival (~98% with access vs ~3% without).  
- **Embarked Port:** Survival varied slightly by port, with Cherbourg passengers (~56%) faring better than Southampton (~33%) and Queenstown (~36%).  

Overall, survival was strongly influenced by **gender, age, class, and lifeboat access**, confirming historical evacuation patterns on the Titanic.

## Usage

1. Open Titanic_EDA_Analysis.ipynb in Jupyter Notebook or Colab  
2. Ensure Titanic_Cleaned.csv is in the same folder  
3. Run all cells to reproduce analysis and generate charts in outputs

## Preview of Outputs

| Visualization | Description |
|---------------|-------------|
| `Survival_by_Gender.png` | Stacked bar chart of survival by gender |
| `Survival_by_Class.png` | Stacked bar chart of survival by passenger class |
| `Survival_by_AgeGroup.png` | Stacked bar chart of survival by age group |
| `Survival_by_BodyRecovered.png` | Survival rate by body recovered |
| `Survival_by_BoatAccess.png` | Survival rate by lifeboat access |
| `Survival_by_Embarked.png` | Survival rate by embarkation port |
| `Survival_Summary.txt` | Short textual summary of key insights |
