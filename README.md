# Canadian Wildfire Data Visualization 

---

## Project Overview
This project involves preparing and visualizing Canadian wildfire data (1972–2023) to provide actionable insights for policymakers and stakeholders. The workflow includes data cleaning with Tableau Prep Builder and creating visualizations in Tableau to understand patterns and trends.

---

## Why This Matters
Harnessing wildfire data enables smarter prevention strategies that protect lives, ecosystems, and economies. The significance of this project lies in:  
- **Improved Safety:** Reducing the risk to human life and property.  
- **Preserved Ecosystems:** Protecting biodiversity and natural habitats.  
- **Economic Stability:** Mitigating recovery costs and enabling resource optimization.  

---
## Key Insights from the Data

### 1. **Northwest Territories Lead in Area Burned**
- The **Northwest Territories (NT)** surpass Quebec (QC) and Saskatchewan (SK) in total area burned.  
- NT is identified as a critical focus area for wildfire prevention efforts.  

### 2. **Wildfires at a Glance**
- Data reveals a **dramatic spike in wildfires**, signaling a crisis in Canada.  
- This surge poses significant threats to public safety and ecosystems.  

### 3. **What Drives Wildfires?**
- **Natural Causes** account for the majority of wildfires, with 81.7 million hectares burned.  
- **16.3 million hectares** remain undetermined, highlighting the need for advanced investigative methods.  

---

## Prevention Strategies

To mitigate the impact of wildfires, the following strategies are recommended:  
1. **Investment in Monitoring and Predictive Technologies:** Enhance forecasting to allocate resources efficiently.  
2. **Improving Firefighter Response:** Provide training and tools to combat wildfires effectively.  
3. **Public Awareness Campaigns:** Educate communities on prevention and preparedness.  
4. **Improving Scientific Research:** Develop new methods to identify and analyze fire causes.  

---
## Stakeholder Communication

### Key Stakeholders
1. **Fire Departments:** Managing immediate fire incidents.  
2. **Emergency Response Teams:** Handling rescue and disaster management.  
3. **Government Agencies:** Developing policies and ensuring public safety.  
4. **Environmental Scientists:** Studying wildfire patterns and impacts.  
5. **Local Communities:** Receiving timely information and resources.  

### Audience Concerns
- Public Safety  
- Environmental Impact  
- Economic Costs  
- Policy Development  

### Recommended Actions
- Implement smarter prevention strategies.  
- Strengthen firefighter training.  
- Relocate high-risk communities.  

### Risks of Inaction
- **Life and Property Loss**: Increased risk to human life and infrastructure.  
- **Environmental Damage**: Irreversible harm to ecosystems.  
- **Economic Disruption**: Prolonged recovery and financial instability.  
---

## Data Preparation

### Dataset Description
The dataset was sourced from Natural Resources Canada and includes:
1. **nbac_1972_2023_20240530**: Comprehensive wildfire records.
2. **sumstats_admin**: Burned areas by administrative regions.
3. **sumstats_natpark**: Burned areas within national parks.

### Cleaning Process with Tableau Prep Builder
#### Table: `nbac_1972_2023_20240530`
- **Steps Taken:**
  1. Imported dataset into Tableau Prep Builder.
  2. Renamed to "National Burned Area Composite Data 1972–2023."
  3. Enabled the Data Interpreter to clean and remove irrelevant rows/columns.
  4. Removed columns with >50% null values.
  5. Retained "Year" column as string for analysis purposes.
  6. Renamed columns per the data dictionary.
  7. Exported the cleaned data as a CSV file.

#### Table: `sumstats_admin`
- **Steps Taken:**
  1. Applied a cleaning step.
  2. Removed columns with >40% missing data.
  3. Filtered rows with missing data in the "NL" column (removed 7 rows).
  4. Exported the cleaned data as a CSV file.

#### Table: `sumstats_natpark`
- **Action Taken:** Discarded due to >90% missing values in most columns.

### Outputs
- **Cleaned Files:**
  - `cleaned_nbac.csv`
  - `cleaned_sumstats_admin.csv`

---

## Dataset Details

### Data Dictionary
#### Table: `sumstats_admin`
| Field Name | Data Type | Description                    | Level of Measurement | Example        |
|------------|-----------|--------------------------------|-----------------------|----------------|
| YEAR       | Integer   | Year of record                | Interval              | 2023           |
| AB         | Float     | Area burned in Alberta        | Ratio                 | 1,933,945.09   |
| BC         | Float     | Area burned in British Columbia | Ratio               | 2,203,857.84   |
| ...        | ...       | ...                           | ...                   | ...            |
| CANADA     | Float     | Total area burned in Canada   | Ratio                 | 14,600,643.19  |

#### Table: `nbac_1972_2023_20240530`
| Field Name | Data Type   | Description                            | Level of Measurement | Example       |
|------------|-------------|----------------------------------------|-----------------------|---------------|
| YEAR       | Integer     | Year of the record                    | Interval              | 2022          |
| NFIREID    | Integer     | Unique ID for each fire               | Ratio                 | 439           |
| FIRECAUS   | Text        | Cause of fire                         | Nominal               | Natural       |
| POLY_HA    | Integer     | Total area burned (hectares)          | Ratio                 | 45,023.96     |
| ADJ_HA     | Integer     | Adjusted area burned (hectares)       | Ratio                 | 44,500.00     |

### Data Source
- **Natural Resources Canada:** [Official Dataset](https://cwfis.cfs.nrcan.gc.ca/datamart)  
- **Published on Data is Plural (June 14, 2023):** [Archive](https://www.data-is-plural.com/archive/2023-06-14-edition/)  

---

## Call to Action
**Act now to prevent bigger losses.**  
- Implement smarter prevention strategies.  
- Strengthen firefighter skills.  
- Relocate high-risk communities.  

If we fail to act, we risk:  
- Lives and property.  
- Biodiversity and ecosystems.  
- Economic stability.  

This project demonstrates the potential of data-driven strategies to reduce wildfire impacts and protect what matters most.
## Conclusion
This project demonstrates the importance of leveraging data preparation and visualization tools to derive actionable insights for wildfire management. The findings and visualizations are designed to assist policymakers in mitigating the devastating effects of wildfires.
