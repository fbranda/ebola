# 2022 Uganda Ebola outbreak

## Contents

This repository contains data extracted from the [ECDC surveillance](https://www.ecdc.europa.eu/en/ebola-virus-disease-outbreak-uganda) and [Ministry of Health, Uganda](https://twitter.com/MinofHealthUG) bulletins in collaboration with the [World Health Organization - Regional Office for Africa (WHO AFRO)](https://www.afro.who.int/countries/publications?country=879).

#### Data changes
* **2022-10-29**: From this date data file (`Surveillance_hospital_data_Ebola_outbreak.csv`) contains case management summaries to accurately reflect the situation in hospitals. 
* **2022-11-11**: From this date data files (`epicurve_by_onset_date.csv`, `epicurve_by_notification_sex.csv`) have cases (confirmed and probable) per date of notification by sex. 
* **2022-11-15**: From this date data file (`epicurve_by_onset_date_district.csv`) have cases (confirmed and probable) per date of notification by district. 


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

## Contributions
1) [Branda F, Maruotti A. 2022 Uganda Ebola outbreak: early descriptions and open data. Journal of Medical Virology. 2022 Nov 24.](https://onlinelibrary.wiley.com/doi/full/10.1002/jmv.28344)
2) [Branda, Francesco and Mahal, Ahmed and Maruotti, Antonello and Pierini, Massimo and Mazzoli, Sandra. The challenges of open data for future epidemic preparedness: The experience of the 2022 Ebolavirus outbreak in Uganda](https://www.frontiersin.org/articles/10.3389/fphar.2023.1101894/full)


## License and attribution

This repository and data exports are published under the CC BY 4.0 license.
