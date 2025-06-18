# Credit Churn Analysis Project

Credit Churn Analysis Project is an initial data analysis project designed to utilise data exploration, analysis, and visualisation in order to understand churn drivers, dimensional trends and key areas of challenge and opportunity in order to enhance future retention.

# ![CI logo](https://codeinstitute.s3.amazonaws.com/fullstack/ci_logo_small.png)


## Dataset Content
* The dataset used for this project comprises of a credit card churn dataset comprising of a single CSV file taken from Kaggle which contained historical churn data for a major credit provider. 

* Our dataset consisted of 10,127 customers and contains information on their age, gender, salary, dependent count, education level, marital_status, income category, credit card limit, credit card category, etc. 

* See link to the original dataset provided by S Goyal at Kaggle: https://www.google.com/url?q=https://www.kaggle.com/datasets/sakshigoyal7/credit-card-customers/data&sa=D&source=editors&ust=1749552955472088&usg=AOvVaw1o2y1XTJcNfrRwjw66KjOU

## Business Requirements

* Key business requirements include the requirement to identify churn drivers, dimensional trends and key areas of challenge and opportunity in order to enhance future retention.

## Hypothesis and how to validate?

* We predict that younger customers will exhibit higher levels of churn and greater credit utilisation, reflecting more fluid financial behaviour. Additionally, we aim to explore potential correlations between educational levels, professional backgrounds, marital status and customer loyalty. These hypotheses will be tested and illustrated using data visualisations, which will be showcased via both an interactive dashboard and a public presentation.

## Project Plan

* Project ideation is that the sales data can be effectively cleaned and analysed in order to identify key trends and useful data to enhance profitability & retention. The project involves validating our hypothesis through data analysis techniques with results to be presented using data visualisations via an interactive dashboard.

* The data was cleaned before analysis in order to identify any missing or incomplete data lines.

* Outline of the high-level steps taken for the analysis: clean data for processing, analyse and present findings for users.

* Ideology- why did we choose the research methodologies we used? We wanted to obtain an initial understanding of how to extract information from data using basic charts and tools.

* Further work including the use of more complex predictive methodologies and strategies to reduce churn could be carried out on the dataset once patterns have been identified and these could be explored further at a later date.

## The rationale to map the business requirements to the Data Visualisations

* Identify churn trends, and investigate the theory that younger, less established clients  more likely to attrit, investigate any correlation between income/educational background and churn, and investigate whether long-term clients less likely to attrit.
* Identify business insights to enhance profitability, investigate validity of our initial hypotheses and allow predictions to be made for future business activity.
* These hypotheses will be investigated through the use of numerical data insights as well as data visualisations to be presented within an interactive dashboard.

## ETL Process for Credit Card Data Analysis

* To ensure the dataset was clean, structured, and suitable for analysis in **Power BI**, we followed a comprehensive **ETL (Extract, Transform, Load) process**. Initially, we **extracted** raw credit card data, identifying and handling inconsistencies such as missing values, incorrect data types, and anomalies. In the **transformation phase**, numerical columns were processed—scaling values where necessary, filling or removing null entries, and ensuring consistency across fields. Outlier correction: The initial **IQR-based filtering** was too strict, reducing the dataset from 10,172 customers to 8,000. To resolve this, we adjusted the IQR threshold from 1.5 to 3.0, ensuring more valid customer records were retained while still filtering extreme values. This has now resulted in 9390 customers. **Attrition flag recoding**: As there was -1 showing in all columns from the original data clean I recoded again the binary classification (0 for attrited, 1 for retained) was adjusted to exclusively use -1 for missing values, ensuring no valid data was removed during processing. **Numerical column transformations**: We applied scaling, null value handling, and consistency checks across key fields, such as credit limits, transaction amounts, and utilization ratios. After completing data transformations:
The cleaned dataset was saved as cleaned_credit_card_data_v2.csv, ensuring all improvements were preserved. It was loaded into **Power BI** for advanced visualization, filtering, and predictive analytics. This revised dataset ensures optimal performance, enabling reliable insights into customer retention and financial behaviours while m- Numerical column transformations: We applied scaling, null value handling, and consistency checks across key fields, such as credit limits, transaction amounts, and utilization ratios.

* Data analysis methods used include numerical data extraction and dashboards incorporating the use of interactive doughnut and scatter/bar charts.

* Any Future improvements? It would have provided a greater level of insight to display a further level of drill down into the data.

* Did the data limit us? The data had to be intensively cleaned before use to deal with missing values, outliers and other issues (these are fully detailed in the ETL section).

* How was AI used in the project? We used generative AI tools to help with ideation, design thinking and code optimisation.

## Ethical considerations

* We took steps to address data privacy, bias or fairness issues with the data.

* Anonymized information about the customers, recording 21 non-identifying features was used.

* The provenance of the data was considered and informed consent/compliance with GDPR was assumed.

* Bias/fairness issues were not considered as no sensitive data was used.

## Dashboard Design 

* KPIs: Total, existing, and churned customers

Charts:

- Churn by age & gender

- Churn by education

- Churn by marital status

- Churn by income

Widgets: Filters for demographics and financial metrics

* Insights on the dashboard were communicated using a clear, visual approach: KPI cards gave an instant overview for non-technical viewers, while interactive breakdowns by age, gender, education, and income allowed technical users to filter and explore patterns in depth. 

Consistent chart types, filters, and labels ensured everyone could interpret the trends with ease. 📊✨

* Our dashboard was designed to communicate complex data insights to different audiences. Clear visuals and interactive filters helped technical users explore patterns, while simple layouts and highlight cards made the dashboard easy for non-technical stakeholders to interpret.

## Development Roadmap

* What challenges did you face, and what strategies were used to overcome these challenges? One challenge we faced during the hackathon was staying in sync across branches and resolving merge conflicts when working simultaneously in VS Code and GitHub, especially as we navigated multiple feature updates in a tight timeframe.
  
* After the hackathon we plan to learn how to use Streamlit to build on the data skills and design thinking we developed during this project, transforming our insights into interactive and accessible applications.

## Conclusions derived from data analysis element:

* High-income customers are less likely to churn, earners > $40k more likely (except >$120k).

* Younger customers have a lower churn risk - high school students least likely 

* Churn by Educational background - 17.9% doctorate, 15% postgrad, 12-13% others

* Proven correlation between marital status & churn risk - married customers less likely to churn in favour of stability.

* Recommendations: Credit provider should target those customers belonging to a high churn segment with targeted retention offers - sub-dividing by age bracket, salary level & other factors as desired.

* Prioritising extra perks that target groups that are more likely to churn, and  targeting those groups that are more likely to churn through ads

* Strengthening of Emotional Ties with Married Customers - since married customers are less likely to churn, look at lean into stability. Lifecycle perks such as mortgage advice and joint account perks.

* Younger or student customers are showing higher retention, so banks could:

- Introduce early-stage financial wellness programs

- Gamify saving or credit-building features through mobile apps

- Start referral perks — young people appreciate a good deal and will happily share on social media

## Main Data Analysis Libraries

* Python, Panda, Numpy, Matplotlib, Seaborn. Please refer to documentation for insights on use and success.

## Credits 

* Code Institute provided repository templates, README template, content, media and extra help with queries along the way.

* W3 coding provided further information and tutorials on designing dashboards and colour palettes.

* Article by Oscar Baruffa on data storytelling was referred to as a reminder of storytelling principles: https://oscarbaruffa.com/storytelling/ 

### Content 

* Template for README has been provided to me to use as a student of Code Institute.
  
* Instructions on how to implement data analysis techniques were provided to us to use as students of Code Institute.

### Media

* The Code Institute logo has been used with permission as a Code Institute student.

## GitHub Project Link:

* Please refer to our GitHub dashboard to explore our project further: https://app.powerbi.com/groups/me/reports/045c75e4-e86e-4e1a-976a-59a4c2fd2837/e61c947319c6afad5376?ctid=c233c072-135b-431d-af59-35e05babf941&experience=power-bi&bookmarkGuid=b2828574-c792-446f-ad27-2cd1625fe0d6 

## Team Members

This project was developed by our hackathon team:

- Beth Knights [GitHub - bethknights] https://www.linkedin.com/in/beth-anne-knights 

- Gregory Emokpae [GitHub - Greggpeter234] https://www.linkedin.com/in/gregory-emokpae 

- Shema Rahman [GitHub - Shema774] https://www.linkedin.com/in/shemarahman 

## Acknowledgements 

We would like to thank the people who provided support through this project:

* Emma Lamont for support and tutorials.
  
* Mark Briscoe, Niel McEwen & John Rearden for tutorials and insights into effective data visualisation.
  
* Everyone at Code Institute for providing the training opportunity and for all of the guidance along the way.
