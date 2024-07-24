# 2024_IA651_RSDJ_final_project
Repository for final project from Rakshith and Dhanumjay 

<H1> TITLE : LOAN DEFALUT PREDICTION  </H1>
<H2> FINAL PROJECT IA651</H2>
<H4> RAKSHITH AND DHANUMJAY </H4>

<h4>ABSTRACT</h4>
        <p>In today's fast-paced world, accurate risk assessment is crucial for financial institutions to mitigate potential losses and ensure sustainable growth. This project focuses on developing a robust machine learning model to predict the risk associated with individuals based on various socio-economic and demographic factors. The dataset used comprises detailed information on individuals' <span class="highlight">income, age, experience, marital status, house and car ownership, profession, city, state, current job years,</span> and <span class="highlight">current house years.</span></p>
        <p>The training dataset includes a 'Risk_Flag' which indicates whether an individual is considered a risk or not. By analyzing this dataset, we aim to uncover patterns and relationships between the input features and the risk flag. The test dataset, devoid of the risk flag, is utilized to validate the model's predictive power.</p>
        <p>In this study, we employ a range of machine learning algorithms to identify the most effective model for risk prediction. The results of this project are expected to provide valuable insights for financial institutions, helping them to better assess and manage potential risks associated with their clients.</p>
<h4>OBJECTIVES</h4>
    <ul>
        <li><strong>Data Analysis and Preprocessing</strong>
            <ul>
                <li>Conduct a thorough exploratory data analysis (EDA) to understand the distribution, patterns, and relationships within the data.</li>
                <li>Identify and handle missing values by removing or imputing them to ensure data integrity.</li>
                <li>Handle outliers and perform necessary data cleaning to ensure data quality.</li>
                <li>Encode categorical variables and normalize numerical features to prepare the data for modeling.</li>
            </ul>
        </li>
        <li><strong>Feature Selection and Engineering</strong>
            <ul>
                <li>Identify the most relevant features that contribute to predicting the risk flag.</li>
                <li>Create new features or transform existing ones to enhance the model's predictive power.</li>
            </ul>
        </li>
        <li><strong>Model Development and Evaluation</strong>
            <ul>
                <li>Develop multiple machine learning models including logistic regression, decision trees, random forests, and gradient boosting to predict the risk flag.</li>
                <li>Train and validate these models using appropriate metrics such as accuracy, precision, recall, and F1-score.</li>
                <li>Perform hyperparameter tuning to optimize the performance of the selected models.</li>
            </ul>
        </li>
        <li><strong>Model Comparison and Selection</strong>
            <ul>
                <li>Compare the performance of different models and select the one with the best predictive accuracy and generalizability.</li>
                <li>Analyze the feature importance to understand the key factors influencing risk prediction.</li>
            </ul>
        </li>
        <li><strong>Deployment and Interpretation</strong>
            <ul>
                <li>Develop a user-friendly interface or application to deploy the final model for practical use by financial institutions.</li>
                <li>Provide clear and actionable insights derived from the model to assist in decision-making processes.</li>
            </ul>
        </li>
        <li><strong>Documentation and Reporting</strong>
            <ul>
                <li>Document the entire process including data preprocessing steps, model development, evaluation results, and final conclusions.</li>
                <li>Prepare a comprehensive report summarizing the findings and recommendations for stakeholders.</li>
            </ul>
        </li>
    </ul> 
<h4>Introduction</h4>
    <p>In the financial sector, accurate risk assessment is essential for mitigating potential losses and ensuring sustainable growth. With the increasing availability of diverse data sources, machine learning has become a powerful tool for predicting risk and making informed decisions. This project aims to develop a robust machine learning model to predict the risk associated with individuals based on a variety of socio-economic and demographic factors.</p>
    <p>The dataset utilized in this project includes detailed information on individuals' income, age, experience, marital status, house and car ownership, profession, city, state, current job years, and current house years. By analyzing these features, the goal is to uncover patterns and relationships that can effectively predict whether an individual poses a risk.</p>
    <p>Through data preprocessing, feature engineering, and the development of various machine learning models, this project seeks to identify the most accurate and generalizable model. The findings and insights derived from this model will provide valuable tools for financial institutions to better assess and manage potential risks associated with their clients.</p>
<h4>DATA COLLECTION</h4>
    <p>The datasets employed in this project were found after a rigorous search for the best datasets on various platforms. These datasets were finally sourced from Kaggle and are frequently utilized for machine learning and data analysis endeavors, providing a solid foundation for developing predictive models.</p>
    <h4>Datasets</h4>
    <ul>
        <li><strong>Training Data</strong>
            <ul>
                <li><strong>Source</strong>: Kaggle</li>
                <li><strong>Description</strong>: This dataset comprises detailed information on individuals, encompassing a wide range of socio-economic and demographic attributes. Key features include income, age, professional experience, marital status, house ownership, car ownership, profession, city, state, current job duration, and current house duration. The target variable 'Risk_Flag' indicates whether an individual is considered a risk (1) or not (0).</li>
                <li><strong>Purpose</strong>: The training data is used to develop and train machine learning models aimed at predicting the risk flag based on the provided features.</li>
            </ul>
        </li>
        <li><strong>Test Data</strong>
            <ul>
                <li><strong>Source</strong>: Kaggle</li>
                <li><strong>Description</strong>: Similar to the training dataset, the test dataset includes comprehensive information on individuals with the same set of features, except for the 'Risk_Flag'. This allows for the assessment of the model's predictive accuracy.</li>
                <li><strong>Purpose</strong>: The test data is utilized to evaluate and validate the predictive performance and generalizability of the trained models.</li>
            </ul>
        </li>
    </ul>
    <h4>DATA FEATURES</h4>
    <ul>
        <li><strong>Income</strong>: Annual income of the individual.</li>
        <li><strong>Age</strong>: Age of the individual.</li>
        <li><strong>Experience</strong>: Number of years of professional experience.</li>
        <li><strong>Married/Single</strong>: Marital status of the individual.</li>
        <li><strong>House_Ownership</strong>: Status of house ownership (owned or rented).</li>
        <li><strong>Car_Ownership</strong>: Status of car ownership.</li>
        <li><strong>Profession</strong>: Professional occupation of the individual.</li>
        <li><strong>CITY</strong>: City of residence.</li>
        <li><strong>STATE</strong>: State of residence.</li>
        <li><strong>CURRENT_JOB_YRS</strong>: Number of years spent in the current job.</li>
        <li><strong>CURRENT_HOUSE_YRS</strong>: Number of years spent in the current house.</li>
        <li><strong>Risk_Flag</strong> (Training Data Only): Indicator of risk (1 for risk, 0 for no risk).</li>
    </ul>
    <h4>DATA PREPROCESSING</h4>
    <p>Prior to model training and validation, several essential preprocessing steps were carried out to ensure data quality and integrity:</p>
    <ul>
        <li><strong>Handling Missing Values</strong>: Any missing values within the datasets were identified and addressed through removal or imputation techniques to maintain dataset completeness.</li>
        <li><strong>Data Cleaning</strong>: Outliers and anomalies were managed, and necessary cleaning operations were performed to enhance data consistency and reliability.</li>
        <li><strong>Feature Encoding</strong>: Categorical variables were encoded using appropriate methods, and numerical features were normalized to facilitate effective machine learning model training.</li>
    </ul>
    <p>By sourcing and preprocessing the datasets from Kaggle, this project leverages a diverse and comprehensive dataset, thereby enabling the development of robust and accurate machine learning models for risk prediction.</p>

<h4>Age Distribution</h4>
        <p>The histogram shows the distribution of ages in the dataset, ranging from <span class="highlight">20 to 80 years</span>. The age groups are relatively evenly distributed, with each bin containing around <span class="highlight">20,000 to 25,000 individuals</span>. There's a slight dip in the <span class="highlight">40s and 50s</span> age bins, while the <span class="highlight">60s</span> have the highest count, exceeding 25,000 individuals. This balanced distribution suggests a well-represented dataset across different age groups, though the dip in the 40s and 50s may warrant further investigation.</p>
 <h4>Experience Distribution</h4>
        <p>The histogram shows the distribution of the <span class="highlight">experience</span> variable, ranging from 0 to 20 years. Most bins (0 to 17.5 years) have a relatively uniform count of <span class="highlight">20,000 to 25,000 individuals</span>. However, there's a significant spike at <span class="highlight">20 years</span>, with over 35,000 individuals. This suggests a large number of individuals have exactly 20 years of experience, which may warrant further investigation to ensure data accuracy and assess its impact on the risk prediction model.</p>
 <h4>Current Job Years Distribution</h4>
        <p>The histogram shows the distribution of <span class="highlight">current_job_yrs</span>:</p>
        <ul>
            <li><span class="highlight">Range</span>: 0 to 14 years.</li>
            <li><span class="highlight">Key Observations</span>:
                <ul>
                    <li>Peak at 4 years (~60,000 individuals).</li>
                    <li>Notable peaks at 8 and 10 years (~35,000-40,000 individuals).</li>
                    <li>Lower counts at 2, 6, 12, and 14 years (~10,000-20,000 individuals).</li>
                </ul>
            </li>
            <li><span class="highlight">Implications</span>: The peak at 4 years suggests many individuals have this job duration, which may impact risk assessment.</li>
            <li><span class="highlight">Next Steps</span>: Investigate the concentration at 4 years and its effect on the model.</li>
        </ul> 
  <h4>Current House Years Distribution</h4>
        <p>The histogram shows the distribution of <span class="highlight">current_house_yrs</span>:</p>
        <ul>
            <li><span class="highlight">Range</span>: 10 to 14 years.</li>
            <li>Peaks at 11 and 12 years (~50,000 individuals).</li>
            <li>Lower counts at 10, 13, and 14 years (~45,000-50,000 individuals).</li>
        </ul>
        <p>This indicates stable representation of house years with no significant outliers.</p>
  <h4>Risk Flag Distribution</h4>
        <p>The histogram shows the distribution of <span class="highlight">risk_flag</span>:</p>
        <ul>
            <li><span class="highlight">Range</span>: 0 (not a risk) and 1 (risk).</li>
            <li>Majority (over 200,000) have a risk flag of 0.</li>
            <li>Minority (under 50,000) have a risk flag of 1.</li>
        </ul>
        <p>This indicates class imbalance, with far more non-risk individuals than risk individuals.</p>
<h4>Income vs Risk Flag Analysis</h4>
        <p>The box plot shows the distribution of <span class="highlight">income</span> for each <span class="highlight">risk_flag</span> category:</p>
        <ul>
            <li>Median income is similar for both risk (1) and non-risk (0) groups.</li>
            <li>Both groups have a similar interquartile range and overall distribution.</li>
            <li>No significant outliers or differences between the two groups.</li>
        </ul>
        <h4>Age vs Risk Flag Analysis</h4>
        <p>The box plot shows the distribution of <span class="highlight">age</span> for each <span class="highlight">risk_flag</span> category:</p>
        <ul>
            <li>Median age is similar for both risk (1) and non-risk (0) groups.</li>
            <li>Both groups have a similar interquartile range and overall distribution.</li>
            <li>No significant outliers or differences between the two groups.</li>
        </ul>
        <h4>Experience vs Risk Flag Analysis</h4>
        <p>The box plot shows the distribution of <span class="highlight">experience</span> for each <span class="highlight">risk_flag</span> category:</p>
        <ul>
            <li>Median experience is similar for both risk (1) and non-risk (0) groups.</li>
            <li>Both groups have a similar interquartile range and overall distribution.</li>
            <li>No significant outliers or differences between the two groups.</li>
        </ul>
        <h4>Current House Years vs Risk Flag Analysis</h4>
        <p>The box plot shows the distribution of <span class="highlight">current_house_yrs</span> for each <span class="highlight">risk_flag</span> category:</p>
        <ul>
            <li>Median house years are similar for both risk (1) and non-risk (0) groups.</li>
            <li>Both groups have a similar interquartile range and overall distribution.</li>
            <li>No significant outliers or differences between the two groups.</li>
        </ul>
        <h4>Feature Comparison vs Risk Flag Analysis</h4>
        <p>The subplots compare various features against the <span class="highlight">risk_flag</span>:</p>
        <ul>
            <li><span class="highlight">Income</span>: Slightly higher for non-risk individuals across all categories.</li>
            <li><span class="highlight">Age, Experience, Current Job Years, Current House Years</span>: Similar distributions for both risk and non-risk individuals across all categories.</li>
            <li><span class="highlight">Marital Status, House Ownership, Car Ownership</span>: No significant difference in risk distribution.</li>
        </ul>
        <h4>Risk Flag vs House Ownership Analysis</h4>
        <p>The bar plot shows the count of <span class="highlight">risk_flag</span> for different <span class="highlight">house_ownership</span> categories:</p>
        <ul>
            <li>Most individuals rent their homes.</li>
            <li>Higher risk (1) is more common among renters compared to owners.</li>
            <li>Very few individuals fall into the "norent_noown" category.</li>
        </ul>
        <h4>Risk Flag vs Car Ownership Analysis</h4>
        <p>The bar plot shows the count of <span class="highlight">risk_flag</span> for different <span class="highlight">car_ownership</span> categories:</p>
        <ul>
            <li>Most individuals do not own a car.</li>
            <li>Higher risk (1) is more common among non-car owners compared to car owners.</li>
            <li>The count of non-risk (0) individuals is higher in both categories.</li>
        </ul>
        <h4>Risk Flag vs Marital Status Analysis</h4>
        <p>The bar plot shows the count of <span class="highlight">risk_flag</span> for different <span class="highlight">marital_status</span> categories:</p>
        <ul>
            <li>Most individuals are single.</li>
            <li>Higher risk (1) is more common among single individuals compared to married ones.</li>
            <li>The count of non-risk (0) individuals is higher in both categories.</li>
        </ul>
