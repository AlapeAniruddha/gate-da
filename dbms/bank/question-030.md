---
title: Question-30
pagetitle: Question-30
categories: [DBMS]
---

Consider the table **employee**(empId, name, department, salary) and the two queries   
𝑄1,𝑄2  below. Assuming that department 5 has more than one employee, and we want to find the employees who get higher salary than anyone in the department 5, which one of the statements is **TRUE** for any arbitrary employee table?

| 𝑄1: | Select e.empId From employee e Where not exists     (Select \* From employee s Where s.department \= "5" and s.salary \>= e.salary)  |
| :---: | ----- |
| 𝑄2: | Select e.empId From employee e Where e.salary \> Any     (Select distinct salary From employee s Where s.department \= "5")  |

- [ ] 𝑄1 is the correct query  
- [ ] 𝑄2 is the correct query  
- [ ] Both 𝑄1 and 𝑄2 produce the same answer  
- [ ] Neither 𝑄1 nor 𝑄2 is the correct query

::: {.callout-note title="Answer" collapse=true}

- [x] 𝑄1 is the correct query  
- [ ] 𝑄2 is the correct query  
- [ ] Both 𝑄1 and 𝑄2 produce the same answer  
- [ ] Neither 𝑄1 nor 𝑄2 is the correct query

:::

