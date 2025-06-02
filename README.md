# Project: Power BI Customer Churn Analysis Dashboard

**Author:** NGUYEN PHAM
**Date:** May 14, 2025
**Contact:** nguyen.pham961309@gmail.com | [https://www.linkedin.com/in/khoinguyenpham/]

---

## 1. Introduction & Objectives

* This project presents an interactive Power BI dashboard designed to analyze the performance of the customer call center.  
* The primary objective is to understand the nature of the customers, including the long-term trends of the customers and agent behavior. From different examples of metrics, we need to define, categorize and arrange the metrics in a proper order to envision a story related to the trends of agents and clients
* This builds upon my experience in creating impactful dashboards to track sales performance and drive customer-centric decisions, similar to my work done at AIA Vietnam

**The core problem** of this project addresses is the need for a clear, dynamic, and easily interpretable visualization of call center performance, aligning with the general demand from the head of call center team. 
**The 2nd core problem** of this project addresses the usage of the head of call center team: as a base for discussing with management. This line of requirement means there is a need for further extension in the future, adapting the business change or the team's activities. Hence, besides a focused dashboard on several important metrics, there must be several recommended options or metrics to delve into the agent's performance. 

**Key Analytical Goals:**
* To identify and visualize different indicators, related to each agent, call topic, length topic, and specific satisfaction rating from the customers.
* There are columns related to time that can be used for time analysis: “Date” (in the form of full date) and “Time” (in the form of the timestamp where the call started)
* To provide a user-friendly interface for stakeholders to explore agents' performance and customer behavior

---

## 2. Data Sources
This dataset is highly structured and standardized, but there are rooms for further exploration to have the analysis efficient
* Each row represents a unique call between customers and an agent, including different attributes of the call and the satisfaction rating from 1 to 5 
* There are columns with binary values (Yes / No) related to the problem discussed in the call
* There are columns with categorical values (agents' names and call topic)
* There are time related columns (speed of answer and average talk duration). They are in different format so they need to be formatted into one unit of time length (in seconds, perhaps)
* There are no clear quantitative variables, but since some of the columns can be formatted into more meaningful columns, we can anticipate discrete variables (such as satisfaction rating in average or time length in seconds)

---

## 3. Tools & Technologies Used
*   **Data Visualization & Dashboarding:** Microsoft Power BI (including DAX for complex measures and calculations)
*   **Data Preparation:** Microsoft Excel (Power Query)
*   **Version Control:** Git & GitHub
*   **IDE/Editor (for this README):** Visual Studio Code

---

#### 4. Project Structure

The repository is organized as follows:

```text
PwC Swiss_Call center_Nguyen Khoi Nguyen PHAM_2003.pbix   # The main Power BI file
├── data/                                                 # For the datasets
│   └── 01 Call-Center-Dataset.csv
├── dax/                                                  # For DAX script including measures
│   └── dax_measures and logics.md
├── images/                                               # For screenshots of my dashboard
│   ├── Fishbone_Callcenter diagram.png
│   ├── PwC Swiss_Data Analysis by PBI_Nguyen Khoi Nguyen Pham-01.png
│   ├── PwC Swiss_Data Analysis by PBI_Nguyen Khoi Nguyen Pham-02.png
│   ├── PwC Swiss_Data Analysis by PBI_Nguyen Khoi Nguyen Pham-03.png
│   ├── PwC Swiss_Data Analysis by PBI_Nguyen Khoi Nguyen Pham-04.png
│   ├── PwC Swiss_Data Analysis by PBI_Nguyen Khoi Nguyen Pham-05.png
│   ├── PwC Swiss_Data Analysis by PBI_Nguyen Khoi Nguyen Pham-06.png
│   ├── Dataset Call center.png
│   ├── date table_dayofweek.png
│   ├── Handle time duration 1.png
│   └── Handle time duration 2.png
├── .gitignore                                            # Specifies intentionally untracked files
└── README.md                                             # This file!