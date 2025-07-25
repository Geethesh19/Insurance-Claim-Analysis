# MySQL-Insurance-Claim-Analysis
**Insurance Claim Analysis: Demographic and Health**

This project performs an in-depth analysis of an insurance claims dataset, focusing on demographic and health-related factors to derive actionable insights. The analysis utilizes MySQL queries to extract, transform, and analyze the data, demonstrating strong proficiency in SQL for data manipulation and reporting.

**DataSet Source:**
* **Google Sheets:** [https://docs.google.com/spreadsheets/d/e/2PACX-1vRa1wWwXmzxEvqITxj4OQTeLywlGTTsOTbhSRqKj2lPuGefjlci-DQhgLBPpgWXe8AAUu2WUBqY59X1/pub?gid=1030172542&single=true&output=csv](https://docs.google.com/spreadsheets/d/e/2PACX-1vRa1wWwXmzxEvqITxj4OQTeLywlGTTsOTbhSRqKj2lPuGefjlci-DQhgLBPpgWXe8AAUu2WUBqY59X1/pub?gid=1030172542&single=true&output=csv)
* **Kaggle:** [https://www.kaggle.com/datasets/thedevastator/insurance-claim-analysis-demographic-and-health?select=insurance_data.csv](https://www.kaggle.com/datasets/thedevastator/insurance-claim-analysis-demographic-and-health?select=insurance_data.csv)

**Key Analyses Performed:**

The following SQL queries were executed to explore the dataset and answer specific business questions:

**1. Filtering Records for Male Patients from the 'southwest' Region:**
    * This query retrieves all data entries for male patients residing in the 'southwest' geographical region.
    * ![q1](https://github.com/Geethesh19/SQL-Insurance-Claim-Analysis/assets/52094094/fd07adbf-79f6-43e5-96fc-7ce2c396c1f8)

**2. Identifying Patients with BMI in a Specific Range (30 to 45 Inclusive):**
    * Retrieves records for patients whose Body Mass Index (BMI) falls within the range of 30 to 45 (inclusive), useful for identifying overweight or obese individuals.
    * ![q2](https://github.com/Geethesh19/SQL-Insurance-Claim-Analysis/assets/52094094/83374797-e97a-4760-b07d-a3016ae9701d)

**3. Determining Minimum and Maximum Blood Pressure for Diabetic Smokers:**
    * Calculates the lowest and highest recorded blood pressure values among patients who are both diabetic and smokers, aliased as `MinBP` and `MaxBP` respectively. This highlights health extremes in a high-risk group.
    * ![q3](https://github.com/Geethesh19/SQL-Insurance-Claim-Analysis/assets/52094094/ccb268ad-84de-47c1-ba04-e88c056e5ec5)

**4. Counting Unique Patients Outside the 'southwest' Region:**
    * Finds the total number of distinct patients who are not from the 'southwest' region, providing insight into geographical distribution of the patient base.
    * ![q4](https://github.com/Geethesh19/SQL-Insurance-Claim-Analysis/assets/52094094/90d147ab-3a05-4431-8475-76e3b4c42320)

**5. Calculating Total Claim Amount from Male Smokers:**
    * Aggregates the total claim amounts filed by male patients who are smokers, useful for assessing financial impact from this specific demographic.
    * ![q5](https://github.com/Geethesh19/SQL-Insurance-Claim-Analysis/assets/52094094/940a6f1b-7ec4-4c5a-a293-bcd7ff1b5d8c)

**6. Retrieving All Records from the 'south' Region:**
    * Selects all patient records originating from any sub-region within the 'south' category (e.g., 'southeast', 'southwest').
    * ![q6](https://github.com/Geethesh19/SQL-Insurance-Claim-Analysis/assets/52094094/ae12eeb0-dde2-44ec-b4be-7cf538810bdc)

**7. Counting Patients with Normal Blood Pressure (Standard Range):**
    * Determines the number of patients whose blood pressure falls within the commonly accepted normal range of 90 to 120.
    * ![q7](https://github.com/Geethesh19/SQL-Insurance-Claim-Analysis/assets/52094094/b4c915bc-7e65-4d4a-a683-5e46e26f0be3)

**8. Counting Patients Under 17 with Age-Adjusted Normal Blood Pressure:**
    * Counts patients under 17 years of age who have blood pressure within an age-adjusted normal range, calculated using the formula: `80 + (age * 2)` to `100 + (age * 2)`.
    * *Note: This formula is for illustrative practice purposes only and should not be taken as medical advice.*
    * ![q8](https://github.com/Geethesh19/SQL-Insurance-Claim-Analysis/assets/52094094/08a53d2b-3606-40da-9116-c8ab042df8d8)

**9. Calculating Average Claim Amount for Non-Smoking, Diabetic Female Patients:**
    * Computes the average claim amount for a specific high-risk group: non-smoking female patients who are diabetic.
    * ![q9](https://github.com/Geethesh19/SQL-Insurance-Claim-Analysis/assets/52094094/fd9a200c-5c78-4c23-99e9-20d372fc21a4)

**10. Updating Claim Amount for a Specific Patient:**
    * Demonstrates DML `UPDATE` operation by changing the `claim` amount for the patient with `PatientID = 1234` to 5000.
    * ![q10](https://github.com/Geethesh19/SQL-Insurance-Claim-Analysis/assets/52094094/f25e0252-385d-424f-bb8a-e275f716e2e5)

**11. Deleting Records for Smokers with No Children:**
    * Illustrates DML `DELETE` operation by removing all patient records who are smokers and have no children, useful for data maintenance or specific analysis scenarios.
    * ![q11](https://github.com/Geethesh19/SQL-Insurance-Claim-Analysis/assets/52094094/a42115cb-7077-4d10-b6c0-507622bf8498)
