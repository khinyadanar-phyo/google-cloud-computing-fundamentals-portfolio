# Alteryx Designer Cloud in Google Skills

## Introduction

This lab focuses on using Alteryx Designer Cloud (Dataprep by Trifacta) to visually explore, clean, transform, and analyze real-world datasets. The service provides a no-code, cloud-based environment for data preparation and enables efficient data wrangling at scale.

In this lab, the dataset from the 2016 United States Federal Election Commission (FEC) is used to demonstrate data import, cleaning, transformation, joining, and aggregation.

## Objectives

- Create and configure a Cloud Storage bucket for data storage.
- Initialize and access Alteryx Designer Cloud (Dataprep).
- Import datasets from Google Cloud Storage into a flow.
- Correct mismatched and inconsistent data types.
- Transform and clean raw datasets using wrangling recipes.
- Join multiple datasets using common keys.
- Perform aggregation and summarization of data.
- Rename and format output columns for analysis.

## Key Steps Performed

1. Created a Cloud Storage bucket to store datasets.
2. Initialized Alteryx Designer Cloud (Dataprep) and configured project access.
3. Created a new flow named **FEC-2016**.
4. Imported datasets:
   - Candidate Master 2016
   - Campaign Contributions 2016
5. Cleaned candidate data by:
   - Filtering valid election year records
   - Fixing mismatched column data types
   - Converting state column to string type
   - Filtering presidential candidates (P values only)
6. Prepared contribution dataset by removing unwanted delimiters using wrangling expressions.
7. Joined candidate and contribution datasets using inferred join keys (column2 = column11).
8. Performed aggregation using pivot operations:
   - Sum of contributions
   - Average contribution amount
   - Count of contributions
9. Grouped results by candidate ID, candidate name, and party affiliation.
10. Renamed columns for readability:
   - Candidate_ID
   - Candidate_Name
   - Party_Affiliation
   - Total_Contribution_Sum
   - Average_Contribution_Sum
   - Number_of_Contributions
11. Rounded average contribution values for better interpretation.

## Results

The final dataset successfully summarizes 2016 U.S. presidential campaign contributions. It provides insights into total fundraising amounts, average donation size, and number of contributions received by each candidate, grouped by political party and candidate identity.

The transformed dataset is clean, structured, and suitable for further visualization and analysis.

## Conclusion

This lab demonstrated how Alteryx Designer Cloud (Dataprep) simplifies data preparation through a visual, no-code interface. The raw FEC datasets were successfully imported, cleaned, transformed, joined, and aggregated into a meaningful analytical dataset.

The exercise highlights the effectiveness of cloud-based data wrangling tools in preparing large datasets for business intelligence and data analysis tasks.
