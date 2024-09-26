# A-fine-tunning-of-Chat-gpt-based-on-user-s-feelings

## Project Overview
This project focuses on fine-tuning a pre-trained masked language model (MLM) on a dataset of French tweets scraped from the hashtag #JeudiConfession. The objective is to enhance the model's ability to understand and generate text within the specific context and style of these confessional tweets.

## Data Collection and Preprocessing
Data Source: We used the snscrape library to collect approximately 10,000 tweets from the #JeudiConfession hashtag.
Data Cleaning: The tweets were preprocessed to remove noise such as URLs, usernames, special characters, and emojis, ensuring a clean dataset for training.
Data Filtering: Only original tweets (not replies) and those within a specific token length range were kept to improve the quality of the training data.
Model Fine-tuning
Base Model: We utilized the "benjamin/gpt2-wechsel-french" model from Hugging Face's Transformers library as our foundation.
Customization: The model was further customized by unfreezing the last few transformer blocks and the language modeling head, allowing it to adapt specifically to the #JeudiConfession dataset.
Training: The model was fine-tuned using the Hugging Face Trainer API, with hyperparameters optimized for language modeling tasks.
Results and Evaluation
Improved Language Generation: The fine-tuned model demonstrates a better understanding of the nuances and style of #JeudiConfession tweets. It can generate more coherent and contextually relevant text compared to the original pre-trained model.
Qualitative Analysis: Sample outputs from the model showcase its ability to capture the confessional tone and generate creative text in line with the theme of #JeudiConfession.
## Technologies Used
Python
Hugging Face Transformers
Datasets library
snscrape
Pandas
PyTorch
evaluate
wandb
## Potential Applications
This fine-tuned model has several potential applications:

## Content Generation:
Generating engaging and relevant social media content for campaigns related to mental health or personal expression.
## Sentiment Analysis:
Analyzing the sentiment of #JeudiConfession tweets to gain insights into public opinion and emotions on various topics.
## Chatbot Development:
Creating a chatbot capable of understanding and responding to users in a natural and empathetic way, particularly in contexts related to confessions or personal struggles.
## Conclusion
This project highlights the power of fine-tuning language models on domain-specific datasets. The resulting model has demonstrated its ability to generate high-quality text within the context of #JeudiConfession tweets, opening up possibilities for various applications in the fields of data science and natural language processing.

Feel free to explore the code and experiment with the fine-tuned model! If you have any questions or suggestions, please don't hesitate to reach out.
