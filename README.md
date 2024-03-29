README Data: The data we use in the project: https://huggingface.co/datasets/financial_phrasebank The data is sentences from financial news. The data is categorized by sentiment, where 0=negative, 1=neutral, and 2= positive. The dataset is loaded using the Hugging Face datasets library and split into training and testing sets.

Model: We convert the data into a pandas data frame, and remove empty rows. We split the data into a training and test set, and convert it back to a hugging face data frame. Next, we tokenize text data using the BERT-base-cased tokenizer and create tokenized versions of the training and test datasets. Then we set up different training arguments as, epochs and batchsize. Then we train the model with the specified arguments and dataset. At last, we create a Grado app, where the input is a text, and the model will predict whether it is negative, neutral, or positive.

The link for the model which is uploaded in Hugging face, can be seen here:
https://huggingface.co/Thysted/M3-DeepLearning
