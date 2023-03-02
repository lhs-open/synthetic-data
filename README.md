# Open Synthetic Patient Data
Open data of synthetic patients for machine learning (ML) and learning health systems (LHS).

Although there are some freely-available large EHR datasets such as MIMIC-III and CPRD, they require qualified applications. In order to make it easier for anyone to obtain synthetic patient data free of privacy concerns, this open data repository is created for the community to share synthetic data. AJ initiated the repository with the initial Synthea datasets from his ML and LHS simulation experiments. 

With these open synthetic datasets, researchers may find it useful in developing ML algorithms, building ML-enabled LHS processes, testing, training, and collaborating across teams. From our research using synthetic and real EHR data, a new "synthetic+real" strategy is emerging: using synthetic data to develop new processes first and then applying them to real EHR data. You may try this strategy to see whether it can accelerate your healthcare ML, AI and LHS projects. If you need new Synthea data that are not found here, you may contact AJ for suggestions.  

The datasets were used in the first LHS simulation study, which published a paper "Simulation of a machine learning enabled learning health system for risk prediction using synthetic patient data" in Nature Scientific Reports (see https://www.nature.com/articles/s41598-022-23011-4). 

To learn more about LHS, please check out the open [LHS Practical Guide](https://github.com/lhs-open/lhs-guide).

## Synthea synthetic patient records

Synthea synthetic patient records were generated by the [Synthea patient generator tool](https://github.com/synthetichealth/synthea). 

For a demo of how to check Synthea data for diseases and use Synthea data for ML training, see [<bold>synEHR DEMO</bold>](https://web2express.org/synehr).  

- 100-patient dataset: Medical records for 100 Synthea live patients are in a zip file in folder record/.
- 30K-patient dataset: This dataset has 2 populations of Synthea synthetic patients, 15K patients each, with original medical records in CSV files. Because the total file size is >3GB in each population, the files are only available in [Harvard Dataverse: Synthetic Patient Data ML Dataverse](https://dataverse.harvard.edu/dataverse/synthetic-patient-ml).

## ML-ready Synthea synthetic patient datasets

The Synthea patient records were processed to ML-ready datasets for machine learning. If the continuous numeric values are converted to categorical values, the data file name has "convert" in it. Medical code format: original standard code (SNOMED-CT, LOINC, etc.) prefixed by 'C-'.

### For lung cancer risk prediction machine learning

- Five lung cancer datasets (pt30k*), each from 30K patients. Five datasets with continuous numeric values converted. 
- Standard codes for the lung cancer data: synthea-lc-dataset-codes.csv.
- Complete collection of lung cancer datasets from 30K to 150K Synthea patients. Only available in [Harvard Dataverse: Synthetic Patient Data ML Dataverse](https://dataverse.harvard.edu/dataverse/synthetic-patient-ml) and [Mendeley Data repository](https://data.mendeley.com/datasets/b24cb4nn8h/1) due to the file size limit by GitHub. These datasets were used to simulate ML-LHS in the Nature Sci Rep paper. 

  - synthea-pt30k-lc-data-sel-convert.csv
  - synthea-pt60k-lc-data-sel-convert.csv
  - synthea-pt90k-lc-data-sel-convert.csv
  - synthea-pt120k-lc-data-sel-convert.csv
  - synthea-pt150k-lc-data-sel-convert.csv

### For stroke risk prediction machine learning

- One stroke ML dataset (pt30k) from 30K patients. One dataset after value conversion.
- Standard codes for the stroke data: synthea-stroke-dataset-codes.csv.
- Stroke ML datasets from 30k to 150k Synthea patients, available in [Harvard Dataverse: Synthetic Patient Data ML Dataverse](https://dataverse.harvard.edu/dataverse/synthetic-patient-ml). These datasets were used to simulate ML-LHS in the Nature Sci Rep paper.

  - synthea-pt30k-stroke-ml-table-sel-convert.csv
  - synthea-pt60k-stroke-ml-table-sel-convert.csv
  - synthea-pt90k-stroke-ml-table-sel-convert.csv
  - synthea-pt120k-stroke-ml-table-sel-convert.csv
  - synthea-pt150k-stroke-ml-table-sel-convert.csv

All of the open Synthea patient datasets are available in [Harvard Dataverse: Synthetic Patient Data ML Dataverse](https://dataverse.harvard.edu/dataverse/synthetic-patient-ml).

## More Synthea patient data

Synthea patient generator is very powerful, thanks to the MITRE team. It has modeled over 100 diseases and conditions already. You can essentially generate a synthetic EHR with millions of patients on your server. In addition, if you need patient data for any disease and condition that is not covered by Synthea yet, Synthea allows you to model the disease or condition and generate new relevant synthetic data.   

**Contact**: If you have questions or need help on generating and using Synthea data, you may email AJ (ajchen(at)web2express.org), Co-Chair of [LHS Tech Forum Initiative](https://www.learninghealth.org/2020-lhs-technology-forum), Learning Health Community. 

<br>

**CAUTION**: ALL SYNTHETIC DATA IN THIS PROJECT ARE NOT REAL DATA. THEY ARE FOR TRAINING AND LEARNING PURPOSE ONLY. THESE DATA AND ANY DERIVED MODELS SHOULD NOT AND CAN NOT BE USED IN ANY REAL-WORLD SERVICES. 

**License**: [CC-BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/). You are free to adapt, copy or redistribute the material, providing you attribute appropriately and do not use the material for commercial purposes.
