# Synthetic data of Synthea patients
Open data of synthetic Synthea patients for machine learning (ML) and learning health systems (LHS).

Although there are a few freely-available large EHR datasets such as MIMIC-III and CPRD, they require qualified applications. In order to make it easier for developers to obtain ML-ready EHR data to work on ML and LHS without privacy concerns, this LHS open data project created synthetic Synthea patient data for ML and LHS simulation experiments. 

The first LHS simulation study titled "Simulation of a machine learning enabled learning health system for risk prediction using synthetic patient data" has been published in Nature Scientific Reports journal (see https://www.nature.com/articles/s41598-022-23011-4). To learn more about LHS, please check out the practical [LHS Quick Guide](https://github.com/lhs-open/lhs-guide).

Next, I hope the open synthetic data may enable more developer and clinician teams to develop and test ML algorithms, construct ML-enabled LHS, train members, and collaborate across hospitals.   

## ML-ready Synthea patient datasets

Synthea synthetic patient data were generated by the [Synthea patient generator tool](https://github.com/synthetichealth/synthea). The EHR records were processed to ML-ready datasets for lung cancer risk prediction. The lung cancer datasets (pt30k) from 30K patients are available here at github. Due to the file size limit by github, the complete collection of datasets from 150K patients is available from Mendeley Data repository.  

  - synthea-pt30k-lc-data-sel-convert.csv
  - synthea-pt60k-lc-data-sel-convert.csv
  - synthea-pt90k-lc-data-sel-convert.csv
  - synthea-pt120k-lc-data-sel-convert.csv
  - synthea-pt150k-lc-data-sel-convert.csv

**CAUTION**: ALL SYNTHETIC DATA IN THIS PROJECT ARE NOT REAL DATA. THEY ARE FOR TRAINING AND LEARNING PURPOSE ONLY. THESE DATA AND ANY DERIVED MODELS SHOULD NOT AND CAN NOT BE USED IN ANY REAL-WORLD SERVICES. 

License: [CC-BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/) (
You are free to adapt, copy or redistribute the material, providing you attribute appropriately and do not use the material for commercial purposes.)
