# Quora-Kaggle-Competition
2018 Submission for the Quora Kaggle Competition
# Quora Exploratory Data Analysis
Brittany Bennett  
11/20/2018  

## Competition Description  
An existential problem for any major website today is how to handle toxic and divisive content. Quora wants to tackle this problem head-on to keep their platform a place where users can feel safe sharing their knowledge with the world.  

Quora is a platform that empowers people to learn from each other. On Quora, people can ask questions and connect with others who contribute unique insights and quality answers. A key challenge is to weed out insincere questions -- those founded upon false premises, or that intend to make a statement rather than look for helpful answers.  

In this competition, Kagglers will develop models that identify and flag insincere questions. To date, Quora has employed both machine learning and manual review to address this problem. With your help, they can develop more scalable methods to detect toxic and misleading content.  

Here's your chance to combat online trolls at scale. Help Quora uphold their policy of “Be Nice, Be Respectful” and continue to be a place for sharing and growing the world’s knowledge.  

## Data Description  
In this competition you will be predicting whether a question asked on Quora is sincere or not.  

An insincere question is defined as a question intended to make a statement rather than look for helpful answers. Some characteristics that can signify that a question is insincere:  

Has a non-neutral tone  
-  Has an exaggerated tone to underscore a point about a group of people  
-  Is rhetorical and meant to imply a statement about a group of people  
-  Is disparaging or inflammatory  
Suggests a discriminatory idea against a protected class of people, or seeks confirmation of a stereotype
-  Makes disparaging attacks/insults against a specific person or group of people  
-  Based on an outlandish premise about a group of people  
-  Disparages against a characteristic that is not fixable and not measurable  
Isn't grounded in reality
-  Based on false information, or contains absurd assumptions  
-  Uses sexual content (incest, bestiality, pedophilia) for shock value, and not to seek genuine answers  

The training data includes the question that was asked, and whether it was identified as insincere (target = 1). The ground-truth labels contain some amount of noise: they are not guaranteed to be perfect.  

Note that the distribution of questions in the dataset should not be taken to be representative of the distribution of questions asked on Quora. This is, in part, because of the combination of sampling procedures and sanitization measures that have been applied to the final dataset.  

**File descriptions**
-  train.csv - the training set
-  test.csv - the test set
-  sample_submission.csv - A sample submission in the correct format

### enbeddings/ - (see below)
Data fields  
qid - unique question identifier  
question_text - Quora question text  
target - a question labeled "insincere" has a value of 1, otherwise 0  
This is a Kernels-only competition. The files in this Data section are downloadable for reference in Stage 1. Stage 2 files will only be available in Kernels and not available for download.  

What will be available in the 2nd stage of the competition?  
In the second stage of the competition, we will re-run your selected Kernels. The following files will be swapped with new data:  

test.csv - This will be swapped with the complete public and private test dataset. This file will have ~56k rows in stage 1 and ~376k rows in stage 2. The public leaderboard data remains the same for both versions. The file name will be the same (both test.csv) to ensure that your code will run.
sample_submission.csv - similar to test.csv, this will be changed from ~56k in stage 1 to ~376k rows in stage 2 . The file name will remain the same.
