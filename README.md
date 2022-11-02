# 2022 Uganda Ebola outbreak

## Contents

This repository contains data extracted from the [ECDC surveillance](https://www.ecdc.europa.eu/en/ebola-virus-disease-outbreak-uganda) and [Ministry of Health, Uganda](https://twitter.com/MinofHealthUG) bulletins in collaboration with the [World Health Organization - Regional Office for Africa (WHO AFRO)](https://www.afro.who.int/countries/publications?country=879).


## Data dictionary

### 

| Column      | Definition | Format     |
| :---        |    :----:   |          ---: |
| Date as of      | Date of reporting.       | YYYY-MM-DD  |
| District     |  ISO 3 letter district code.       | String   |
| ConfCases | Daily number of new confirmed cases. | Numeric |
| CumCases| Cumulative number of cumulative confirmed cases. | Numeric |
| ConfDeaths | Daily number of new confirmed deaths. | Numeric |
| CumDeaths | Cumulative number of cumulative confirmed deaths. | Numeric |
| ConfRecoveries | Daily number of new confirmed recoveries. | Numeric |
| CumRecoveries | Cumulative number of cumulative confirmed recoveries. | Numeric |
| ConfHCWcases | Daily number of new confirmed cases of healthcare workers. | Numeric | 
| CumHCWCases | Cumulative number of confirmed cases of healthcare workers. | Numeric |
| ConfHCWDeaths | Daily number of new confirmed deaths of healthcare workers. | Numeric | 
| CumHCWDeaths | Cumulative number of confirmed deaths of healthcare workers. | Numeric |

## Getting the data

**Direct download (CSV)**: https://raw.githubusercontent.com/fbranda/ebola/main/Surveillance_data_Ebola_outbreak.csv

**Python** (requires `pandas`):
```python
import pandas as pd
df = pd.read_csv("https://raw.githubusercontent.com/fbranda/ebola/main/Surveillance_data_Ebola_outbreak.csv")
```

**R** (requires `httr`):
```r
library(httr)
df <- read.csv(text=content(GET("https://raw.githubusercontent.com/fbranda/ebola/main/Surveillance_data_Ebola_outbreak.csv")))
```


## License and attribution

This repository and data exports are published under the CC BY 4.0 license.
