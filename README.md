# mn-ds-news-classification
Notebook for the technical validation of MN-DS: A Multilabeled News Dataset for News Articles Hierarchical Classification

### Dataset.

MN-DS is a dataset of 10,917 news articles with hierarchical news categories collected between January 1st 2019, and December 31st 2019. We manually labelled the articles based on a hierarchical taxonomy with 17 first-level and 109 second-level categories. This dataset can be used to train machine learning models for automatically classifying news articles by topic. This dataset can be helpful for researchers working on news structuring, classification, and predicting future events based on released news.

Repository contains:
- [pipelineFull](https://github.com/alinapetukhova/mn-ds-news-classification/pipelineFull.ipynb): Jupyter notebook with the code for models tranining
- [requirements.txt](https://github.com/alinapetukhova/mn-ds-news-classification/requirements.txt): List of packages used in the training

### Results.


| Embeddings model  | TF-IDF precision  | TF-IDF recall | TF-IDF f1 score  | Glove precision  | Glove recall | Glove f1 score | DistilBertTokenizer precision | DistilBertTokenizer recall| DistilBertTokenizer f1 score
| :------------ |---------------:| -----:|-----:|-----:|-----:|-----:|-----:|-----:|-----:|-----:|-----:|
| Multinomial NB 	| 0.802 | 0.631 | 0.649 | 0.629 | 0.499 | 0.529 | n/a   | n/a   | n/a   | 
| Logistic Regression	| 0.800 | 0.763 | 0.774 | 0.747 | 0.739 | 0.739 | n/a   | n/a   | n/a   |
| SVC classifier 	| 0.808 | 0.796 | 0.799 | 0.768 | 0.762 | 0.760 | n/a   | n/a   | n/a   |
| DistilBERTModel 	| n/a   | n/a   | n/a   | n/a   | n/a   | n/a   | 0.849 | 0.842 | 0.844 |


| Multinomial NB 	| 0.628 | 0.602 | 0.583 | 0.496 | 0.484 | 0.469 | n/a | n/a | n/a |
| Logistic Regression	| 0.646 | 0.649 | 0.635 | 0.589 | 0.589 | 0.577 | n/a | n/a | n/a |
| SVC classifier 	| 0.645 | 0.646 | 0.628 | 0.581 | 0.595 | 0.571 | n/a | n/a | n/a |
| DistilBERTModel 	| n/a | n/a | n/a | n/a | n/a | n/a | 0.735 | 0.715 | 0.715 |

