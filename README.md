# Resentful Bot

#### The objective of this project was to investigate the retort of a chatbot that was trained on a dataset comprising pessimistic data, in responding to daily inquiries and questions. To achieve this, the initial step was to develop a sentiment analysis model capable of detecting the polarity (i.e., positive, negative, or neutral) of textual data. Subsequently, the model was employed to extract specific data from a larger dataset, which was split into two halves, with the first half used as input and the second half as output. However, this approach is (surprise surprise) suboptimal, and there is a need for a more comprehensive dataset to train the chatbot better. Therefore, the search for an optimal dataset is ongoing.

### Files & their purpose
  * #### sentiment_detection:
    * This file is used to train the model which detects the polarity of a textual message, utilizing twitter_training.csv as its data, as it has a column dedicated for its text, and the corresponding value which is either       positive/negative/neutral.
  * #### angryGPT:
    * This file is dedicated to the training of the chatbot itself. Importing the previous model from sentiment_detection using "model.pkl". Importing the data-set "utterances.jsonl" and converting it to a csv file which 
      we named "provoking_file.ipynb". In the file we import certain Hugging Face Transformers to deal with the NLP training, and at last export our new-found model to "my_model.pkl"
  * #### app.py: 
    * The file which runs this project in the browser using a well known machine-learning/data-science library named streamlit. Which is the reason we have a "venv" as the versions of certain libraries were not compatible         with others. If you were to clone this repository and run it yourself (keep in mind we used google colab to run angryGPT as our personal computers did not have the adequate power themselves) then all you would have to
      prompt the terminal is "streamlit run app.py" to get it running in the browser.
