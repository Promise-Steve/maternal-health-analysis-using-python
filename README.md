# maternal-health-analysis-using-python


## Project Workflow and Documentation

### 1. Data Inspection and Understanding

The project began with importing the original NDHS Stata dataset using Pandas. We examined its structure, dimensions, columns and initial observations to understand the available data.

![Initial Data Inspection](images/Screenshot%202026-11-13%20211851.png)

![Dataset Exploration](images/Screenshot%202026-11-13%20212027.png)

### 2. Identification of Relevant Variables

We explored the available maternal health variables and identified indicators relevant to the research objectives. The variable identification process involved examining variables beginning with the prefix `m` and selecting relevant indicators for further investigation.

![Maternal Variable Identification](images/Screenshot%202026-11-13%20212105.png)

![Selection of Relevant Variables](images/Screenshot%202026-11-13%20212114.png)

### 3. Data Extraction and Preparation

A smaller working dataset was created by extracting the selected variables from the original dataset. The resulting dataset was examined to verify its dimensions and structure.

![Maternal Dataset Extraction](images/Screenshot%202026-11-13%20212152.png)

![Dataset Structure and Information](images/Screenshot%202026-11-13%20212202.png)

### 4. Understanding Variable Metadata

Pyreadstat was installed and used to access the dataset's metadata, including variable descriptions and value labels. This helped the team understand the numerical codes attached to the selected maternal health indicators.

![Pyreadstat Installation and Metadata Access](images/Screenshot%202026-11-13%20212219.png)

![Variable Labels and Value Codes](images/Screenshot%202026-11-13%20212231.png)

### 5. Missing Value Assessment

The team investigated missing-value patterns across the selected maternal health variables. This involved identifying records with incomplete information and preparing a separate dataset for subsequent maternal health analysis.

![Missing Value Assessment](images/Screenshot%202026-11-13%20212241.png)

![Maternal Analysis Dataset Preparation](images/Screenshot%202026-11-13%20212256.png)

### 6. Data Cleaning and Transformation

The cleaning process involved examining invalid values, handling special response codes and replacing inappropriate or unknown responses with missing values.

Selected variables were renamed and transformed into meaningful categories to improve readability and interpretation.

![Invalid Value Assessment](images/Screenshot%202026-11-13%20212306.png)

![Handling Special Missing Values](images/Screenshot%202026-11-13%20212317.png)

![Residence and Education Recoding](images/Screenshot%202026-11-13%20212328.png)

![Maternal Health Variable Transformation](images/Screenshot%202026-11-13%20212338.png)

![Delivery Location and Caesarean Section Classification](images/Screenshot%202026-11-13%20212348.png)

### 7. Data Validation

Following the cleaning and transformation stages, the team examined the resulting categories and their distributions to assess the consistency of the processed dataset.

![Validation of Cleaned Categories](images/Screenshot%202026-11-13%20212400.png)

### 8. Survey Design Inspection and Weighted Analysis Preparation

The project examined the survey-design variables required for complex survey analysis, including sampling weights, primary sampling units (clusters) and strata.

The dataset contained 1,368 unique clusters and 74 unique strata. These variables were inspected to support the preparation of survey-weighted analysis.

![Survey Design Validation](images/Screenshot%202026-11-13%20212415.png)

![Weighted Delivery Analysis Preparation](images/Screenshot%202026-11-13%20212618.png)
