
## Team Members
[Julia Gild](https://github.com/JuliaGild)  
[John Neely](https://github.com/NeelyJohn)  
[Valerie Tran](https://github.com/vvt15)  
[Jack Glawatz](https://github.com/jackglawatz) 

[Oluwabukola Ogundare](https://github.com/RachaelOgundare)


## Data set
- Employee Salaries - 2024
https://catalog.data.gov/dataset/employee-salaries-2024

## Problem Description
- The dataset titled “Employee Salaries - 2024” contains detailed information about employee compensation across various departments and divisions.
-  It includes a total of 10,398 rows and 8 columns, each representing a different attribute related to employee salary data. The data was obtained from the US Government Database The columns in the dataset are as follows: Department, which provides the abbreviated name of the department; Department Name, which gives the full name of the department; and Division, which refers to specific teams or units within each department. The Gender column identifies whether the employee is male (M) or female (F). Salary-related information includes Base Salary, which is a float data type representing the employee's annual base pay, 2024 Overtime Pay for any additional earnings from extra hours worked, and 2024 Longevity Pay, which accounts for bonus payments based on years of service. Lastly, the Grade column indicates the employee’s job level or classification (such as M3, EX2, or N17), although this field contains some missing values. Overall, this dataset provides a comprehensive snapshot of employee compensation, allowing for in-depth analysis of salary structures, gender pay comparisons, and departmental compensation trends.



## Question 1
Question 1: What departments have the greatest nominal gender pay gap?

<img width="627" alt="Screenshot 2025-04-27 at 6 17 19 PM" src="https://github.com/user-attachments/assets/87ba99b3-8696-4083-b6c0-661f76d7f581" />

<img width="331" alt="Screenshot 2025-04-27 at 6 17 30 PM" src="https://github.com/user-attachments/assets/4ba93af7-875a-44be-8c5b-2c8183d5ffa7" />

- 📄 [Book2 (3) (7).twbx](./Book2%20(3)%20(7).twbx)



Our chart shows the nominal gender pay gap across various departments, with positive values showing males that earn more on average than females. The calculation is based on the difference between the average total compensation for females in each department.

Looking at our data visual, departments showing the greatest male advantage in pay are; NFB, which has an extremely large pay gap favoring males standing out by far among other  departments, CBK, ECM, and CAT; these departments are technical and highly specialized and also show a substantial male advantage. Other administrative departments such as OAS have smaller or even reversed pay gaps, which could higlhight differences in role types or seniority levels by gender.

Overall, the results shown in our model highlight where gender-based pay disparities are more notable and suggest a need for further analysis in the hiring, promotion, and pay practices in most departments, espically the ones mentioned above.


The manipulations applied to the dataset as part of the analysis:
- To analyze the gender pay gap by department, a new calculated field called "Gender Pay Gap" was created in Tableau. This calculation compared the average total compensation of male and female employees within each department. Specifically, it used an IF statement to separately find the average total compensation for males and for females, then subtracted the female average from the male average. A positive result shows that, on average, males earn more than females in that department. A negative result would show a female pay advantage. This step was necessary because the original dataset only listed individual salaries and did not directly provide a gender comparison. By creating this calculated field, it became possible to visualize the pay gap clearly in a horizontal bar chart, making department-level differences easy to identify



  
## Question 2
Question 2: Which departments rely most on lower-paid employees for overtime work?

📄 [Book2 (3) (8).twbx](./Book2%20(3)%20(8).twbx)

<img width="1439" alt="Screenshot 2025-04-27 at 6 30 00 PM" src="https://github.com/user-attachments/assets/4014f2f3-ff3a-4500-acef-3af3d53563b3" />
