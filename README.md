Superstore Retail Insights Dashboard

<img width="1588" height="813" alt="Superstore Pic 1" src="https://github.com/user-attachments/assets/c08e2e73-e4b3-4594-9edf-2f26e0590cd8" />


PROJECT OVERVIEW

Following my role as a Senior Data Analyst at Feefo, I developed this Looker dashboard as a portfolio project to demonstrate my proficiency within the Looker ecosystem. Using the classic Superstore dataset, this project serves as a comprehensive look at my ability to manage the full data lifecycle—from initial modeling in BigQuery to LookML development and final visualisation.



The primary objective was to evidence my understanding of Views, Explores, and the underlying LookML logic required to build functional, enterprise-ready dashboards. While this version utilises a combined dimension table for efficiency, it is designed to showcase how to join dimension and fact views effectively within a single model.



DATA SOURCE AND PROCESS

The project utilises the open-source Superstore dataset from Kaggle, which provides transactional retail records.



My process began with ingesting the raw CSV data into Google BigQuery to assess data quality, checking for missing or duplicated values. I then used SQL to structure the data into a Fact table for transactions and a 'combined' Dimension table for attributes. Once the data was mirrored in Looker, I developed custom dimensions and summary measures, such as Net Profit Margin, to provide deeper business insights.



TECHNICAL ARCHITECTURE

I focused on several key LookML features to demonstrate senior-level technical proficiency:



\* Custom Measure Logic: I developed complex measures using the SQL parameter. A primary example is the Net Profit Margin, calculated as: Total Profit / Total Sales.

\* Dimension Groups: I defined specific dimension groups for time-based fields, enabling end-users to drill down from Year to Quarter or Month seamlessly.

\* Data Integrity: I implemented primary keys within the LookML views to prevent fan-outs and ensure accurate row counts across all joins.

\* Semantic Layer Management: I focused on transforming technical SQL column names into intuitive, business-friendly labels to improve the self-service experience.



REPOSITORY STRUCTURE

\* Views: Includes the .view files defining dimensions and measures for order facts and product/customer dimensions.

\* Models: Includes the .model file where Explores are defined, including join logic and caching policies.

\* Dashboards: Contains LookML-defined dashboard files for version-controlled visualisation.



FUTURE IMPROVEMENTS

While this dashboard serves as a technical proof of concept, I have identified several strategic and technical areas for future iteration:



\* User Persona Integration: Transitioning the design from a technical showcase to a persona-based approach (Strategic vs. Operational) to better serve specific business stakeholders.

\* Advanced Functionality: Implementing Liquid parameters for dynamic date granularity (Year/Month/Week) and adding a date switching filter to toggle between Order Date and Ship Date.

\* Enhanced Normalisation: Splitting the current dimension table into fully normalised tables for Customers, Products, and Geography to optimise model performance.

\* Visual Refinement: Replacing standard bar charts with combined bar and line charts to better visualise sales as a combination of profit and costs and generally tidying up the UI. 

