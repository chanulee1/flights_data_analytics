# Project Background
This project analyzes the on-time flight performance data of the air carriers that held over one percent of the industry's total domestic scheduled-service passenger revenues in the US. This included the following 20 airlines:
- AirTran Airways Corporation
- Alaska Airlines Inc.
- Aloha Airlines Inc.
- American Airlines Inc.
- American Eagle Airlines Inc.
- Atlantic Southeast Airlines
- Comair Inc.
- Continental Air Lines Inc.
- Delta Air Lines Inc.
- Expressjet Airlines Inc.
- Frontier Airlines Inc.
- Hawaiian Airlines Inc.
- JetBlue Airways
- Mesa Airlines Inc.
- Northwest Airlines Inc.
- Pinnacle Airlines Inc.
- Skywest Airlines Inc.
- Southwest Airlines Co.
- United Air Lines Inc.
- US Airways Inc.

Performance is evaluated based on two main areas: cancellations and arrival delays*.

Insights are provided on the following key areas:

- **Seasonal Patterns:** Changes in cancellation and delay volume based on the time of year.
- **Cancellation Analysis:** Cancellation volume and rates by airline and airport, broken down by cause.
- **Delay Analysis:** Delay volume and rates by airline and airport, broken down by cause.

The SQL queries used to inspect and clean the data for this analysis can be found here [link].

Targeted SQL queries regarding various business questions can be found here [link].

An interactive Tableau dashboard used to report and explore sales trends can be found here [link].

\***Note:** A flight is considered "delayed" if it arrived at least 15 minutes later than the scheduled arrival time. Thus, flights that arrived less than 15 minutes late are technically not "delayed", but these flights were still included in the delay time distribution analysis.

# Data Structure & Initial Checks

The database constructed for this project (MySQL) consists of three tables: flights_on_time_2007, carriers, airports, with a total row count of 7458082 records. A description of each table is as follows:

- **flights_on_time_2007:** Flight records, including data such as the departure and arrival time, cancellation status, and delay times.
- **carriers:** Air carrier records, including their codes and descriptions.
- **airports:** Airport records, including their codes and locations.

The following ER diagrams contain only the fields that are relevant to the analysis.
![Database ER diagram (crow's foot) (1)](https://github.com/user-attachments/assets/d033e652-5dab-4502-8c95-bf1b7aa429d1)


# Executive Summary

### Overview of Findings

#### Busy Seasons
Although it varied across different airlines, the general seasonal patterns were as follows:
- The number of flights remained relatively constant over the year, with small spikes during the summer and towards the beginning/end of the year.
- The number of cancellations spiked during the spring and summer months, as well as towards the beginning/end of the year.
- The number of delays also spiked during the spring and summer months, as well as towards the beginning/end of the year.

#### Airlines with the Best and Worst Cancellation Performance
Based on cancellation rate, the worst-performing airline was **American Eagle Airlines Inc.**, which cancelled roughly **4.22%** of their flights in 2007 (540494 total flights). The best-performing airline was **Frontier Airlines Inc.**, with a cancellation rate of **0.41%** (97760 total flights).

#### Airlines with the Best and Worst Delay Performance
Based on delay rate, the worst-performing airline was **Atlantic Southeast Airlines**. Roughly **31.91%** of their flights in 2007 were delayed (286234 total flights). The best-performing airline was **Hawaiian Airlines Inc.**, with a delay rate of **6.29%** (56175 total flights).

#### Best and Worst Airline Overall
Ranking the airlines by taking a simple average of the cancellation and delay rates, the worst performing airline was **Atlantic Southeast Airlines**, with a score of roughly **0.175**. The best performing airline was **Hawaiian Airlines Inc.**, with a score of about **0.036**.

# Insights Deep Dive
### Seasonal Patterns:

* **Main insight 1.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 2.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 3.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 4.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.

[Visualization specific to category 1]


### Cancellation Analysis:

* **Main insight 1.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 2.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 3.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 4.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.

[Visualization specific to category 2]


### Delay Analysis:

* **Main insight 1.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 2.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 3.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 4.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.

[Visualization specific to category 3]


# Recommendations:

Based on the insights and findings above, we would recommend the [stakeholder team] to consider the following: 

* Specific observation that is related to a recommended action. **Recommendation or general guidance based on this observation.**
  
* Specific observation that is related to a recommended action. **Recommendation or general guidance based on this observation.**
  
* Specific observation that is related to a recommended action. **Recommendation or general guidance based on this observation.**
  
* Specific observation that is related to a recommended action. **Recommendation or general guidance based on this observation.**
  
* Specific observation that is related to a recommended action. **Recommendation or general guidance based on this observation.**
  


# Assumptions and Caveats:

Throughout the analysis, multiple assumptions were made to manage challenges with the data. These assumptions and caveats are noted below:

* Assumption 1 (ex: missing country records were for customers based in the US, and were re-coded to be US citizens)
  
* Assumption 1 (ex: data for December 2021 was missing - this was imputed using a combination of historical trends and December 2020 data)
  
* Assumption 1 (ex: because 3% of the refund date column contained non-sensical dates, these were excluded from the analysis)
