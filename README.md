**Automating Key Phrases Identification in Patient Notes**

Clinical Skills examination became a component of the United States Medical Licensing Examination(USMLE). Participants(Medical Students) in the exam had to communicate with standardized patients (people skilled in acting out particular clinical cases) and record patient notes. The patient notes are then scored by certified physicians using rubrics that list the key ideas in each case (also known as features). Among other things that affect the final test score, the more of these features are present in a patient note, the higher the score. However, it takes a lot of time and labor to have doctors grade patient note exams. To automate this process Kaggle has conducted a competition on the same. While the goal of Kaggle was to automate the evaluation and scoring process, I used this use-case to investigate the capabilities of the BERT model and its improvements, such as RoBERTa, PubMedBERT, and BioBERT, in language comprehension tasks by applying the models to the dataset that is now accessible.

The data was obtained straight from kaggle, with the entire zip file including four files as following:
1. features.csv - features rubric for each clinical case
2. patient notes.csv - history of patient notes
3. train.csv
4. test.csv

Note: The extracted data is stored in Dataset folder of the repository.

Implemented BERT-Base-Uncased, RoBERTa, PubMedBERT, BioBERT and compared which model works best in predicting the location of words in the paragraph which contains the feature contexts. The results showed that RoBERTa is the best model for predicting the location correctly having 94% of accuracy and with a computation time of 37 minutes.
