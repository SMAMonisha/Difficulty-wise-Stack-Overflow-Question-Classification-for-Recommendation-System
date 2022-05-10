# Classification of Stack Overflow Questions Based on Difficulty

Stack Overflow post classification based on the difficulty. Our proposed models are implemented and evaluated based on the contextual features of the questions and the users. Each features considered is a part of certain feature sets, e.g. Semantic feature set, Pre-hoc set and Post-hoc set. 

- 	Semantic feature set: Body, LOC, QuestionLength, Url+ImageCount
- 	Pre-hoc feature set: Sementic feature set, Reputation, user_badge_bronze_counts, user_badge_gold_counts, user_badge_silver_counts, accept_rate
- 	Post-hoc set: Pre-hoc feature set, view_count, answer_count, favorite_count, question_score, up_vote_count, First_answer_Interval, Accept_answer_Interval

Each post title and tags are considered part of its respective body. The semantic analyzer models in our proposed methodology are **TF-IDF** vectorizer, **LDA**(Latent Dirichlet Allocation) and **Doc2Vec** model with classifiers of **Random Forest**, **Xgboost**, **Adaboost** and **SVM**(Support Vector Machine). And considered the metrics are Accuracy, Precision, Recall, f1 score and AUC-ROC.