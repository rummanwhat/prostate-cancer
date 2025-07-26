Prostate Cancer Risk Factor Analysis
Overview

This repository contains a data analysis project focused on understanding potential risk factors for prostate cancer using a synthetic dataset. The analysis aims to identify significant associations between various health and lifestyle factors and estimated prostate cancer risk levels, providing insights valuable for public health awareness, machine learning research, and medical decision-support application development.
Dataset

The analysis utilizes a purely synthetic dataset simulating 1,000 individual health profiles. This dataset is designed for educational, research, and development purposes and contains no real patient information.

Dataset Columns:

Column Name
	

Description

id
	

Unique identifier for each individual (synthetic)

age
	

Age of the individual in years (30–80)

bmi
	

Body Mass Index (simulated around average value with some variation)

smoker
	

Indicates if the person is a smoker ("Yes" or "No")

alcohol_consumption
	

Level of alcohol intake: "None" / "Moderate" / "High"

diet_type
	

Type of diet: "Healthy" / "Fatty" / "Mixed"

physical_activity_level
	

Physical activity level: "Low" / "Moderate" / "High"

family_history
	

Whether there is a family history of cancer ("Yes" or "No")

mental_stress_level
	

Perceived mental stress: "Low" / "Medium" / "High"

sleep_hours
	

Average hours of sleep per day (between ~4.5 to 9)

regular_health_checkup
	

Whether the person does routine health checkups ("Yes" or "No")

prostate_exam_done
	

Whether prostate exam was done recently ("Yes" or "No")

risk_level
	

Estimated prostate cancer risk: "Low" / "Medium" / "High" (target variable)
Analysis Questions Addressed

The project specifically addressed the following questions:

    Does family_history significantly increase the risk_level?

    Are smoker and alcohol_consumption independent of each other?

    What is the average age for each risk_level?

Key Findings
1. Association between Family History and Risk Level

    Finding: A statistically significant association was found between family_history of cancer and the risk_level for prostate cancer (p\<0.0001).

    Implication: Individuals with a family history of cancer are considerably more likely to be in the 'Medium' or 'High' risk categories within this dataset. This highlights family history as a crucial factor in prostate cancer risk assessment.

2. Independence of Smoking Status and Alcohol Consumption

    Finding: The analysis indicated no statistically significant association between smoker status and alcohol_consumption levels (p=0.5192).

    Implication: In this synthetic dataset, smoking habits and alcohol consumption appear to be independent factors. Knowing one does not provide significant statistical information about the other's prevalence.

3. Average Age Across Risk Levels

    Finding: A clear positive correlation was observed between age and risk_level.

        Average age for 'Low' risk: ~53.83 years

        Average age for 'Medium' risk: ~56.55 years

        Average age for 'High' risk: ~60.21 years

    Implication: Older individuals, on average, are categorized into higher prostate cancer risk levels within this dataset, aligning with general epidemiological understanding of age as a primary risk factor for prostate cancer.

Technologies Used

    Python 3.x

    Pandas: For data loading, manipulation, and analysis.

    SciPy: For statistical tests (Chi-squared test).

    Matplotlib: For basic plotting.

    Seaborn: For enhanced statistical visualizations.

How to Run the Analysis

    Clone the repository:

    git clone <repository-url>
    cd <repository-name>



    Place the dataset: Ensure the synthetic_prostate_cancer_risk.csv file is in the root directory of the cloned repository.

    Install dependencies:

    pip install pandas scipy matplotlib seaborn



    Run the Python script(s):
    Execute the Python script containing the analysis code (e.g., python analyze_prostate_risk.py). The script will print the statistical outputs and display the generated plots.

Contact

Feel free to connect with me on LinkedIn: [Rumman Mohammad](https://www.linkedin.com/in/rummanmohammad/)
