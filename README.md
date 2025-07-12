# Equality Score Classification – Excel Task

This project contains a simple Excel-based data cleaning and classification task completed as part of the **Deloitte Data Analytics Virtual Internship**.

## 📌 Task Overview

We were given a dataset with the following columns:
- Factory
- Job Role
- Equality Score (ranging from -100 to +100)

### Objective:
Add a 4th column named `Equality Class`, based on the following logic:

| Equality Score Range       | Classification           |
|----------------------------|---------------------------|
| Between -10 and +10        | Fair                      |
| Between -20 and -11 OR 11 to 20 | Unfair               |
| Less than -20 OR greater than 20 | Highly Discriminative |

### 🛠 Tools Used:
- Microsoft Excel
- Formula used:  
  ```excel
  =IF(ABS(C2)<=10, "Fair", IF(ABS(C2)<=20, "Unfair", "Highly Discriminative"))
