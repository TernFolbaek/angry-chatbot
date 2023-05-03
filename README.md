# Resentful Bot

### The objective of this project was to investigate the retort of a chatbot that was trained on a dataset comprising pessimistic data, in responding to daily inquiries and questions. To achieve this, the initial step was to develop a sentiment analysis model capable of detecting the polarity (i.e., positive, negative, or neutral) of textual data. Subsequently, the model was employed to extract specific data from a larger dataset, which was split into two halves, with the first half used as input and the second half as output. However, this approach is (surprise surprise) suboptimal, and there is a need for a more comprehensive dataset to train the chatbot better. Therefore, the search for an optimal dataset is ongoing.

### Files & their purpose
  * #### sentiment_detection:
    * This file is used to train the model which detects the polarity of a textual message, utilizing twitter_training.csv as its data, as it has a column dedicated for its text, and the corresponding value which is either         pstive/negative/neutral
