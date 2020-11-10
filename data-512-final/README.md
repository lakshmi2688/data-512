
<h1>Analysis of COVID impact on US households</h1>

Lakshmi Venkatasubramanian 
University of Washington  
11/10/2020

<h3> Abstract </h3> 

<p>The goal of this project is to understand the overall impact of COVID on people’s behavior, mental health, housing and livelihoods. There is a large amount of emotionally negative stimuli related to the COVID-19 pandemic. How do people prepare themselves in difficult times like this? Understanding the impact on people is important in order to mitigate the effects and be more prepared in the future. Analyzing and exploring people's response to pandemic can provide useful insights into people's perspective about COVID and the challenges they face.</p>


## Repository structure
```
├── A4-Final-project-proposal.md
├── A5-Final-project-plan.md
├── LICENSE
├── README.md
├── Analysis of COVID impact on US households

<h3>Data sources</h3>
<p>The <a href='https://www2.census.gov/programs-surveys/demo/technical-documentation/hhp/2020_HPS_Background.pdf'>Household Pulse Survey</a> provides timely data to help understand the experiences of American households during the coronavirus pandemic. The data provides insights on education, employment, food security, health, housing, social security benefits, household spending, and transportation. Data Collection has been done in 2 phases.</p>
<ul><li>The first phase of the Household Pulse Survey began on April 23 and ended on July 21, 2020.</li>
<li>The second phase of the Household Pulse Survey began on August 19, 2020 and ended on October 26, 2020 </li></ul></p>

<h4> Links to Data set and Data dictionary</h4>
<p>The datasets are available for public use under <a href='https://www.census.gov/programs-surveys/household-pulse-survey/datasets.html'>census.gov</a> website as weekly files. 

<p>Data dictionary is available in the census.gov website under the following links</p>
<p><li><a href='https://www.census.gov/programs-surveys/household-pulse-survey/technical-documentation.html#phase1'>Phase 1 Household Pulse Survey Technical Documentation</a></li>
<li><a href='https://www.census.gov/programs-surveys/household-pulse-survey/technical-documentation.html#phasePhase2'>Phase 2 Household Pulse Survey Technical Documentation</a></p></li>

<p>The datasets are very rich and informative. Data is collected through survey and interviews. The dataset has been edited or imputed to fill in missing values in order to mitigate the non-response bias.</p>
    <li><strong>Phase 1</strong> dataset has 105 variables, 1088314 observations and includes employment status, food security, housing, physical and mental health, access to health care, and educational disruption. </li>
     <li><strong>Phase 2</strong> dataset has 188 variables, 413976 observations and includes responses from people on how their domains are changing as the pandemic continues and, application and receipt of benefits, spending patterns, and availability of financial resources, post-secondary education disruptions, capacity to telework, and travel practices. </li>
   <p>In order to support the nation’s recovery, we need to know the ways this pandemic has affected people’s lives and livelihoods. Data from these datasets will show the widespread effects of the coronavirus pandemic on individuals, families, and communities across the country.</p>

<h4>Terms of use of census data </h4>
<p>The Census Bureau is committed to open government by sharing its public data as open data. Census data continues to be a key national resource, serving as a fuel for entrepreneurship and innovation, scientific discovery, and commercial activity.  We continuously identify and publish datasets and Application Programming Interface’s (API’s) to Data.gov in accordance with the Office of Management and Budget (OMB) Memorandum M-10-06, the Executive Order 13642 on open data, and the overall principles outlined in the Digital Government Strategy.  In accordance with the Open Data Policy, M-13-13, the Census Bureau publishes its information in machine-readable formats while also safeguarding privacy and security.</p>


<h3>Research Questions</h3>
<ul>
    <li>Understand the impacts of COVID in terms of Employment loss, income loss, Food insufficiency, Education interuptions, inability to meet housing expenses and how does this vary by Race/Ethnicity or gender? Are minority groups and women affected the most?</li>
    <li>What is the impact on Mental health status (Anxiety and depression) by Age, Household income and race? Is there a correlation between Mental health status (Anxiety and depression) and factors such as age, number of household members, gender, income, health status, race? </li>
    <li>How do these characteristics vary in Washington state? </li>
    <li>How do different groups based on age, race and ethnicity differ in their behavior or attitude towards COVID. Are there any patterns observed in the population based on certain characteristics pertaining to COVID?</li> 
</ul>

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



