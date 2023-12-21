# Vietnamese Student Feedback Sentiment Analysis Project
---
In this Project, I have used the Corpus named Vietnamese Student Feedback Corpus, which belongs to The UIT NLP Group and has more than 16,000 feedback from Vietnamese students, to solve the Sentiment Analysis task. I have done some models and chosen the best model which has resulted in the following table

## Model used:
|Model|Feature|Precision|Recall|F1-Score|Accuracy|
|---|---|---|---|---|---|
|LSTM| Word2Vec|90.0|89.7|89.8|89.7|

---
## Wep Application
We have built a web application for Analyzing the Sentiment of Vietnamese Student's Feedback

### Corpus Analysis
You can browse the corpus with a lot of feedbacks like 4 corpus in [Data/testForApp](Data/testForApp) directory. The application will predict the sentiment for each feedback, then display the dataframe of result and the chart for analysis.
<p align = "center">
    <img src="images/forapp/corpus1.png" alt="workflow" width="70%">
</p>

<p align = "center">
    <img src="images/forapp/corpus2.png" alt="workflow" width="70%">
</p>

<p align = "center">
    <img src="images/forapp/corpus3.png" alt="workflow" width="70%">
</p>

### Sentence's Sentiment Analysis
You can input a Vietnamese feedback about school or university, the application will predict the sentiment and display the polarity beside.
<p align = "center">
    <img src="images/forapp/sentiment1.png" alt="workflow" width="70%">
</p>

<p align = "center">
    <img src="images/forapp/sentiment2.png" alt="workflow" width="70%">
</p>

---
## How to use?
#### Clone the project
```bash
git clone https://github.com/VuBacktracking/
```
#### Install required packages

```bash
pip install -r requirements.txt
```

#### Generate model (optional)
We already ran and saved the model `lstm_model.h5` in `models` directory

```bash
#run this file to generate the models
lstm_create_model.ipynb
```
```bash
#run this file to check the result of model
lstm_result.ipynb
```

#### Now run
``` bash
streamlit run app.py
```
___
## Future Work