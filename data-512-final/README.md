
<h1>Analysis of COVID impact on US households</h1>

Lakshmi Venkatasubramanian 
University of Washington  
11/10/2020

<h3> Abstract </h3> 

<p>The goal of this project is to understand the overall impact of COVID on people’s behavior, mental health, housing and livelihoods. There is a large amount of emotionally negative stimuli related to the COVID-19 pandemic. How do people prepare themselves in difficult times like this? Understanding the impact on people is important in order to mitigate the effects and be more prepared in the future. Analyzing and exploring people's response to pandemic can provide useful insights into people's perspective about COVID and the challenges they face.</p>


## Repository structure
```
├── README.md
├── LICENSE
├── Analysis of COVID impact on US households.ipynb
```

<h3>Data Source</h3>
<p>The <a href='https://www2.census.gov/programs-surveys/demo/technical-documentation/hhp/2020_HPS_Background.pdf'>Household Pulse Survey</a> provides timely data to help understand the experiences of American households during the coronavirus pandemic. </p>

<p>Data Collection has been done in 2 phases.</p>
<ul><li>The first phase of the Household Pulse Survey began on April 23 and ended on July 21, 2020.</li>
<li>The second phase of the Household Pulse Survey began on August 19, 2020 and ended on October 26, 2020 </li></ul></p>

<h4> Links to Data set and Data dictionary</h4>
<p>The datasets are available for public use under <a href='https://www.census.gov/programs-surveys/household-pulse-survey/datasets.html'>census.gov</a> website as weekly files. 

<p>Data dictionary is available in the census.gov website under the following links</p>
<li><a href='https://www.census.gov/programs-surveys/household-pulse-survey/technical-documentation.html#phase1'>Phase 1 Household Pulse Survey Technical Documentation</a></li>
<li><a href='https://www.census.gov/programs-surveys/household-pulse-survey/technical-documentation.html#phasePhase2'>Phase 2 Household Pulse Survey Technical Documentation</a></li>

<p>The datasets are very rich and informative. Data is collected through survey and interviews. The dataset has been edited or imputed to fill in missing values in order to mitigate the non-response bias.</p>
    <li><strong>Phase 1</strong> dataset has 105 variables, 1088314 observations and includes employment status, food security, housing, physical and mental health, access to health care, and educational disruption. </li>
     <li><strong>Phase 2</strong> dataset has 188 variables, 413976 observations and includes responses from people on how their domains are changing as the pandemic continues and, application and receipt of benefits, spending patterns, and availability of financial resources, post-secondary education disruptions, capacity to telework, and travel practices. </li>

<p>The survey was designed to gauge the impact of the pandemic on overall household characteristics such as employment status, consumer spending, food security, housing, education disruptions, and dimensions of physical and mental wellness. It was conducted by an internet questionnaire, with invitations to participate sent by email and text message. Housing units linked to one or more email addresses or cell phone numbers were randomly selected to participate, and one respondent from each housing unit was selected to respond. Below is a sample question from the survey:</p>
<strong>Over the last 7 days, how often have you been bothered by the following problems … Not being able to stop or control worrying? Would you say not at all, several days, more than half the days, or nearly every day? Select only one answer.</strong>

<p>In order to support the nation’s recovery, we need to know the ways this pandemic has affected people’s lives and livelihoods. Data from these datasets will show the widespread effects of the coronavirus pandemic on individuals, families, and communities across the country. <strong>For the purpose of this analysis, only phase 1 datasets are used</strong></p>
   
<h4>Download data</h4>
<p>Data is directly downloaded from census website using zipfile feature of python<p>

<h4>Terms of use of census data </h4>
<p>The Census Bureau is committed to open government by sharing its public data as open data. Census data continues to be a key national resource, serving as a fuel for entrepreneurship and innovation, scientific discovery, and commercial activity.  We continuously identify and publish datasets and Application Programming Interface’s (API’s) to Data.gov in accordance with the Office of Management and Budget (OMB) Memorandum M-10-06, the Executive Order 13642 on open data, and the overall principles outlined in the Digital Government Strategy.  In
 accordance with the Open Data Policy, M-13-13, the Census Bureau publishes its information in machine-readable formats while also safeguarding privacy and security.</p>


<h3>Research Questions</h3>
<ul>
    <li>Understand the impacts of COVID in terms of employment loss, income loss, food insufficiency, education interruptions, inability to meet housing expenses and how does this vary by Race/Ethnicity or gender? Are minority groups and women affected the most?</li>
    <li>What is the impact on Mental health status (Anxiety and depression)? Is there a correlation between Mental health status (Anxiety and depression) and factors such as age, number of household members, gender, income, health status, race? How does the anxiety levels vary between first and last week of survey?</li>
    <li>How does employment loss, income loss, food insufficiency, education interruptions, inability to meet housing expenses in Washington differ as compared  to national average?</li>
    <li>How do different groups based on age, race and ethnicity differ in their behavior or attitude towards COVID. Are there any patterns observed in the population based on certain characteristics pertaining to COVID?</li> 
</ul>

<h3>Background/Related Work</h3>
<p>As we all know,the impacts of the pandemic and the economic fallout have been widespread, but are particularly prevalent among Black, Latino, Indigenous, and immigrant households. Similarly percentage of adults who report symptoms of anxiety or depression that have been shown to be associated with diagnoses of generalized anxiety disorder or major depressive disorder.  These symptoms generally occur more than half the days or nearly every day. The research questions will follow similar quantitative analysis and will target specific variables. Below are some references: </p>
<li><a href='https://www.cbpp.org/research/poverty-and-inequality/tracking-the-covid-19-recessions-effects-on-food-housing-and'>Covid Recession effects</a></li>
<li><a href='https://www.cdc.gov/nchs/covid19/pulse/mental-health.htm'>Covid data from NCHS</a></li>


<h3>Methodology</h3>
<ul>
    <li>For the first 2 research questions, multivariate regression analysis will be used. This will help me to understand any correlation among the variables. </li>
    <li>For question 3, statitical tests such as z-test will be helpful in understanding the difference between WA state and national average </li>
    <li>For the third question, clustering and PCA will help me understand the various patterns in the behavior</li> 
</ul>

<h3>Source of Bias</h3>
<p> Nonsampling errors can also occur and are more likely for surveys that are implemented quickly, achieve low response rates, and rely on online response.  Nonsampling errors for the Household Pulse Survey may include:</p>

<ul><li><strong>Measurement error:</strong> The respondent provides incorrect information, or an unclear survey question is misunderstood by the respondent. The Household Pulse Survey schedule offered only limited time for testing questions. </li>
<li><strong>Coverage error: </strong>Individuals who otherwise would have been included in the survey frame were missed. The Household Pulse Survey only recruited households for which an email address or cell phone number could be identified.</li>
<li><strong>Nonresponse error:</strong> Responses are not collected from all those in the sample or the respondent is unwilling to provide information. The response rate for the Household Pulse Survey was substantially lower than most federally sponsored surveys.</li>
<li><strong>Processing error: </strong>Forms may be lost, data may be incorrectly keyed, coded, or recoded. The real-time dissemination of the Household Pulse Survey provided limited time to identify and fix processing errors.</li>
 
<p>The Census Bureau employs quality control procedures to minimize these errors.  However, the potential bias due to nonsampling errors has not yet been evaluated.</p>
## Resources used

This analysis was prepared using Python 3.8 running in a Jupyter Notebook environment.  
Documentation for Python can be found here: https://docs.python.org/3.8/  
Documentation for Jupyter Notebook can be found here: http://jupyter-notebook.readthedocs.io/en/latest/  

The following Python packages were used and their documentation can be found at the accompanying links:

* [pandas](https://pandas.pydata.org/)
* [numpy](https://numpy.org/)
* [IPython](https://ipython.org/)
* [matplotlib](https://matplotlib.org/)
* [seaborn](https://seaborn.pydata.org/)

<h3>Unknowns and dependencies</h3>
<p>These data are experimental and samples may not be representative of the population. </p>



