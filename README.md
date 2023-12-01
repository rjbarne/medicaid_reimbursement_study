# dmda-capstone
Capstone project for BS DMDA program utilizing a variety of skills acquired during the program.

# Determining Unfairness in Medicaid Reimbursement Rates
# Between Idaho and the Nation
By Robert Barnett

# A. Project Overview
## A1. Research Questions
Is there a significant difference in Medicaid reimbursement rates between Idaho and the nation?
## A2. Context & Background
Healthcare organizations share a common view that Medicaid often pays below costs. While Medicaid is overseen by the Centers for Medicare and Medicaid Services (CMS) on a federal level, much of a Medicaid program’s operation is left to the authority of each state, including pricing methodologies. Medicaid programs subscribe to a national database, such as Medispan or First Databank, for a standardized drug information catalog. However, due to each state’s ability to manage their own Medicaid programs, each program’s pricing methodologies can give rise to different reimbursement rates. Some programs attempt to augment the burden by obtaining kickbacks from manufacturers, incentivizing providers to adhere to therapy regimens, and other tactics. Some tactics are executed successfully while others create gaps in coverage and reimbursements. Atypical reimbursement rates would be a useful indicator to justify an investigation into suboptimal tactics employed by a Medicaid program’s pricing methodologies. Consistently low reimbursement rates can adversely affect a healthcare organization’s viability to provide care to Medicaid beneficiaries. 
## A3. Summary of Published Works
In Medicaid Reimbursement Rates Are a Racial Justice Issue, Ford, T., & Michener, J. (2022), Medicaid has a reputation for underpaying healthcare providers for covered services. In a blog article from The Commonwealth Fund titled "Medicaid Reimbursement Rates Are a Racial Justice Issue", the authors discuss how reimbursement rates affect access and quality of care for underprivileged groups. They highlight that Medicaid reimbursement rates are significantly lower than Medicare and commercial insurance rates which creates a financial disincentive for providers to accept Medicaid patients which affects availability and quality of care. It draws many connections between Medicaid's low reimbursement rates and low quality of care. This source of information paints a broader picture of the impact of low reimbursement rates in communities.
A lawsuit was filed in Washington (National Association of Chain Drug Stores v. Xavier Becerra, 2021) by the National Association of Chain Drug Stores (NACDS), National Community Pharmacists Association (NCPA), and the Washington State Pharmacy Association versus the Secretary of the United States Department of Health and Human Services (HHS) and the Centers for Medicare and Medicaid Services (CMS). The plaintiffs claim that Medicaid does not adequately reimburse pharmacies for the services they provide to beneficiaries and that their reimbursement rates are the lowest in the country, which violates federal law. They allege that the rates are below their actual costs which has caused significant harm to rural and independent pharmacies. The lawsuit particularly focuses on the dispensing fee component of reimbursement rates. Dispensing fees are intended to cover costs associated with dispensing a medication, such as payroll, utilities, rent, supplies, etc. This source illustrates the impact of low reimbursement rates and the resulting action that can be taken against Medicaid to correct it.
Medicaid underpayment has been a long concern in the legislative landscape as well. As reported in 2009 by Kaiser Health News (Pharmacy Groups Lobby for Revisions to Proposed Medicaid Rule, 2009), CMS proposed a rule in 2006 to implement provisions of the Deficit Reduction Act that would reduce Medicaid reimbursements for prescriptions. The rule would redefine the cost basis for reimbursements. HHS forecasted that the change would adversely affect revenue for small pharmacies in low-income areas where the concentration of Medicaid beneficiaries was high. HHS advised that small pharmacies purchase lower-cost drugs to mitigate the burden. However, that was already a best practice among all pharmacies. HHS also released a report finding that 19 of the 25 highest-expenditure drugs would result in underpayments under the new rule. Pharmacy groups attempted to work with lawmakers to draft revisions to change the cost-basis to a metric that was tangible for pharmacies, but the CMS administrator dismissed concerns in favor of waiting to see how things turned out. This source of information illustrates legislative challenges that propagate the issues that give rise to low reimbursement rates.
## A4. Summary of Data Analytics Solution
This project will seek to evaluate if a statistically significant difference exists between Idaho and the nation in Medicaid reimbursements. Two datasets will be explored which are both obtained from Medicaid. One dataset will contain the reimbursement data and the other dataset will be used to expand drug information in the main dataset. The data will be cleaned and then formed into useful dataframes. Histograms will be viewed to observe distributions of reimbursement rates. The reimbursement rates will be evaluated on a Z-score for each state and then compared against Idaho's Z-score. A Z-test will be used to evaluate a null hypothesis with a Z-critical of 1.96. 
## A5. Benefits & Support of Decision-Making Process
The solution of this analysis can be beneficial in many ways.
-	Pharmacies can use this information to identify which drugs are underpaid and apply it to their inventory management.
-	Organizations can use this information to take legal action against their state’s Medicaid program if any laws or rules are broken. 
-	A pharmacy may be able to identify opportunities for improving billing best practices by comparing this data against their dispensing data.
The benefits can directly assist in decision-making by creating access to a list of low-revenue drugs and searching for NDCs with better reimbursements. 
An example could be that a pharmacy identifies some of their dispensings of a specific NDC that was underpaid yet did not show as underpaid in the analysis. This would indicate that they most likely billed the item incorrectly, creating a systematic training opportunity.
# B. Data Analytics Project Plan
## B1. Goals, Objectives, & Deliverables
The goal of this project is to evaluate if a significant difference exists between Idaho and the nation with Medicaid reimbursements. 
The following objectives will meet this goal:
-	Acquire the datasets. Download the datasets from Medicaid.gov and load them into a Jupyter Notebook.
o	Deliverable: Raw datasets downloaded into local files.
-	Clean the datasets. Review and prepare the datasets for exploration within the Jupyter Notebook.
o	Deliverable: Loaded and cleaned data.
-	Explore the datasets. Transform the data into information and perform statistical calculations.
o	Deliverable: Explored data.
-	Compare the z-scores of reimbursements among the states. Evaluate the calculated statistics to evaluate the hypothesis.
o	Deliverable: Analyzed data with statistical significance calculated.
-	Finalize a report of the findings. Report conclusions based on the insights found in the exploration of the dataset.
o	Deliverable: Written report of conclusions.
## B2. Scope of the Project
The scope of the project will include analysis and visualizations using Python in a Jupyter Notebook with two CSV datasets as input. The input will be used to calculate statistical significance using a Z-score test for the state of Idaho. The datasets are aggregated from sources in 2022 and will compare 1st quarter data. This project will not find a statistical significance for other states or other years as that falls outside the scope. 
Specifically, this project will include an evaluation of the dataset filtered to explore the reimbursement rates of countable drugs within the 1st quarter of 2022 for the state of Idaho and the nation, subset by branded and generic drugs to find a statistical significance. This project will not explore any statistical significance for other states or any other subsets of drugs.
## B3. Project Planning Methodology
This project will use the CRISP-DM (Cross-Industry Standard Process for Data Mining) methodology. It’s useful for analytics projects and the following phases will be utilized:
-	Business understanding: Define the objectives, scope, and criteria for success concerning the business needs. In this step, I identified the need to address underpayments.
-	Data understanding: Collect, explore, and clean the data while selecting relevant features for the analysis. I found datasets available from a payor with features that would be appropriate for analysis.
-	Data preparation: Transform, clean, and integrate the data. This step will be performed within a Jupyter Notebook using Python and various libraries.
-	Evaluation: This step will evaluate the analysis for statistical significance with a Z-score test
-	Deployment: This step will ensure that the functions can be useful on similar datasets provided by Medicaid to evaluate other years.
## B4. Timeline for Milestones
Milestone	Duration	Start	End
Acquire Data	1 day	11/23	11/24
Clean Data	1 day	11/24	11/25
Explore Data	1 day	11/25	11/26
Analyze Data	2 days	11/26	11/27
Finalize Report	1 day	11/27	11/28

## B5. Resources and Associated Costs
1.	PC: $1000
2.	Python 3: $0
3.	Anaconda: $0
4.	Datasets: $0
5.	40 work hours: $2000 @ $50 per hour
B6. Criteria for Success
The criteria for success will be:
-	A completed Z-score test. The Z-score will be calculated and compared to a Z-critical score of 1.96 based on an α of 0.05. If the absolute value of the Z-score is less than the absolute value of the Z-critical value, then the null hypothesis will be accepted. Otherwise the alternate hypothesis is accepted. 
-	Acceptance or rejection of the null hypothesis based on the calculated Z-score. The acceptance of either the null hypothesis or alternate hypothesis shall be stated clear and concise. 
-	Data visualizations to represent distributions. Successful visualizations will display the data with easily observable inferences.
# C. Design of Data Analytics Solution
## C1. Hypothesis
Null Hypothesis: There is no significant difference in reimbursement rates between Idaho and the nation.
Alternate Hypothesis: There is a significant difference in reimbursement rates between Idaho and the nation.
α = 0.05
Z-Critical = 1.96
## C2. Analytical Method
The Z-score statistical test compares a data point to a population mean. The formula for calculating the z-score is z = (x - μ) / σ where x is the data point, μ is the population mean and σ is the population standard deviation. The data will be cleaned and then used to calculate the reimbursement rate. That reimbursement rate will be grouped by NDC, and a z-score will be calculated. Idaho’s z-score will be compared to the national z-scores for branded and generic drugs. 
The analytical method will be descriptive. The analysis will observe a past dataset to describe what happened to reimbursement rates in Idaho compared to the nation. This type of analytical method is used to transform past data into information that can be acted upon. 
## C3. Tools & Environment
This project will be completed within a Jupyter Notebook running Python 3. It will require the following libraries: pandas, NumPy, MatplotLib, and SciPy. 
Jupyter Notebook is a useful IDE to perform descriptive analytics with Python code, cell by cell. The ability to use markdown language allows an analyst to create a self-contained presentable journey through the analytical process. 
Python 3 is useful because it can utilize many data science-oriented libraries to effectively analyze data. 
The pandas library is critical for loading large datasets and performing essential data manipulation tasks within dataframes. 
The numpy library is useful for arrays. 
The MatplotLib library is useful for creating visualizations in Python, such as the histograms and box plots for this project.
The SciPy library is useful for statistical modules. In this project, it will be used for calculating Z-score for the dataframe.
## C4. Methods & Metrics to Evaluate Statistical Significance
The planned statistical test is a Z-score test. The null hypothesis is that no significant difference in Medicaid reimbursement rates exists between Idaho and the nation. This will produce a Z-score to compare against the population mean. The α of 0.05 is statistically significant for a two-sided Z-test will have a Z-critical of 1.96 to accept or reject the null hypothesis. This is an appropriate statistical test because it will illustrate the amount of underpayment that Idaho experiences relative to the sample population. 
## C5. Practical Significance
The practical significance of this project is that pharmacies will be able to identify items that they may be underpaid for. If there is a systematic underpayment, then it can lead to legislative action. On a granular level, a pharmacy can compare their Medicaid reimbursement data against this project’s data to identify items that do not match and investigate the cause which may be a billing error by the pharmacy. Such billing errors could be a systemic training issue in their organization which may affect their reimbursements from other payors. Larger organizations, like state boards of pharmacy or a pharmacy services administrative organization (PSAO), may look at region-wide data to find legally actionable issues, such as the case in Washington. 
## C6. Visual Communication
Histograms will be useful for observing the distribution of counts reimbursement rates across the nation and to judge appropriateness of applying a Z-score test. The anticipation is that the distribution will resemble a Gaussian distribution. A histogram comparing the distributions of reimbursement rates for generic drugs in each state will be created using matplotlib. A histogram comparing the distributions of reimbursement rates for brand drugs in each state will be created using matplotlib. Histograms of various NDCs will also be created to view the distribution on a granular level. 
Box plots can illustrate measures of central tendency very well. A box plot will be utilized to illustrate the Z-scores across the nation for each brand and generic reimbursement rates. This will illustrate how Idaho compares to the nation on a more granular view. Then another box plot will be created to compare Idaho directly to the population. 
# D. Description of Dataset
## D1. Source of Data
DrugUtilization2022_updated.csv and nadac-national-average-drug-acquisition-cost-2022.csv were both retrieved from data.medicaid.gov and each has a Public Domain Mark 1.0 license.
## D2. Appropriateness of Dataset
The DrugUtilization dataset contains the reimbursement data for all states by NDC. The NADAC dataset has drug information that the DrugUtilization dataset does not have and will be used to expand the drug information based on NDC as a shared key. 
## D3. Data Collection Methods
The DrugUtilization2022_updated.csv file was downloaded from https://data.medicaid.gov/dataset/200c2cba-e58d-4a95-aa60-14b99736808d/data. 
The nadac-national-average-drug-acquisition-cost-2022.csv file was downloaded from https://data.medicaid.gov/dataset/dfa2ab14-06c2-457a-9e36-5cb6d80f8d93. 
## D4. Observations on Quality & Completeness of Data
The datasets are good quality. They are both clean and free of errors. There is some missing data due to states that failed to report on time, but I believe it is not significant enough to affect the exploration. Other than that, the datasets appear complete to a high satisfaction. The datatypes are consistent in each column and the columns properly describe their data. Some data is missing due to states that did not report on time, but they describe areas outside the scope of this project. 
The data will be evaluated for the 1st quarter, so the missing data from later quarters is not a concern. The data will be filtered for the 1st quarter and then NaN rows will be dropped. The NADAC dataset has much more data than is needed for the scope of this project, so most of the unnecessary rows will be dropped to save memory. The duplicate rows of NDC will also be dropped so that it can function as a key for merging into the main dataset. 
## D5. Data Governance, Privacy, Security, Ethical, Legal & Regulatory Compliances
These datasets are available under a Public Domain Mark 1.0 license which has no restrictions on use. These datasets may be copied, modified, distributed, and perform work without asking for permission. There is no personal information within these datasets to create any privacy or security concerns. There are no ethical, legal, or regulatory compliance concerns with these datasets. As such, no precautions are necessary.

# Sources
Ford, T., & Michener, J. (2022, June 16). Medicaid Reimbursement Rates Are a Racial Justice Issue. The Commonwealth Fund. Retrieved from https://www.commonwealthfund.org/blog/2022/medicaid-reimbursement-rates-are-racial-justice-issue 
“Pharmacy Groups Lobby for Revisions to Proposed Medicaid Rule” (2009, June 11). Kaiser Health News. Retrieved from https://kffhealthnews.org/morning-breakout/dr00045610/
National Association of Chain Drug Stores v. Xavier Becerra, 2:21-cv-00576-RSM (W.D. Wash. filed April 29, 2021)
