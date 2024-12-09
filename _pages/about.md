---
permalink: /
title: "About me"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Hi, I am Xiaolong Li, a research assistant and advised by Professor Reynold C.K. Cheng at the University of Hong Kong. I am interested in Text-to-SQL, Data Science Code Generation, LLM Agent. 

## Education

- **The University of Hong Kong**  
  *Master of Science in Computer Science (General Track)*  
  **Nov 2024**  
  - Overall GPA: 3.8/4.0  
  - Graduate with **Distinction**

- **The University of British Columbia**  
  *Bachelor of Science in Computer Science*  
  **Mar 2023**  
  - Overall GPA: 3.8/4.0  
  - **Dean’s Honour List** (Nov 2021)  
  - Graduate with **Distinction**

## Research Experience
### [BIRD-SQL](https://bird-bench.github.io/): Data Quality Check, Submission Evaluation, and Metric Analysis & Optimization  

**May 2024 — Aug 2024**  

- Performed comprehensive data quality checks on the BIRD dataset development set to ensure data integrity and consistency.
- Evaluated more than 30 submissions from companies and universities, including cutting-edge text-to-SQL parsers from [Google Cloud](https://arxiv.org/abs/2410.01943), AT&T, and [Distyl AI](https://arxiv.org/abs/2408.07702) on the BIRD benchmark.
- Developed two novel text-to-SQL evaluation metrics:
  - **Soft-F1 score**: A more lenient metric that reduces the impact of column order and missing values in the tables produced by predicted SQL queries, providing a more accurate assessment of parser performance.
  - **R-VES (Reward-based VES)**: A metric for measuring the efficiency of text-to-SQL parsers using discrete functions.

---

### [BIRD-SQL Mini-Dev](https://github.com/bird-bench/mini_dev): A Multilingual, Lightweight Version of the BIRD Development Set   
**May 2024 — Aug 2024**  

- Designed the Mini-Dev dataset to facilitate efficient and cost-effective development cycles.
- Reduced the development set size from 1,534 to 500 examples by prioritizing error correction and ensuring a balanced difficulty distribution. The subset includes all relevant keywords as outlined in the BIRD benchmark and samples across all databases.
- Enhanced the practicality of the BIRD system by supporting multiple SQL dialects, including MySQL and PostgreSQL, to better align with industry applications.
- Collaborated with Arcwise, an AI data analysis company, to conduct a comprehensive analysis of the BIRD Mini-Dev dataset, further improving the dataset's robustness and reliability.
- Evaluated Mini-Dev baseline performance on over 10 models, demonstrating comparable performance to the full test set and confirming its representativeness of the BIRD dataset's features and attributes.

## Work Experience
### Teaching Assistant / Introduction to Relational Databases  
**Department of Computer Science, The University of British Columbia**  
**July 2022 — Dec 2022**  
- Assisted professor in lecture preparation, including topics such as database systems, ER models, normalization, formal relational query language, and SQL, as well as curriculum discussions and student feedback collection.
- Graded assignments, mentored group projects, and maintained workflow.