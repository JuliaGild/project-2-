
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
- The dataset titled “Employee Salaries - 2024” contains detailed information about employee compensation across various departments and divisions. It includes a total of 10,398 rows and 8 columns, each representing a different attribute related to employee salary data. The data was obtained from the US Government Database The columns in the dataset are as follows: Department, which provides the abbreviated name of the department; Department Name, which gives the full name of the department; and Division, which refers to specific teams or units within each department. The Gender column identifies whether the employee is male (M) or female (F). Salary-related information includes Base Salary, which is a float data type representing the employee's annual base pay , 2024 Overtime Pay for any additional earnings from extra hours worked, and 2024 Longevity Pay, which accounts for bonus payments based on years of service. Lastly, the Grade column indicates the employee’s job level or classification (such as M3, EX2, or N17), although this field contains some missing values. Overall, this dataset provides a comprehensive snapshot of employee compensation, allowing for in-depth analysis of salary structures, gender pay comparisons, and departmental compensation trends.



## Question 1
Question 1: Which departments have the highest average total compensation (base + longevity + overtime), and how does it differ by gender?

<img width="623" alt="Screenshot 2025-04-21 at 7 39 33 PM" src="https://github.com/user-attachments/assets/9f10b8ae-3376-45b2-8659-7e979c0b7515" />

[Download Tableau Workbook: Book2 (3) (4).twbx](./Book2%20(3)%20(4).twbx)


- This shows you which departments may have pay gaps or higher overall compensation levels across genders
- Total compensation was calculated by the following: (base + longevity + overtime)
- We calculated the total compensation because it shows the complete amount of money an employee earns, not just their base salary. This helps give a full picture of employee earnings, which helps when comparing compensation across departments and identifying pay disparities
- This analysis reveals which departments offer the highest overall compensation when combining base salary, longevity pay, and overtime pay. Breaking down the results by gender also highlights potential pay disparities between men and women within the same department. This helps identify departments with the most competitive pay structures and uncovers any possible gender-based inequalities in total compensation


## Question 2
Question 2:What departments have the greatest nominal gender pay gap?

[Download Tableau Workbook: Book2 (3) (5).twbx](./Book2%20(3)%20(5).twbx)
<img width="766" alt="Screenshot 2025-04-21 at 8 06 04 PM" src="https://github.com/user-attachments/assets/22918617-ad07-45e0-81ec-9ac67f3c5a5d" />
<img width="274" alt="Screenshot 2025-04-21 at 9 18 39 PM" src="https://github.com/user-attachments/assets/177c90c2-135f-4a65-87f4-b3e363ca6fad" />

- This visualization reveals the departments with the largest gender-based differences in total compensation. The positive values indicate that there is a higher pay for men while the negative values show a higher pay for women. By isolating the pay gap itself, this view highlights where compensation imbalances are most pronounced based on gender.
- Each bar represents the gender pay gap in a specific department.
- The longer the bar, the larger the gap in favor of that gender.
- The chart helps visually identify which departments have the largest disparities
- After using the formula to calculate the gender pay gap: Positive → Men earn more than women in that department, Negative → Women earn more than men in that department, Zero → No gender pay gap; compensation is equal
