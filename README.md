
## Team Members
- Julia Gild [@JuliaGild](https://github.com/JuliaGild)
- John Neely [@NeelyJohn](https://github.com/NeelyJohn)
- Valerie Tran [@ValerieTran](https://github.com/vvt15)
- Jack Glawatz [@jackglawatz](https://github.com/jackglawatz)
- Oluwabukola Ogundare [@RachaelOgundare](https://github.com/RachaelOgundare)


## Data Set
- Employee Salaries - 2024
https://catalog.data.gov/dataset/employee-salaries-2024

## Problem Description
- The dataset titled “Employee Salaries - 2024” contains detailed information about employee compensation across various departments and divisions.
-  It includes a total of 10,398 rows and 8 columns, each representing a different attribute related to employee salary data. The data was obtained from the US Government Database. The columns in the dataset are as follows: Department, which provides the abbreviated name of the department; Department Name, which gives the full name of the department; and Division, which refers to specific teams or units within each department. The Gender column identifies whether the employee is male (M) or female (F). Salary-related information includes Base Salary, which is a float data type representing the employee's annual base pay, 2024 Overtime Pay for any additional earnings from extra hours worked, and 2024 Longevity Pay, which accounts for bonus payments based on years of service. Lastly, the Grade column indicates the employee’s job level or classification (such as M3, EX2, or N17), although this field contains some missing values. Overall, this dataset provides a comprehensive snapshot of employee compensation, allowing for in-depth analysis of salary structures, gender pay comparisons, and departmental compensation trends.



## Question 1: What departments have the greatest nominal gender pay gap?
<img width="1500" alt="Screenshot 2025-04-27 at 6 17 19 PM" src="https://github.com/user-attachments/assets/87ba99b3-8696-4083-b6c0-661f76d7f581" />

- 📄 [Book2 (3) (7).twbx](./Book2%20(3)%20(7).twbx)

### Importance
- Our chart shows the nominal gender pay gap across various departments, with positive values showing males who earn more on average than females. The calculation is based on the difference between the average total compensation for females in each department.

### Analysis
- Looking at our data visual, departments showing the greatest male advantage in pay are; NFB, which has an extremely large pay gap favoring males, standing out by far among other  departments, CBK, ECM, and CAT; these departments are technical and highly specialized, and also show a substantial male advantage. Other administrative departments, such as OA,S have smaller or even reversed pay gaps, which could highlight differences in role types or seniority levels by gender. Overall, the results shown in our model highlight where gender-based pay disparities are more notable and suggest a need for further analysis in the hiring, promotion, and pay practices in most departments, especially the ones mentioned above.

### Manipulations
- To analyze the gender pay gap by department, a new calculated field called "Gender Pay Gap" was created in Tableau. This calculation compared the average total compensation of male and female employees within each department. Specifically, it used an IF statement to separately find the average total compensation for males and for females, then subtracted the female average from the male average. A positive result shows that, on average, males earn more than females in that department. A negative result would show a female pay advantage. This step was necessary because the original dataset only listed individual salaries and did not directly provide a gender comparison. By creating this calculated field, it became possible to visualize the pay gap clearly in a horizontal bar chart, making department-level differences easy to identify.
<img width="331" alt="Screenshot 2025-04-27 at 6 17 30 PM" src="https://github.com/user-attachments/assets/4ba93af7-875a-44be-8c5b-2c8183d5ffa7" />



  
## Question 2: Which departments rely most on lower-paid employees for overtime work?
<img width="1500" alt="Screenshot 2025-04-27 at 6 30 00 PM" src="https://github.com/user-attachments/assets/4014f2f3-ff3a-4500-acef-3af3d53563b3" />
- 📄 [Book2 (3) (8).twbx](./Book2%20(3)%20(8).twbx)

### Importance
- This bar chart shows the total 2024 overtime pay for employees in each department who earn below the median base salary. Base pay was selected as the appropriate metric instead of total compensation, so we could isolate the overtime variable, which would have been included in the total compensation metric. By focusing only on employees earning less than the median, the graph highlights where lower-paid employees contribute significantly to departmental overtime hours. By hiring more workers to cover these overtime shifts, the department could reduce the overall salary expense, as the same number of hours would be worked but with a lower average rate.

### Analysis
- From the visualization, we can see that certain departments, like the Department of Police and Fire and Rescue Service, have much higher overtime totals compared to others. This suggests that lower-paid workers in these departments are heavily relied upon to work extra hours. It raises questions about workload distribution, employee well-being, and whether overtime is being used as a long-term staffing solution for these essential services. Departments with little to no overtime pay among below-median earners could indicate either a better balance or possibly stricter overtime management. Understanding where overtime is concentrated among lower-paid employees is essential for ensuring fair compensation practices and identifying departments that may need better staffing or support. If this model has been relied upon for long-term staffing instead of a short-term solution, then the department’s salary expense could be reduced considerably by hiring additional workers, preventing the need to pay a higher rate during overtime.

### Manipulations
- To display only individuals whose base salary was lower than the median base salary in the dataset, a fixed calculated field had to be created first to act as a point of comparison for a secondary calculation.
- A second calculated field that returns True/False was then created to filter by wages.
- The “Below Median | Filter” field was placed into the ‘filter’ section with the ‘true’ value selected.

