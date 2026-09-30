# Causal Forest Estimation of Cash Transfers & Caloric Intake (PROGRESA)

## Objective
This project investigates heterogeneous treatment effects of the Mexican PROGRESA cash transfer program on household caloric intake. The analysis uses causal forests to examine whether treatment effects vary systematically across households with different baseline characteristics, moving beyond average treatment effects and standard OLS interaction models.


## Data & Methodology
* **Data Source:** Experimental evaluation data from the Mexican PROGRESA program (retrieved from the Harvard Dataverse).
* **Method:** Generalized Random Forests (Athey, Tibshirani, and Wager, 2019) implemented via the `grf` package in R.
* **Estimand:** Conditional Average Treatment Effects (CATEs) 
* **Core Question:** Do the effects of cash transfers on household caloric consumption vary systematically with baseline household constraints and characteristics?


## Repository Structure
* `/scripts`: R scripts for data cleaning, exploratory analysis, causal forest tuning, estimation, and variable-importance analysis
* `/output`: Figures and outputs showing the estimated distribution of treatment effects and heterogeneous treatment profiles.


## Requirements
The analysis is conducted in R using the following main packages:

    grf
    tidyverse
    ggplot2

Install the required packages with:
install.packages(c("grf", "tidyverse", "ggplot2"))


## Reproducibility 

Run the scripts in `/scripts` in the indicated order to reproduce the data preparation, model estimation, and visualizations.


## Reference 
Athey, S., Tibshirani, J., & Wager, S. (2019). Generalized Random Forests. The Annals of Statistics, 47(2), 1148–1178.
