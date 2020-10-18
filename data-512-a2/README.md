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

<h2><strong>Description of fields in the data file en-wikipedia_traffic_200712-202008.csv</strong></h2>
	<table>	
		<thead>	

		</thead>
		<tbody>	
      			<tr>	
				<td>|</td>
				<td>year</td>
				<td>|</td>
				<td>year in the format YYYY</td>
				<td>|</td>		
			</tr>
			<tr>	
				<td>month</td>
				<td>month in the format MM</td>
			</tr>
			<tr>	
				<td>	</td>
				<td>	</td>
				<td>	</td>
			</tr>
		</tbody>
	</table>

</body>


<h2><strong>Known issues/considerations</strong></h2>
<p>Data from the Pageview API excludes spiders/crawlers, while data from the Pagecounts API does not</p>

