# maternal-health-analysis-using-python

**Learning Together. Analysing Data. Creating Impact.**

Pairbud is a collaborative data analytics project focused on exploring maternal healthcare indicators in Nigeria using Python and data from the Nigeria Demographic and Health Survey (NDHS).

The project applies data inspection, cleaning, transformation and statistical data preparation techniques to examine maternal healthcare indicators and explore the socioeconomic factors associated with maternal healthcare utilisation.

---

## About the Project

Maternal healthcare remains an important public health priority in Nigeria. Access to essential maternal health services can vary according to socioeconomic circumstances, educational attainment, household wealth and geographical location.

This project uses Python to explore maternal health data, identify relevant indicators, prepare datasets for analysis and develop a foundation for understanding patterns in maternal healthcare utilisation.

Through this project, the Pairbud team demonstrates how programming and data analytics can contribute to public health research and evidence-informed decision-making.

## Project Objectives

The project seeks to:

- Explore maternal healthcare indicators within the NDHS dataset.
- Examine maternal healthcare utilisation across different socioeconomic groups.
- Investigate differences associated with educational attainment, household wealth and place of residence.
- Assess antenatal care attendance and delivery-related indicators.
- Apply appropriate data cleaning and preparation techniques.
- Develop a structured dataset for subsequent statistical analysis.

## Tools and Technologies

The project uses the following Python tools and technologies:

| Tool | Application |
|---|---|
| Python | Primary programming language |
| Pandas | Data manipulation and cleaning |
| NumPy | Numerical operations |
| Matplotlib | Data visualisation |
| Pyreadstat | Reading Stata datasets and metadata |
| Samplics | Complex survey analysis |
| Jupyter Notebook | Interactive analysis and documentation |

## Project Workflow and Documentation

The analysis follows a structured data preparation workflow. The following sections document the practical work undertaken by the team.

### 1. Data Inspection and Understanding

The initial stage involved importing the NDHS Stata dataset, examining its structure, inspecting the first few records and understanding the available variables.

The original dataset contained 39,050 records and 6,411 columns.

**Notebook documentation:**

![Data Inspection](images/01-data-inspection.png)

### 2. Identification of Relevant Variables

The team examined the available dataset variables to identify indicators relevant to the project's maternal healthcare objectives.

A broader variable-matching exercise identified 1,940 variables beginning with the prefix `m`, from which relevant maternal health indicators were selected for further investigation.

**Notebook documentation:**

![Variable Identification](images/02-variable-identification.png)

### 3. Data Extraction and Preparation

A smaller working dataset was created by extracting selected variables from the original dataset.

The initial selection contained nine variables, covering respondent characteristics, socioeconomic indicators and maternal health information.

**Notebook documentation:**

![Data Extraction](images/03-data-extraction.png)

### 4. Missing Value Assessment

The team investigated missing-value patterns across the selected maternal health variables to understand the extent and distribution of incomplete observations.

This process identified 25,082 records with all four initially selected maternal health variables missing and 13,968 records with at least one available maternal health variable.

A separate analysis dataset was subsequently prepared using three core maternal health variables.

**Notebook documentation:**

![Missing Value Assessment](images/04-missing-values.png)

### 5. Data Cleaning and Transformation

Data cleaning involved identifying special response codes, replacing inappropriate or unknown responses with missing values, renaming variables and transforming numerical codes into more meaningful categories.

The selected variables were converted into readable classifications to support interpretation and subsequent analysis.

Examples include:

- Residence: Urban and Rural.
- Education: No education, Primary, Secondary and Higher.
- Tetanus injections: Categorised according to the number of injections received.
- Antenatal care: Number of antenatal visits.
- Delivery location: Grouped into relevant delivery facility categories.
- Caesarean section: Yes and No.

**Notebook documentation:**

![Data Cleaning](images/05-data-cleaning.png)

### 6. Data Validation

Following data cleaning and transformation, the team examined unique values and category distributions to assess the consistency of the processed variables.

This stage helped verify the recoded categories and identify potential data inconsistencies before proceeding to further analysis.

**Notebook documentation:**

![Data Validation](images/06-data-validation.png)

### 7. Survey Design Inspection

The project also examined the survey-design variables required for complex survey analysis.

These included:

- Sampling weights (`v005`)
- Primary sampling units or clusters (`v021`)
- Sampling strata (`v022`)

The dataset contained 1,368 unique clusters and 74 unique strata.

This inspection provided the foundation for incorporating the survey design appropriately into subsequent statistical analysis.

**Notebook documentation:**

![Survey Design Inspection](images/07-survey-design.png)

---

## Dataset Summary

The following table summarises the key figures obtained during the data preparation stage.

| Description | Result |
|---|---:|
| Original dataset records | 39,050 |
| Original dataset columns | 6,411 |
| Initially selected variables | 9 |
| Records with at least one available maternal variable | 13,968 |
| Records retained for the three core maternal variables | 13,968 |
| Identified survey clusters | 1,368 |
| Identified survey strata | 74 |

*Note: These figures describe different stages of dataset inspection and preparation. They should not be interpreted as final analytical findings or as the sample size for every subsequent analysis.*

## Project Structure

The repository is organised to maintain a clear separation between datasets, analytical notebooks, documentation and supporting images.

```text
maternal-health-analysis-using-python/
│
├── data/
│
├── notebooks/
│
├── documentation/
│
├── images/
│   ├── 01-data-inspection.png
│   ├── 02-variable-identification.png
│   ├── 03-data-extraction.png
│   ├── 04-missing-values.png
│   ├── 05-data-cleaning.png
│   ├── 06-data-validation.png
│   └── 07-survey-design.png
│
├── requirements.txt
├── .gitignore
└── README.md
```

## Getting Started

To explore and reproduce the project workflow:

**1. Clone the repository**

```bash
git clone https://github.com/Promise-Steve/maternal-health-analysis-using-python.git
```

**2. Navigate into the project directory**

```bash
cd maternal-health-analysis-using-python
```

**3. Install the required dependencies**

```bash
pip install -r requirements.txt
```

**4. Access the project notebook**

Navigate to the `notebooks/` directory and open the relevant Jupyter Notebook.

```bash
jupyter notebook
```

**5. Access the dataset**

The original NDHS microdata is not distributed with this repository. Researchers should obtain the appropriate access authorisation through the DHS Program before attempting to reproduce the analysis.

## Project Status

The project has completed its initial data inspection, variable identification, data extraction, missing-value assessment, cleaning, transformation and validation stages.

The prepared dataset provides a foundation for subsequent maternal health statistical analysis and visualisation.

## Contributors

**Pairbud Project Team**

A collaborative learning initiative focused on applying Python programming and data analytics to real-world public health research.

GitHub Repository: [Maternal Health Analysis Using Python](https://github.com/Promise-Steve/maternal-health-analysis-using-python)

## Acknowledgements

We acknowledge the Demographic and Health Surveys (DHS) Program and the relevant Nigerian survey authorities for making the survey data available for research purposes.

We also appreciate the Python Study Group community for encouraging collaborative learning, practical programming and the application of data analytics to real-world challenges.

---

**PAIRBUD**

*Learning Together. Building Together. Creating Impact.*
