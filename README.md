# Kaggle Competition: [HR Analytics: Job Change of Data Scientists](https://www.kaggle.com/datasets/arashnic/hr-analytics-job-change-of-data-scientists)

___

A company which is active in Big Data and Data Science wants to hire data scientists among people who have successfully passed some courses conducted by the company. Many people signed up for the training. The company now wants to know which of these candidates is actually open to work for them (= change their job) after the training.

___

## Setup of virtual environment

```
pyenv local 3.9.8
python -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```

## Conclusion

I did find out some interesting things about the data and, above all, learned a lot while working with this data set. 

But the performance of the model is not too satisfactory: 80% accuracy and 61% precision are not exactly outstanding. However, I also believe that you can't make perfect predictions with this data set. There are too few relevant features in it. 

On Kaggle I saw notebooks with significantly better performances. However, I also saw a lot of technical errors in these notebooks, especially I saw many notebooks where the sampling with SMOTE was applied BEFORE the train test split. 

If I worked like this, I would also have a much better precision (77 instead of the current 60%, I tested it), but of course this is a blatant case of data leakage. I prefer to work cleanly and realistically, even if the result is not so impressive at first glance. With some data sets you simply cannot achieve better performance. 

