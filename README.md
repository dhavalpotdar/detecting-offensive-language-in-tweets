# Detecting Offensive Language in Tweets

This project aims to detect offensive language in tweets using ML Classification Algorithms. A training and predicting pipeline is implemented
to contrast performance of various popular classification algorithms and determine the best suited model. 

## Data
Data is taken from two sources:
1.	Hate Speech Twitter Annotations
    - Publication: 
Z. Waseem and D. Hovy. Hateful symbols or hateful people? predictive features for hate speech detection on twitter. In NAACL SRW, pages 88–93, 2016 
    - Authors: Waseem, Zeerak and Hovy, Dirk
    - GitHub Link: https://github.com/zeerakw/hatespeech
    -	Description: 
The dataset contains about 17,000 Tweet ID's labeled for racism and sexism. We downloaded this dataset and querried a Twitter API to scrape the actual tweets from Twitter. Retrieval of about tweets 5,900 failed either because the tweet was deleted or the account was deactivated. 

2.	Hate Speech and Offensive Language Detection
    - Publication: 
Automated Hate Speech Detection and the Problem of Offensive Language
    - Authors: Davidson, Thomas and Warmsley, Dana and Macy, Michael and Weber, Ingmar
    - GitHub Link: https://github.com/t-davidson/hate-speech-and-offensive-language
    - Description:
The dataset has about 25,000 Tweets annotated by crowd sourcing. As per the number of users labeling the Tweets, each is put in one of three classes - hate speech, offensive language and neither. We downloaded the dataset in Python from GitHub as a csv file.<br>
The data from both sources are clubbed. Here is the distribution of the tweets into the two classes:


![Dataset](/distribution_of_tweets.png)

## Code
The code is distributed into two Juypyter Notebooks which can be viewed in rendered format on the links:
- cyberbullying_wrangling.ipynb | [Link](https://nbviewer.jupyter.org/github/dhavalpotdar/cyberbyllying-detection/blob/master/cyberbullying_wrangling.ipynb)
- cyberbullying_v2.ipynb | [Link](https://nbviewer.jupyter.org/github/dhavalpotdar/cyberbyllying-detection/blob/master/cyberbullying_v2.ipynb)

## Summary
![performance](/algo_comparison.png) <br>

![time](/algo_time.png)

After tuning hyper-parameters to optimize the algorithms, Stochastic Gradient Descent was found to be the best suited algorithm, taking both performance and time complexity into account.
Following performance metrics were achievec:
-	Accuracy: 92.81 %
-	Precision: 96.97 %
-	Recall: 91.94 %
-	F1-Score: 94.39 %

## License
The contents of this repository are covered under the [MIT License](https://github.com/dhavalpotdar/cyberbyllying-detection/blob/master/LICENSE).
