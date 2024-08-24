-Sentiment Analysis on E-commerce Dataset
I'm excited to share my recent project that leverages the power of transformers and the Hugging Face library for sentiment analysis on an e-commerce dataset. The goal of this project was to analyze product sentiment using two models: bert-base-uncased and microsoft/MiniLM-L12-H384-uncased.

-Dataset and Preprocessing
The dataset used for this project was an e-commerce dataset available on Hugging Face, containing reviews in Indonesian and English. I cleaned the dataset by removing Indonesian reviews and correcting spelling errors. The sentiment was represented by 1 for positive and 0 for negative. Since the dataset only contained training data, I created a test set using the train test split method.

-Tokenization
I imported the tokenizer from the transformers library and applied it to the dataframe. Initially, I faced issues with tokenization, but I resolved them by converting the dataframe back to a Hugging Face dataset using the dataset.from_pandas method.

-Model Training
I trained two models: bert-base-uncased and microsoft/MiniLM-L12-H384-uncased. Both models performed similarly in terms of accuracy, but I chose the microsoft/MiniLM-L12-H384-uncased model WHY ?

-Model Evaluation
Both models performed similarly in terms of accuracy. However, the microsoft/MiniLM-L12-H384-uncased model was chosen due to its lower validation loss, indicating better generalization to unseen data.

-Sentiment Analysis
The trained model was used to perform sentiment analysis on product reviews, outputting sentiment as either positive or negative.

-Conclusion
This project demonstrates the application of transformers and the Hugging Face library for sentiment analysis on an e-commerce dataset. Despite initial challenges with tokenization, the project was successful, and the microsoft/MiniLM-L12-H384-uncased model provided the best performance.
