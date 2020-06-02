# Mod3Project-
Categorical Modeling 

# Goal
The goal of this project is to predict whether a well in Tanzania is functional or in need of repair.

# Target
functional = 0

functional and in need of repair = 1

non-functional = 2

# Predictors
amount_tsh,	gps_height,	installer,	longitude,	latitude,	basin,	region,	region_code,	district_code,	population,	public_meeting,	scheme_name	permit,	construction_year,	extraction_type,	payment,	water_quality,	quality_group	quantity,	quantity_group,	source,	waterpoint_type.	

# Data Cleaning
Our data clean, mostly we just had to drop Na's and change the types of our data so we can run it in our model. 

# Distribution of Target
https://lh6.googleusercontent.com/BOusAosgmri1koVSbwEQUj86ZqGl90NutQsNvINqlqxeWGnwdOSXWfceMCIyvrNEQzd6Pv27cWAuSL3kLPk5Qh22kCtazhmJJjbdSNof9EjesmDEVP6KbewMJsKrgsAZXg0hSIDM5BI

# Feature Engineering/ Feature Selection
Created a new feature that dictates how old the well is. Tanzania started keeping a record of all of their wells starting in 1960. All wells that were made before that we considered ancient and made the value 100 years old.

We used a MinMax Scaler to regularize all of our data.

Our Top 10 features ended up being
- Longtitude
- Latitude
- GPS Height
- Quantity
- Years Operational
- Payment Type
- Water Point Type
- Distric Code
- Amount Tsh: Amount of water available at water point
- Region
- Installer
- Permit

# Models
We tried multiple models, including Logistic Regression, Random forrest, Bagging, and XGBoost

# Conclusion
After running and gridsearching multiple models we found that the Random Forrest model was the best. Random Forrest happens to the best model because of how pure the differences were in our variables. Most the the wells that needed to be repaired fall into the same category

# Link to Presentation
https://docs.google.com/presentation/d/1mTiuE6NfeDh1VY0OvN6paSgPHz68cfbn2P-pr3vTtSA/edit#slide=id.g74636f51ab_2_50
