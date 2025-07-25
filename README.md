# Los-Angeles-Crime-Analysis


[Dataset source](https://www.kaggle.com/datasets/hemil26/crime-in-los-angeles/data?select=crime_in_la.csv)

# GOAL
  The goal of this project is to uncover insights and trends in the los angeles crime dataset from 2020-2024

# Columns in the dataset
    DR_NO
    Division of Records Number: Official file number made up of a 2 digit year, area ID, and 5 digits
  
  
    DATE OCC
    Date the crime occurred in MM/DD/YYYY format.
  
    TIME OCC
    In 24 hour time.
  
    AREA
    The LAPD has 21 Community Police Stations referred to as Geographic Areas within the department. These Geographic Areas are sequentially numbered from 1-21.
  
    AREA NAME
    The 21 Geographic Areas or Patrol Divisions are also given a name designation that references a landmark or the surrounding community that it is responsible for. For example 77th Street Division is located at the intersection of South Broadway and 77th Street, serving neighborhoods in South Los Angeles.

    Rpt Dist No
    Reported district number.
  
    
    Crm Cd
    Crime code. 
  
    Crm Cd Desc
    Defines the Crime Code provided.
    
    Mocodes
    Modus Operandi: Activities associated with the suspect in commission of the crime.See attached PDF for list of MO Codes in numerical order.
    
    Vict Age
    Victim's Age.
  
    Vict Sex
    Victim's gender.
    F - Female
    M - Male
    X - Unknown
    H - Undefined in dataset source
  
    
    Vict Descent
    Descent Code:
    A - Other Asian
    B - Black
    C - Chinese
    D - Cambodian
    F - Filipino
    G - Guamanian
    H - Hispanic/Latin/Mexican
    I - American Indian/Alaskan Native
    J - Japanese
    K - Korean
    L - Laotian
    O - Other
    P - Pacific Islander
    S - Samoan
    U - Hawaiian
    V - Vietnamese
    W - White
    X - Unknown
    Z - Asian Indian
  
    
    Premise Desc
    The type of structure, vehicle, or location where the crime took place.

    Weapon Used Cd
    The code of the weapon used.
    
    Weapon Desc
    Defines the Weapon Used Code provided.
    
    Status
    Status of the case.
    
    Status Desc
    Defines the Status Code provided.
    Invest Cont - Investigation Continuing – Case is still open or under investigation.
    Adult Arrest - An adult was arrested for the crime.
    Juvenile Arrest - A juvenile was arrested in relation to the case.
    Adult other - Case involving adult was resolved through other means.
    Juvenile other - Case involving juvenile was resolved through other means.
    UNK - Unknown
    
    LOCATION
    Street address of crime incident rounded to the nearest hundred block to maintain anonymity.
  
  
    LAT
    Latitude coordinate
    
    LON
    Longtitude coordinate

    

# OBJECTIVES

## Load and clean dataset
  * Load the dataset
  * Replace missing values and invalid entries in columns if any
  * Drop duplicates if any 
  * Drop columns not needed for analysis
  * convert date column to datetime format
    


## Area Summary
  * Create a summary DataFrame showing the the total number of crimes, average victim age, most common location and most common crime by area.
  * Visualize the total crimes and the average victim age by area
  * Top/Bottom crimes
    * Get the top and bottom 5 crimes then visualize
  * Crime Resolution
    * Resolution status: Calculate the resolution rates of crimes per area and visualize
    * Comparison by crime type: Identify which crime types have the highest/lowest resolution rates and visualize
    * District area performance: Create a DataFrame ranking districts by resolution rate, alongside total crime counts.


## Demographic Analysis
  * Victim age group
  * Create a summary dataframe showing the number and percentage of crimes affecting age groups
  * Visualize the above data
  * Victim Gender
    * Create a summary dataframe showing the number and percentage of crimes affecting genders
    * Visualize the above data
  * Victim Descent
    * Create a summary dataframe showing the number and percentage of crimes affecting different descent
    * Visualize the above data


## Time/Season Analysis
  * Hourly Analysis: Group crimes by hours, calculate average crime count 
  * Day-of-Week Analysis: Group crimes by day of the week (Monday–Sunday) to identify patterns. Calculate average crime counts per day, create a summary dataframe and visualize.
  * Seasonal Trends: Group data by season (e.g., Winter: Dec–Feb, Spring: Mar–May, etc.) to compare crime average crime counts among seasons.
  * Holiday Spikes: Compare crime count on holidays vs. non-holidays.




