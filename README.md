# Exploring Data Science Salaries in 2023

### Introduction
![](https://github.com/blessingekwere/Data-Science-Salary/blob/main/Inro%20pics%202.jpg)
###### Photo Source: Google

Technology careers have evolved rapidly over the years, driven by advancements in computing, communication, and automation technologies. The rise of the internet, mobile devices, cloud computing, and artificial intelligence has led to the creation of new job roles and has transformed existing ones. Some of the most popular technology careers today include software development, data science, cybersecurity, and cloud computing. These roles require a mix of technical and soft skills, including programming languages, database management, project management, communication, and problem-solving.

Data science is a multidisciplinary field that involves using scientific methods, processes, algorithms, and systems to extract insights and knowledge from structured and unstructured data. It involves various fields such as statistics, computer science, mathematics, domain knowledge, and more. The evolution of data science in tech has been rapid and transformative. In the early days, data science was primarily used for traditional data analysis tasks, such as exploratory data analysis, regression analysis, and predictive modeling. However, with the advent of big data and the explosion of digital information, the field of data science has expanded and transformed significantly. One of the biggest trends in data science in recent years has been the development of machine learning algorithms and deep learning neural networks. These advanced techniques have enabled data scientists to analyze and extract insights from massive amounts of data and solve complex problems in areas such as natural language processing, computer vision, and more. In addition, there has been an increasing emphasis on data-driven decision-making in businesses, leading to the rise of data analytics and business intelligence. Data scientists are now playing a critical role in helping organizations make data-driven decisions by providing insights and recommendations based on their analysis.

Overall, technology careers have undergone significant evolution over the years, and the demand for skilled professionals is expected to continue to grow. As a result, the salaries for these roles are likely to remain competitive and offer opportunities for career growth and advancement.

### Problem Statement
![](https://github.com/blessingekwere/Data-Science-Salary/blob/main/Into%20pics%203.jpg)
###### Photo Source: Google

With the increasing demand for data science professionals in various industries, there is a need to understand the factors that impact salaries in this field. This includes analyzing data related to compensation for data scientists and related positions, such as location, level of experience, education, job title, and industry. By exploring this data, we aim to identify trends and patterns that can help both job seekers and employers make informed decisions about compensation packages and career planning.

Furthermore, as the job market and skills required for data science evolve, it is crucial to track changes in salaries and understand how they may be impacted by these factors in the year 2023. Thus, the problem statement is to explore the data science salaries in 2023 dataset to gain insights into the factors that contribute to salary differences in this rapidly growing field. 

This project will answer questions such as 
* What is the average data science salary in 2023? 
* What is the median data science salary in 2023? 
* What is the highest and lowest salary in the dataset?
* What is the distribution of salaries in the dataset? 
* Which region pays the highest salaries?
* Which region has the most data science jobs? 
* Which year was the highest salaries paid? 
* What is the average salary for data scientists with different levels of experience? 
* Which job titles have the highest salaries? 
* How does company size affect salaries for data science roles?


### Skills Demonstrated
* Data Exploration
* Data cleaning and preparation
* Data Manipulation
* Visualization
* Analysis


### Data Sourcing
The data was downloaded from Kaggle. The dataset contains data from 10,000 respondents and was collected through a survey. The data is available in a CSV file format and contains 11 columns. The columns include:

* work_year: The year the salary was paid.
* experience_level: The experience level in the job during the year
* employment_type: The type of employment for the role
* job_title: The role worked in during the year.
* salary: The total gross salary amount paid.
* salary_currency: The currency of the salary paid as an ISO 4217 currency code.
* salaryinusd: The salary in USD
* employee_residence: Employee's primary country of residence in during the work year as an ISO 3166 country code.
* remote_ratio: The overall amount of work done remotely.
* company_location: The country of the employer's main office or contracting branch.
* company_size: The median number of people that worked for the company during the year.
You can click [here](https://www.kaggle.com/datasets/arnabchaki/data-science-salaries-2023
) to access the original dataset



### Data Transformation
Although the dataset was not really messy, I still had to take a few measures to prepare it for further analysis. These steps included:
* Checking for duplicates, spelling errors, inconsistencies and missing data.
* Converting data in different columns to the correct data type. For example, I converted the 'salary_in_usd' column from varchar to int, work_year to date data type using the 'Alter' function.
![](https://github.com/blessingekwere/Data-Science-Salary/blob/main/Replacing%20the%20values%20in%20the%20experience%20level%20column.png)
![](https://github.com/blessingekwere/Data-Science-Salary/blob/main/Replacing%20the%20values%20in%20the%20experience%20level%20column.png)
* Updating values in different columns to their full form from abbreviated form. For instance, I converted 'EL' to 'Entry Level', 'ML' to 'Mid Level', 'EN' to 'Entry Level to Mid-Level', and 'EX' to 'Experience' in the 'experience_level' column. Similarly, I converted 'FT' to 'Full Time', 'CT' to 'Contract', and 'PT' to 'Part Time' in the 'Employment_type' column.
* Updating the abbreviated names of countries in the 'Employee_residence' and 'Company_location' columns with their corresponding full country names using the 'update' command.


### Analysis
As previously mentioned, the purpose of this analysis was to address various questions, including those outlined earlier. So, let's dive in and tackle these questions one by one, as well as any additional ones that arise. Lets see the queries and visualisations that helped us arrive at our conclusions.

* After writing queries to answer all the questions, I create view for all of the queries using the ‘Create View AS’ syntax.

* After creating all the views, I launched my Power BI, which is the tool that I will be using to visualize this data. From the Power BI launch page, I clicked on ‘Get Data’, a drop down appeared, and I clicked on the SQL server option to connect my Power BI to the SQL server. I then inputted the required details which are my SQL server name and the database I needed to extract the data from. After that my SQL server was connected to my Power BI, I then had to select the views which I earlier created on SQL Server and clicked transform to launch my power query editor in case there was need for further transformation.
* 
Well, since there was no need for further transformation on power query editor, I loaded the tables into Power BI to continue the analysis and visualization.


*	What is the average data science salary in 2023?
![](https://github.com/blessingekwere/Data-Science-Salary/blob/main/What%20is%20the%20average%20data%20science%20salary%20in%202023_.png)
This query shows that the average salary of a data scientist in 2023 is $158,020 and the reason is likely because this report is published in the second quaarter of 2023.

*	What is the median data science salary in 2023?
![](https://github.com/blessingekwere/Data-Science-Salary/blob/main/What%20is%20the%20median%20data%20science%20salary%20in%202023_.png)

 This query shows that the median of a data scientist salary in 2023 is $143182
 
![](https://github.com/blessingekwere/Data-Science-Salary/blob/main/Median%20Data%20Science%20Salary%202023%20-%20Copy.png)
###### Visual showing the median salary of data science in 2023

*	What is the highest, lowest and average salary in the dataset?
![](https://github.com/blessingekwere/Data-Science-Salary/blob/main/What%20is%20the%20highest%2Clowest%20and%20average%20salary%20in%20the%20dataset_.png)

This query showed that the highest, lowest and average salaries are 450000, 5132 and 137570 resectively

*	What is the distribution of salaries in the dataset?
To answer this question, I first grouped to salary into what I call salary rating and then used the rating to check for the salary distribution
![](https://github.com/blessingekwere/Data-Science-Salary/blob/main/Grouping%20the%20salary%20scale%20to%20check%20the%20distrubution%204.png)

![](https://github.com/blessingekwere/Data-Science-Salary/blob/main/Count%20of%20salary%20rating%20by%20salary%20rating%20-%20Copy.png)
###### Visual showing the distribution of salary by rating


*	Which region pays the highest salaries?

![](https://github.com/blessingekwere/Data-Science-Salary/blob/main/Which%20region%20pays%20the%20highest%20salaries_.png)
This query shows that United States of America pays the highest salaries of $461,538,909

![](https://github.com/blessingekwere/Data-Science-Salary/blob/main/Salary%20by%20work%20location%20-%20Copy.png)
###### Visual showing the regions that pay the highest salaries

*	Which region has the most data science jobs?
![](https://github.com/blessingekwere/Data-Science-Salary/blob/main/Which%20region%20has%20the%20most%20data%20science%20jobs_%20correct.png)
This query shows that United States of America has the most data science jobs

![](https://github.com/blessingekwere/Data-Science-Salary/blob/main/Top%2010%20company%20location%20by%20employee%20count%20-%20Copy.png)
###### Visual showing the regions that pay the highest salaries

*	What year had the highest salaries?
![](https://github.com/blessingekwere/Data-Science-Salary/blob/main/What%20year%20was%20the%20highest%20salaries%20paid.png)
This query showed that the highest salary was paid in 2023 with a total of $266,046,291

![](https://github.com/blessingekwere/Data-Science-Salary/blob/main/Salary%20By%20year.png)
###### Visual showing salaries paid per year


*	What is the top-paying company sizes for data science roles?
![](https://github.com/blessingekwere/Data-Science-Salary/blob/main/What%20are%20the%20top-paying%20company%20Sizes%20for%20data%20science%20roles_.png)
This query showed that companies categorized under the medium category paid the most salaries with a total of $121,639,683 for data science roles followed by large and small categorized companies paying $16,595,465 and $3,085,782 respectively.

*	What is the average salary for data scientists with different levels of experience?
![](https://github.com/blessingekwere/Data-Science-Salary/blob/main/What%20is%20the%20average%20salary%20for%20data%20scientists%20with%20different%20levels%20of%20experience_.png)

![](https://github.com/blessingekwere/Data-Science-Salary/blob/main/Average%20Salary%20By%20experience%20level%20-%20Copy.png)
###### Visual showing the average salary for data science role by experience level


*	Which job titles have the highest salaries?
![](https://github.com/blessingekwere/Data-Science-Salary/blob/main/Which%20job%20titles%20have%20the%20highest%20salaries_.png)

![](https://github.com/blessingekwere/Data-Science-Salary/blob/main/Top%2010%20job%20title%20by%20salary%20-%20Copy.png)
###### Visual showing the top 10 job titles by total salary

*	How does company size affect salaries for data science roles?
![](https://github.com/blessingekwere/Data-Science-Salary/commit/6bd48dbe4bef5240ee7c3956cfc74d5fcb841889)
This query shows that companies categories as medium size employ more data scientists.

*	How many employees are not resident in their company location?
![](https://github.com/blessingekwere/Data-Science-Salary/blob/main/How%20many%20employees%20are%20not%20resident%20in%20their%20company%20location.png)

![](https://github.com/blessingekwere/Data-Science-Salary/blob/main/employees%20not%20resident%20in%20company%20location%20-%20Copy.png)


*	Which job titles have the highest number of staff?
![](https://github.com/blessingekwere/Data-Science-Salary/blob/main/Which%20job%20titles%20have%20the%20highest%20number%20of%20staff.png)
This query shows that the job title with the highest number of staff is Data Engineer


* 	What is the number of staff by year?
![](https://github.com/blessingekwere/Data-Science-Salary/blob/main/9.png)

This query showed that the number of staff by year kept increasing with the 2023 recording the highest number of staff of 1785 and 2020 recording the least of 76


### Visualization
![](https://github.com/blessingekwere/Data-Science-Salary/blob/main/Data%20Science_page-0001%20-%20Copy.jpg)

You can clich [here](https://app.powerbi.com/groups/me/reports/9f492943-3d5f-44fe-b282-92a9629d061e) to interact with the dashboard
###### Dashboard

### INSIGHTS
*	Companies classified as medium-sized paid the highest salary of $451,290,619, followed by companies categorized as large, which paid a total of $53,708,646, and companies categorized as small paid a total salary of $11,577,549.

*	Data Engineers earned the highest salary with a total of $148.5M, followed by data scientists with a total of $118.3M.

*	The median salary for data scientists in the year 2023 was $143.18K.

*	The average salary for an experienced professional is $196,161, while that of an entry-level professional is $160,489. The average salary for mid-level professionals and entry-to-mid-level professionals is $95,825 and $71,533, respectively.

*	81 full-time employees and 10 contract employees do not reside in their company locations.

*	The top 5 regions that pay the highest salaries are the United States of America with a total of $461,538,909, followed by Great Britain with a total of $14,945,089. Canada, Germany, and Spain pay a total salary of $11,476,839, $4,944,173, and $4,441,057, respectively.

*	Looking at salaries by year, the lowest salary was paid in the year 2020 with a total of $7,015,000, while in 2021, 2022, and 2023, the salaries paid resulted in a total of $21,640,058, $221,875,465, and $226,046,291, respectively.

*	The United States of America is the country with the highest number of employees.

*	Considering the total number of employees by experience, entry-level professionals are the largest group at 67%, followed by mid-level professionals at 21.44%. Entry-to-mid-level professionals and experienced professionals make up 8.52% and 0.11%, respectively.

*	I conducted a predictive analysis on salaries for the next five years, and the results showed that there will be a 43.72% decrease in salary in 2024, followed by a 122.89% increase in 2025. In 2026, there will be a 13.16% increase in salary, and in 2027 and 2028, there will be increases of 20.36% and 79.6%, respectively.

![](https://github.com/blessingekwere/Data-Science-Salary/blob/main/Salary%20prediction%20for%20the%20next%205%20years.png)
###### Visual showing salary prediction for the next five years

*	I also conducted a predictive analysis on the number of employees for the next five years, and the results showed that there will be an 80.48% increase in 2024, followed by a 4.5% increase in 2025. In 2026, there will be a 42.39% increase in the number of employees, and in 2027 and 2028, there will be increases of 3.84% and 28.1%, respectively.
![](https://github.com/blessingekwere/Data-Science-Salary/blob/main/Staff%20strength%20prediction%20for%20the%20next%205%20years%20-%20Copy.png)
###### Visual showing staff strength prediction for the next five years


### Conclusion and Recommendation
Based on the insights from your data science salaries 2023 analysis, here are some recommendations:
*	Companies should consider re-evaluating their salary structure to ensure that they are paying competitive salaries. Small-sized companies, in particular, should consider reviewing their salaries to ensure that they remain competitive with larger companies in their industry.

*	Professionals looking to maximize their earning potential should consider pursuing a career as a data engineer, as they are currently earning the highest salaries in the industry.

*	Companies looking to attract and retain top talent in the data science industry should consider offering salaries that are at least equal to or higher than the median salary for data scientists in 2023, which was $143.18K.

*	Companies should consider tailoring their salary offerings to different levels of experience. For instance, entry-level professionals are the largest group in the industry and should be offered salaries that reflect this, while experienced professionals should be offered salaries that reflect their level of expertise.

*	Companies should also consider offering remote work options to employees who do not reside in their company locations. This can help them attract top talent from all over the world.

*	companies looking to expand their operations should consider focusing on regions that offer higher salaries, such as the United States of America, Great Britain, Canada, Germany, and Spain. However, it's also important to keep an eye on other countries with emerging prospects, as they may become competitors to the leading countries in the near future.

*	Companies should be prepared for the predicted changes in salaries and number of employees over the next five years. For example, in 2024, there will be a 43.72% decrease in salary, so companies should be prepared to adjust their budgets 

Thank you for going through this documentation.

Your thoughts and recommendation will be highly appreciated🤩

Kindly connect with me on [LinkedIn](https://www.linkedin.com/in/blessing-ekwere-857326216) and [Twitter](https://twitter.com/Eddie_Gregs?t=dF3996shVxvPJTePTtxDdw&s=09)
