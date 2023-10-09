# Bangla-YouTube-Sentiment-Analysis-App
Given a VideoId of any YouTube video (Bangla), this application is designed to do sentiment analysis on the comments of the said video and provide opinion score and polarity of the viewers. Works best with GPU support.
We used YouTube API for fetching the comments. 
We have developed, trained and fine-tuned a state-of-the-art transformer model for this sentiment analysis task. The model is available on the link below https://huggingface.co/Arunavaonly/Bangla_multiclass_sentiment_analysis_model

#Model Development:
The base architecture is roBERTa, which is an optimised version of BERT (Bidirectional Encoder Representations from Transformers). We have trained and fine-tuned roBERTa architecture to develop this three class sentiment analysis model. The model achieves 93% f1 score on the test dataset. The model has been trained specifically for Bangla-English code-mixed situations. The data contains Bangla, English and Romanised Bangla sentences. Special care has been taken to include both Bangladeshi and West Bengali varieties of Bangla. We have trained the model for 3 epochs and fine-tuned it with learning-rate 3e-05.

#Application:
The user needs to provide videoid of a YouTube video (Bangla). The application would then fetch the comments from the video and analyse them. It is recommended to use GPU if the number of comments is very large. The application would provide the polarity and opinion score. There are five different polarities: Extremely Positive, Positive, Neutral, Negative, Extremely Negative.

#What I Learned
1. Basic architecture of the transformer models
2. Masked language models like BERT
3. Details about BERT and the versions of BERT like roBERTa
4. Training and fine-tuning with transformer models, adding the output layer
5. Testing and employing the model for real world tasks
6. Designing a sentiment analysis project from scratch.
