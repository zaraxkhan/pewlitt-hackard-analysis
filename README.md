# Pewlitt-Hackard-Analysis
Pewlitt Hackard is a large company boasting over thousands of employees and has been around for a long time. As baby-boomers begin to retire at a rapid pace, Pewlitt Hackard is looking toward the future. First it is offering a retirement package to eligible employees and also asking questions such as which positions will become soon availible due to this retirement wave as thousands of positions will become open. Bobby is an HR hire and is tasked with figuring out who will be retiring within the next year and how many positions will become availible. With my help, he will come up with a list of employees who will be retiring and build an employee database. 

## Overview
With the Use of SQL and PGAdmin 4, I will be aiding Bobby and his company to help determine the number of retiring employees per title, and identify employees who are eligible to participate in a mentorship program. This information will help Pewlitt Hackard prepare for the 'silver tsunami' of employees who will be getting ready to retire shortly. The mentorship program will ease the transition for new employees to fill the shoes of those before them. 

## Results
Below are the results from the analysis. 

### Figure 1: Retirement Titles

![retirement_titles](https://user-images.githubusercontent.com/105755095/180590625-b1b78f1e-5623-4b32-b5df-81b9bd34c0ea.png)

The first analysis I ran shared which employees, along with their title and start dates, were eligible to retire within the next few years. I ran this analysis by filtering the birth dates between 1/1/1952 and 12/31/1965 as this age group would be retiring in a few years. Figure 1, above, shows this data. However, many employees are duplicated within this analysis as they have moved positions or departments and have multiple titles throughout the company. Because of this, employee names are repeated and does not give the exact number of actual employees leaving. 

### Figure 2: Unique Titles

![unique_titles](https://user-images.githubusercontent.com/105755095/180590679-ba5ee54a-8435-45da-8fd9-d43ae7671859.png)

Because the first analysis had many repeats, I re-did the query in order to share employees without their multiple titles. This cut the rows in almost half, as the results went from 133,776 rows in the retirement titles to 72,458 rows with these unique titles. From this analysis, we were able to figure out the exact number of employees that will be retiring shortly with their title. 

### Figure 3: Retiring Titles

![retiring_titles](https://user-images.githubusercontent.com/105755095/180590803-74040ce1-0401-4ab2-ac2e-52f9ebbebd40.png)

This analysis gave a quick overview of exactly how many new hires Pewlitt Hackard will need to fill based on the job titles. From a glance, we can see that they will need to fill the role of Senior Engineer with over 25,000 new employees. With some quick calculations, we determined that this company will have about 72,458 roles to fill very shortly. 

### Figure 4: Mentorship Eligibility

![mentorship_eligibility](https://user-images.githubusercontent.com/105755095/180590904-337f5a80-2372-4a55-ab81-69dd37fa05ff.png)

The last analysis for this challenge shared the titles of the employees who are at retiring age but have not left the company or put in their retirement notice. This employee database shares all the employees who are eligible to be a part of the mentorship program that will help ease the transition for the employees that they will be hiring in the near future. There are about 1,548 eligible employees for this mentorship program. 


## Summary

### How many roles will need to be filled as the "silver tsunami" begins to make an impact?
When we ran the "Retiring Titles" analysis, the number of rows that appeared were 75,428. This means that there will be over 75,000 openings very soon. I ran an additional analysis to count how many vacancies will be opening per department. This table is show below and under the "Retiring Dept" csv file. This query will help each department prepare for hiring so each area knows how many new employees they should expect to train very soon.  

### Figure 5: Retiring Department Count
![retiring_dept](https://user-images.githubusercontent.com/105755095/180626073-a0de3edf-2f1d-4173-b1b5-f339db74fdd7.png)

### Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees?
With the mentorship eligibility analysis we had done, it came out with around 1,548 employees who are not yet retired and would be able to stay and help out with training the new employees. However, this is not enough. As we saw in the previous analysis titled 'Retiring Titles', we counted around 75,428 staff will be retiring soon. There are way too many vacancies that will soon be open and not enough eligible employees to help mentor them all. With a quick calculation (75,428/1,548) each mentor would have to have around 46 employees to train in order to fill the job openings, which is impossible. I ran an additional analysis which shows how many mentors are availible per Department. Below is Figure 6 which shares the table of how many employees are avalible per department to mentor. This analysis goes hand and hand with retiring titles, as this analysis shares how many spots will soon become availible and how many staff are eligible to mentor. The difference is staggering and Pewlitt Hackard will have to come up with an additional plan in order to have a smooth transition of training the new wave of employees soon. 

Figure 6: Mentor Count per Department

![mentor_count](https://user-images.githubusercontent.com/105755095/180626305-42fddddb-a12a-4aee-8ca0-6e9994d0cb55.png)
