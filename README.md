# Fictitious-Business---Data-Analysis
This is the start of my first data analysis project using a public dataset on a fictitious company.
[Download the Excel dataset](data/Subscription%20Cohort%20Analysis%20Data.xlsx). Follow the link and click on 'View raw'.

Documentation Overview: 

## 1. What is this project about?
  I want to dive into Data Analytics by applying my knowledge in real case analyses. This will be my first project, so it might not be as professional, but it will be showcasing my skills in this area nonetheless.
  For this project I have chosen a public and freely accessible dataset uploaded on Maven Anlaytics, which is provided under following link: https://mavenanalytics.io/data-playground/streaming-video-subscriptions
  Since this is my first 'real case application' I will be following the recommended questions. Those are as follows:
  How have Mavenflix subscriptions trended over time? 
  What percentage of customers have subscribed for 5 months or more? 
  What month has the highest subscriber retention, the lowest retention?

## 2. Data Preparation using Microsoft Excel

  <img width="730" height="828" alt="image" src="https://github.com/user-attachments/assets/ef653247-a18f-4235-8267-d0696008c149" />

  When first opening the file using Microsoft Excel you get overwhelmed by the mess of data this spreadsheet provides. I am going to clean up this data and transform it into a more readable and visually appealing format.
  ###  1. Seperating the data into individual columns
  ### 2. Creating a separate cleanup sheet
  ###  3. Standardizing date fields
  ###  4. Formatting Subscription costs
  ###  5. Checking for duplicate entries
  This is just a simple overview of the most important steps. I have attached the Excel file for a more detailed view to the data folder.

  Here is the result:

  <img width="940" height="791" alt="image" src="https://github.com/user-attachments/assets/d369366a-5c7d-4f4a-b0ea-c3455059b066" />

## 3. Analysis
  Now that I have finished the preparation of the data, I will analyze the cleaned dataset. The analysis will be presented in an interactive Power BI dashboard.
  After loading the completed Excel file into PowerBI, I have created 2 visuals to answer the first question: How have Mavenflix subscriptions trended over time?

  <img width="1380" height="792" alt="image" src="https://github.com/user-attachments/assets/4599c8d1-5d8c-456a-ab1d-a62c4c2d408d" />

  The left visual represents the Count of Canceled Date by Year, whereas the right visual focuses on the Count of Subscription Interval by Year and Month.
  By analyzing both visuals it is clear that 2023 had almost 50% more canceled subscriptions due to Mavenflix trending in the same year. I would also highlight      that April 2023 had a massive wave of canceled subscriptions. Also the low count in September 2023 could be due to unfinished data entries.
  And now to the second question: What percentage of customers have subscribed for 5 months or more? 
  That part was a bit more complex since my initial dataset did not contain data that explicitly said anything about subscription durations. Therefore I had to      create new columns in PowerBI using DAX.

  <img width="1567" height="901" alt="Screenshot 2026-09-16 091625" src="https://github.com/user-attachments/assets/c24fc225-96a1-4ad5-b4e0-b44976924747" />

  First a Duration column to determine how long each customer has subscribed for.

  <img width="1595" height="896" alt="Screenshot 2026-09-16 091641" src="https://github.com/user-attachments/assets/2db9c6ed-1b21-4429-aa7b-9c78d9b35ce9" />

  Secondly a Duration category column to automatically sort each customer into 2 different categories. 
  The last thing I had to do was creating a visual, which was much more simplified due to the prior steps.

  <img width="1362" height="772" alt="Screenshot 2026-09-16 091604" src="https://github.com/user-attachments/assets/a2304aa8-2337-4f99-92da-2591eb40bae1" />

  So, the answer to the second question is: 18.44% of Mavenflix customers have subscribed for 5 months or more.
  To answer the last question (What month has the highest subscriber retention, the lowest retention?) I had to create a new measure since I had no way of knowing   the retention rate otherwise.

  <img width="1027" height="293" alt="image" src="https://github.com/user-attachments/assets/388a916b-33f9-4a00-9f9a-58e9c254bfec" />

  And with that out of the way, the final visual is complete.

  <img width="1382" height="787" alt="Screenshot 2026-09-16 094030" src="https://github.com/user-attachments/assets/63bc8c0b-706c-4c63-989d-d5a7f52ae029" />

  The month with the highest retention rate is August with 82%, and the month with the lowest is November with only 12%.
## 4. Conclusion

The analysis focused on preparing and validating the dataset, identifying subscription patterns, analyzing customer subscription duration, and measuring retention over time. Data quality checks were also performed to distinguish legitimate multiple subscriptions from exact duplicate records.
The Power BI dashboard helped turn the cleaned data into an interactive view of key subscription metrics and customer behavior. This made it possible to identify patterns in subscription duration and retention and to explore how customer activity changes over time.
Beyond the analytical results, the project gave me practical experience with the complete data analysis workflow — from raw data cleaning and validation to data modeling, DAX calculations, visualization, and communicating findings.
This project also strengthened my understanding of how data can be transformed into meaningful business insights and provided a foundation for further projects.
  
