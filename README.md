# Capitalizing on changing sentiment and discourse in the Russia-Ukraine war

### Abstract

At the beginning of the Russia-Ukraine war the general consensus on many people's social media feeds seemed to show support for the country of Ukraine and its refugees. However, as the conflict continued with no clear end in sight, interest seemed to wane. How did specific events and acts of aggression affect people's feelings about the war? 

My client, a non-profit organization hoping to raise money to support Ukranian refugees, is interested in learning how current events and developments in the war might impact interest in charitable giving.

I looked at social media tweets to determine how significant events resulted in changes in sentiment and how people talked about the war.

### Design

Using a [dataset from Kaggle] (https://www.kaggle.com/datasets/bwandowando/ukraine-russian-crisis-twitter-dataset-1-2-m-rows
) consisting of tweets related to the Ukraine-Russian conflict, I selected English language tweets from dates corresponding to significant events as follows:
	- March 01, 2022 - Russia completely surrounds Mariupol
	- March 13, 2022 - Russia attacks military base; 35 people killed, 130 hospitalized
	- March 15, 2022 - Russia besieges Mariupol hospital; hundreds held hostage
	- March 16, 2022 - Russia bombs Mariupol Theater being used as shelter; hundreds killed
	- April 03, 2022 - Russia withdraws from Bucha, leaving evidence of atrocities
	- April 08, 2022 - Russia strikes Kramatorsk railway station

### Data

At the time of analysis, the dataset from Kaggle consisted of 26 million tweets containing certain hashtags related to the Russia-Ukraine conflict that were collected from the end of February 2022 through April 2022. For the purposes of this project I randomly sub-sampled 100K tweets from the corpus for select significant days (totaling 600K tweets).


### Algorithms
 
I used VADER to evaluate each document (tweet), which gave four scores indicating the likely sentiment of each document: negative, neutral, positive, and compound. For the purposes of this project, I chose to utilize the compound score as it accounted for more variance or nuance in tweets.

### Tools

I used Pandas and NLTK to pre-process and clean the documents, which were then analyzed using VADER and CountVectorizer. Matplotlib and Scattertext were used to help visualize some of the differences in the corpora across dates.


### Communication

See slides for presentation