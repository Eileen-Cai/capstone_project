# Content Moderation on Social Media Apps

## Table of Contents

[Project Overview](#overview)
- [Introduction](#introduction)
- [Problem Statement](#problem)
- [Our Solution](#solution)
- [Objectives](#objectives)
- [Potential Impact](#impact)

[Dataset](#dataset)  
- [Data Description](#description)
- [Data Dictionary](#dictionary)
- [Data Source](#source)

[Project Roadmap](#roadmap)
- [Exploratory Data Analysis](#eda)
- [Model Development](#develop)
- [Model Interpretation](#interpret)
- [Model Deployment](#deploy)
- [User Interface Development](#uid)

[Conclusion](#conclusion)
- [Insights & Findings](#insight)
- [Key Takeaways](#takeaway)
- [Future Directions](#dir)

## Project Overview <a name="overview"></a>
### Introduction <a name="introduction"></a>
My area of interest is to use machine learning to help identify social media content that are harmful to teens mental health. A challenge faced by many social media companies is the spread of child sexual abuse material online and other harmful content, such as, cyber bullying, drug sales and hate speach. Although there are tools, such as [Take it Down](https://takeitdown.ncmec.org/), that allow parents and minors to get images removed from social media, I want to take a more proactive approach to identify harmful content before it reaches the wrong audience. 
### Problem Statement <a name="problem"></a>
The problem we try to address in this project is to use machine learning to automatically detect harmful texts. The users are teens and parents. Teens benefit from the removal of unhealthy social media, and avoid becoming a victim of online predators and cyberbullying, which can raise the risk of mental health conditions like anxiety, depression, and worst-case self-harm and death. Parents benefirt from having a piece of mind knowing that their kids are been protected online. 
### Our Solution <a name="solution"></a>
To address these issues, our proposed solution is to perform natural language processing (NLP) to encode text data into a numeric matrix then feed the numeric data into a machine learning model for sentiment analysis.
### Objectives <a name="objectives"></a>
Build machine learning models for automatic detection of hate speech and offensive language.
### Potential Impact <a name="impact"></a>
- **Sentiment Analysis**: By classifying tweets as hate speech, offensive language, or neither, the model can help in understanding the sentiment behind different tweets and identifying patterns of negative or offensive language. 
- **Hate Speech Detection**: The model can automatically detect hate speech on Twitter and make it possible to create a system that can identify and flag hate speech in real-time, making social media platforms safer and more inclusive. 
- **Content Moderation**: Social media platforms can use this model to improve their content moderation systems. By using machine learning algorithms trained on this data, it becomes easier to automatically detect and remove offensive or hateful content from the platform, reducing the burden on human moderators and improving user experience by keeping online spaces free from toxic behavior. 
## Dataset <a name="dataset"></a>
### Data Description <a name="description"></a>
This dataset is a meticulously curated collection of annotated tweets with the specific purpose of detecting hate speech and offensive language. The dataset primarily consists of English tweets and is designed to train machine learning models or algorithms in the task of hate speech detection. 

The dataset includes several columns that provide valuable information for understanding each tweet's classification. The column count represents the total number of annotations provided for each tweet, whereas hate_speech_count signifies how many annotations classified a particular tweet as hate speech. On the other hand, offensive_language_count indicates the number of annotations categorizing a tweet as containing offensive language. Additionally, neither_count denotes how many annotations identified a tweet as neither hate speech nor offensive language.
- The dataset is presented in a CSV file format named 'train.csv'.
- It consists of annotated tweets with information about their classification as hate speech, offensive language, or neither.
- Each row represents a tweet along with the corresponding annotations provided by multiple annotators.
- The main columns that will be essential for our analysis are: count(total number of annotations), hate_speech_count(number of annotations classifying a tweet as hate speech), offensive_language_count(number of annotations classifying a tweet as offensive language), neither_count(number of annotations classifying a tweet as neither hate speech nor offensive language).
### Data Dictionary <a name="dictionary"></a>
| Column | Data Type | Description |
|--------|-----------|-------------|
| count  | int | The total number of annotations for each tweet.
| hate_speech_count | int | The number of annotations classifying a tweet as hate speech.
| offensive_language_count | int | The number of annotations classifying a tweet as offensive language.
| neither_count | int | The number of annotations classifying a tweet as neither hate speech nor offensive language.
| class | int | The category in which a tweet belongs to.
| tweet | str | The actual text of the tweet.
### Data Source <a name="source"></a>
The data collection methodology used to create this dataset involved obtaining tweets from Twitter's public API using specific search terms related to hate speech and offensive language. These tweets were then manually labeled by multiple annotators who reviewed them for classification purposes.

Dataset can be found on Huggingface [hate_speech_offensive](https://huggingface.co/datasets/tdavidson/hate_speech_offensive)
## Project Roadmap <a name="roadmap"></a>
### Exploratory Data Analysis <a name="eda"></a>
- Perform text processing to remove stop words and tokenize tweets.
- Perform bag of words vectorization.
- Distribution of tweet counts per classification category (hate speech, offensive language, neither).
- Most common words/phrases associated with each class.
- Co-occurrence analysis to identify correlations between hate speech and offensive language. 

Data quality concerns: Although efforts have been made to ensure the accuracy of the data, it is important to acknowledge that annotations are subjective opinions provided by individual annotators. As such, there may be variations in classifications between annotators.
### Model Development <a name="develop"></a>
- Split the dataset into training and testing sets for model evaluation purposes.
- Perform Logistic Regression and KNN to compare model performances.
### Model Interpretation <a name="interpret"></a>
### Model Deployment <a name="deploy"></a>
### User Interface Development <a name="uid"></a>
## Conclusion <a name="conclusion"></a>
### Insights & Findings <a name="insight"></a>
### Key Takeaways <a name="takeaway"></a>
### Future Directions <a name="dir"></a>
Use machine learning to also recognize harmful images, videos, and memes.