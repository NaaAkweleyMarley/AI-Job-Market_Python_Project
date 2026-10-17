# A Tour of the AI Labour Market
### AI Job Market Analysis: Descriptive, Diagnostic, Prescriptive & Predictive Insights

#### About the Project

**A Tour of the AI Labour Market** is a Python-based data analysis project that explores salaries, in-demand skills and geographical trends in AI job postings.

The project covers four types of analytics: Descriptive, Diagnostic, Prescriptive and Predictive Analytics.

#### Project Overview

- Dataset obtained from Kaggle
- 15,000 rows and 19 columns
- Data was cleaned in Python to ensure readiness for analysis
- Types of analytics performed include: Descriptive, Diagnostic, Prescriptive and Predictive Analytics

#### Project Objectives

1. Analyze distribution of salaries across experience, education, and company size.
2. Identify top-paying industries and job roles.
3. Examine how benefits score, years of experience, and remote ratio relate to salaries.
4. Explore most in-demand skills.
5. Visualize geographical trends in AI job salaries.


#### Dataset Overview & Cleaning

- Checked for missing values and duplicates
- Cleaned text (standardized job titles and skills)
- Standardized data types across columns

The dataset contains 19 columns: job_id, job_title, salary_usd, salary_currency, experience_level, employment_type, company_location, company_size, employee_residence, remote_ratio, required_skills, education_required, years_experience, industry, posting_date, application_deadline, job_description_length, benefits_score and company_name.

#### Analysis Components

##### 1. Descriptive and Diagnostic Analytics — Objective 1: Salary Distribution by Experience, Education, and Company Size

- **Experience level:** Senior-level (SE and EX) roles have the highest median salaries.
- **Education level:** PhD-level roles show wider salary variation.
- **Company size:** Larger companies tend to pay more consistently.

##### 2. Objective 2: Top Paying Industries and Roles

**Top 10 Highest-Paying Industries (average salary)**

| Industry | Salary (USD) |
|---|---|
| Consulting | 117,602 |
| Manufacturing | 116,163 |
| Media | 116,128 |
| Education | 116,027 |
| Real Estate | 115,919 |
| Technology | 115,832 |
| Government | 115,694 |
| Finance | 115,323 |
| Telecommunications | 115,291 |
| Energy | 115,188 |

AI Research (Consulting) and Cloud Computing (Manufacturing) roles lead the salary charts.

**Top 10 Highest-Paying Job Titles (average salary)**

| Job Title | Salary (USD) |
|---|---|
| AI Specialist | 120,571 |
| Machine Learning Engineer | 118,828 |
| Head of AI | 118,543 |
| AI Research Scientist | 117,898 |
| AI Architect | 117,437 |
| Robotics Engineer | 116,471 |
| Principal Data Scientist | 116,305 |
| Research Scientist | 116,067 |
| Data Engineer | 115,971 |
| Data Scientist | 115,819 |

AI Specialists and ML Engineers earn top-tier pay.

##### 3. Objective 3: Salary Relationships

- **Benefits score vs salary:** Benefits score slightly influences salary levels.
- **Years of experience vs salary:** Years of experience shows moderate positive correlation with salary.
- **Remote ratio vs salary:** Remote ratio has weak correlation, showing that remote jobs can pay competitively.

**Correlation Matrix (Salary and Numeric Features)**

| | salary_usd | benefits_score | years_experience | remote_ratio |
|---|---|---|---|---|
| salary_usd | 1.00 | 0.00 | 0.74 | 0.01 |
| benefits_score | 0.00 | 1.00 | -0.01 | 0.00 |
| years_experience | 0.74 | -0.01 | 1.00 | 0.02 |
| remote_ratio | 0.01 | 0.00 | 0.02 | 1.00 |

##### 4. Objective 4: Most In-Demand Skills

**Top 15 Most In-Demand AI Skills**

| Skill | Count |
|---|---|
| Python | 4,450 |
| SQL | 3,407 |
| TensorFlow | 3,022 |
| Kubernetes | 3,009 |
| Scala | 2,794 |
| PyTorch | 2,777 |
| Linux | 2,705 |
| Git | 2,631 |
| Java | 2,578 |
| GCP | 2,442 |
| Hadoop | 2,419 |
| Tableau | 2,341 |
| R | 2,311 |
| Computer Vision | 2,284 |
| Data Visualization | 2,270 |

Python, SQL, and Machine Learning appear in most AI job postings.

##### 5. Objective 5: Geographical Trends

**Top 10 Company Locations by Average Salary**

| Location | Salary (USD) |
|---|---|
| Switzerland | 170,639 |
| Denmark | 165,652 |
| Norway | 159,491 |
| United States | 146,833 |
| United Kingdom | 128,720 |
| Singapore | 128,004 |
| Netherlands | 126,750 |
| Sweden | 123,560 |
| Germany | 121,810 |
| Australia | 118,239 |

US and Western Europe dominate high-paying AI markets. Emerging hubs include Australia, Germany, and Singapore.

##### 6. Salary Forecasting Model — Predictive Analytics (Machine Learning)

- **Model Used:** Linear Regression
- **Target:** salary_usd
- **Predictors:** experience_level, education_required, company_size, remote_ratio, benefits_score, and industry

| Metric | Result |
|---|---|
| R² | 0.64 (model explains ~64% of salary variance) |
| MAE | 27,051 (average error) |
| MSE | 1.3 billion |

**Interpretation:** The model performs reasonably well for estimating salary ranges.

##### 7. Prescriptive Analytics (Recommendations)

**For Job Seekers**

- Learn in-demand skills like Python, SQL and Machine Learning, and pair them with the experience level, role and industry you're targeting.
- Apply for jobs in bigger companies or senior roles because they usually offer higher salaries and more career growth.

**For Employers**

- Check how much other companies pay for similar roles in the region so your salaries remain attractive to skilled professionals.
- Provide good benefits and flexible working options (like remote work). These make jobs more appealing to AI and tech experts.
- Invest in employee training to help your current staff build AI and data skills instead of only hiring new talent.

**For Policymakers and Universities**

- Create more programs and courses in AI, data science, and digital skills to prepare students for the growing AI job market.
- Support partnerships between universities and tech companies so students can gain hands-on experience through internships or projects.
- Encourage remote and international job opportunities to connect local talent with global employers and boost digital employment.

#### Takehome Points

1. In this dataset, salary patterns vary with experience, company size, industry and location.
2. Python, SQL and Machine Learning appear most often in job postings. That shows demand for these skills, but it doesn't show they earn higher pay on their own.
3. A skill's value depends on context: who has it, the role, the industry, the region and the level of experience. Job seekers, employers and educators should look at those conditions, not only at skill lists.

#### Conclusion

This analysis of 15,000 AI job records shows that salaries vary with experience, company size, industry and location, and that Python, SQL and Machine Learning appear most often in job postings. Frequency alone doesn't make a skill valuable. Its worth depends on who has it, the role, the industry, the region and the level of experience.

Even this salary model, which explains about 64% of the variance, is best used to estimate ranges rather than exact figures. The better question is not "What skill should I learn?" but "Under what conditions does a skill become valuable?"

#### Tools Used

- **Python** — Data cleaning, analysis and machine learning
- **JupyterNotebook** — Development environment

#### Visualisations

- Box plots
- Horizontal bar charts
- Scatter plots
- Correlation heatmap

#### Project Summary
**A Tour of the AI Labour Market** is an end-to-end Python data engineering and machine learning project that dissects compensation architecture, talent distribution, and structural hiring mechanics across 15,000 global AI job profiles. 
Moving beyond static data aggregates, this project builds a complete analytics lifecycle to determine what truly drives valuation in the contemporary artificial intelligence workforce.

The analytical framework is categorized into four distinct processing tiers:

• **Descriptive Analytics**: Mapping global salary benchmarks across experience levels, education baselines, and scaling organizational tiers.

• **Diagnostic Analytics**: Pinpointing structural correlations, isolating high-earning industry verticals (such as Consulting and Manufacturing), and establishing geographical premium variances led by Switzerland, Denmark, and the United States.

• **Predictive Analytics**: Structuring a multi-variable Linear Regression model that reliably factors core features—including experience, education tiers, and enterprise footprints—to explain 64% of salary variance (\(R^2 = 0.64\)).

• **Prescriptive Analytics**: Coding data-backed operational frameworks tailored for market stakeholders, transforming workforce data into practical roadmaps for job seekers, corporate compensation leaders, and academic policymakers.

A key finding of this pipeline is that, while foundational tools like Python, SQL, and Machine Learning architectures populate the highest operational frequency across job profiles, raw frequency does not inherently equal a salary premium. 
The findings demonstrate that skill valuation is contextual and highly dependent on a localized intersection between regional hubs, target industries, and senior leadership experience tiers.


#### Author:
#### Naa Akweley Marley
LinkedIn: [Naa Akweley Marley](https://www.linkedin.com/in/naa-akweley-marley)