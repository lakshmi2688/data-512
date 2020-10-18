<h1><strong>Bias in data</strong></h1>

<h2><strong> Goal of this project </strong></h2>
<p>The goal of this assignment is to identify what, if any, sources of bias may exist in these datasets, and to develop testable hypotheses about how these biases might impact the behavior of machine learning models trained on the data, when those models are used for research purposes or to power data-driven applications. The purpose of this assignment is to perform a self-directed exploratory data analysis and think critically about the implications of the findings.</p>

<h2><strong>License of the source data </strong></h2>
<p><p>All data we have collected and generated for the <a href='https://meta.wikimedia.org/wiki/Research:Detox'>Wikipedia Detox</a> project is available under free licenses on the <a href ='https://figshare.com/projects/Wikipedia_Talk/16731'>Wikipedia Talk Corpus on Figshare</a>, per the <a href='https://foundation.wikimedia.org/wiki/Open_access_policy'>open access policy</a>. </p>

<h2><strong>Links to all relevant API documentation:</strong></h2>
<p>The corpus we use for the detox project is called the Wikipedia Talk corpus, and it consists of three datasets. Each dataset contains thousands of online discussion posts made by Wikipedia editors who discuss how to write and edit Wikipedia articles. Crowdworkers labelled these posts for three kinds of hostile speech: “toxicity”, “aggression”, and “personal attacks”. Many posts in each dataset were labelled by multiple crowdworkers for each type of hostile speech, to improve accuracy.</p>

<p>Google data scientists used these <a href='https://figshare.com/projects/Wikipedia_Talk/16731'>annotated datasets</a> to train machine learning models as part of a project called <a href='https://conversationai.github.io/'>Conversation AI</a>. The models have been used in a variety of software products and made freely accessible to anyone through the Perspective API. </p>

<p>There are currently two distinct types of data included:</p>
   <ol><li> A corpus of all 95 million user and article talk diffs made between 2001–2015 which can be scored by our personal attacks model.</li>
   <li> An annotated dataset of 1m crowd-sourced annotations that cover 100k talk page diffs (with 10 judgements per diff) for personal attacks, aggression, and toxicity.</li></ol>
<h4>These datasets can be downloaded from the below links</h4>
<ul><li>https://figshare.com/articles/dataset/Wikipedia_Talk_Labels_Aggression/4267550</li>
<li>https://figshare.com/articles/dataset/Wikipedia_Talk_Labels_Toxicity/4563973</li>
<li>https://figshare.com/articles/dataset/Wikipedia_Talk_Labels_Personal_Attacks/4054689</li>
<li>https://figshare.com/articles/dataset/Wikipedia_Talk_Corpus/4264973</li></ul>

| Columns        | Description    |
| :------------- | :----------  | 
|  worker_id | Anonymized crowd-worker id.  | 
| gender   | The gender of the crowd-worker. Takes a value in {'male', 'female', and 'other'}. | 
|  english_first_language | Does the crowd-worker describe English as their first language. Takes a value in {0, 1}. | 
| age_group   | The age group of the crowd-worker. Takes on values in {'Under 18', '18-30', '30-45', '45-60', 'Over 60'}. | 
| education | The highest education level obtained by the crowd-worker. Takes on values in {'none', 'some', 'hs', 'bachelors', 'masters', 'doctorate', 'professional'}. Here 'none' means no schooling, some means 'some schooling', 'hs' means high school completion, and the remaining terms indicate completion of the corresponding degree type. | 


<strong> Lets understand the different columns in the comments dataset</strong>

<ul><li><strong>rev_id: </strong> MediaWiki revision id of the edit that added the comment to a talk page (i.e. discussion).</li>
<li><strong>comment: </strong> Comment text. Consists of the concatenation of content added during a revision/edit of a talk page. MediaWiki markup and HTML have been stripped out. To simplify tsv parsing, \n has been mapped to NEWLINE_TOKEN, \t has been mapped to TAB_TOKEN and " has been mapped to ".</li>
<li><strong>year: </strong> The year the comment was posted in.</li>
<li><strong>logged_in: </strong> Indicator for whether the user who made the comment was logged in. Takes on values in {0, 1}.</li>
<li><strong>ns: </strong>Namespace of the discussion page the comment was made in. Takes on values in {user, article}.</li>
<li><strong>sample: </strong> Indicates whether the comment came via random sampling of all comments, or whether it came from random sampling of the 5 comments around a block event for violating WP:npa or WP:HA. Takes on values in {random, blocked}.</li>
<li><strong>split: </strong> For model building in our paper we split comments into train, dev and test sets. Takes on values in {train, dev, test}.</li></ul>

| Columns        | Description    |
| :------------- | :----------  | 
|  rev_id |  MediaWiki revision id of the edit that added the comment to a talk page (i.e. discussion).  | 
| comment   | Comment text. Consists of the concatenation of content added during a revision/edit of a talk page. MediaWiki markup and HTML have been stripped out. To simplify tsv parsing, \n has been mapped to NEWLINE_TOKEN, \t has been mapped to TAB_TOKEN and " has been mapped to ". | 
|  year | The year the comment was posted in | 
| logged_in   | Indicator for whether the user who made the comment was logged in. Takes on values in {0, 1} | 
| ns | Namespace of the discussion page the comment was made in. Takes on values in {user, article}. | 
|  sample | Indicates whether the comment came via random sampling of all comments, or whether it came from random sampling of the 5 comments around a block event for violating WP:npa or WP:HA. Takes on values in {random, blocked}. | 
| split   | For model building in our paper we split comments into train, dev and test sets. Takes on values in {train, dev, test}.| 

<h2><strong>Known issues/considerations</strong></h2>
<p>Data from the Pageview API excludes spiders/crawlers, while data from the Pagecounts API does not</p>

