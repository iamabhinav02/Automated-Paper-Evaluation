# Automated-Paper-Evaluation

In this modern age, where the world moves towards automation so, there is a need for automation in answer evaluation system. Currently, the online answer evaluation is available for mcq based question, hence evaluation of the theory answer is hectic for the checker. Teacher manually checks the answer and allot the marks. The current system takes more manpower and time to evaluate the answer. Since in manual answer evaluation, the manpower and the time consumption is much more. Also, in the manual system, it may be possible that the marks given to two same answers are different. This application system provides an automatic evaluation of answer based on the syntax, semantics, cosine similarity of the answer. 

We will be working on Word2Vec and LSTM model for achieving accuracy. We also worked on some simple Linear, Logistic, SVM, Naive Bayes Classifier models. Major thanks goes to NLTK library for the text pre-processing. 

## We achieved a Cohen's Kappa score of 0.9491 on this dataset which is among one of the highest scores on this dataset.

# About the Data

Dataset is taken from The Hewlett Fundation: Automated Essay Scoring.
The training data is provided in three formats: a tab-separated value (TSV) file, a Microsoft Excel 2010 spreadsheet, and a Microsoft Excel 2003 spreadsheet. 

essay_id: A unique identifier for each individual student essay
essay_set: 1-8, an id for each set of essays
essay: The ascii text of a student's response
rater1_domain1: Rater 1's domain 1 score; all essays have this
rater2_domain1: Rater 2's domain 1 score; all essays have this
rater3_domain1: Rater 3's domain 1 score; only some essays in set 8 have this.
domain1_score: Resolved score between the raters; all essays have this
rater1_domain2: Rater 1's domain 2 score; only essays in set 2 have this
rater2_domain2: Rater 2's domain 2 score; only essays in set 2 have this
domain2_score: Resolved score between the raters; only essays in set 2 have this
rater1_trait1 score - rater3_trait6 score: trait scores for sets 7-8

The validation and test files each have 6 columns:
 
essay_id: A unique identifier for each individual student essay.
essay_set: 1-8, an id for each set of essays.
essay: The ascii text of a student's response.
domain1_predictionid: A unique prediction_id that corresponds to the predicted_score on the essay for domain 1; all essays have this.
domain2_predictionid: A unique prediction_id that corresponds to the predicted_score on the essay for domain 2; only essays in set 2 have this.
