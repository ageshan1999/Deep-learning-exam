README
Data:
The data we use in the project: https://huggingface.co/datasets/financial_phrasebank
The data is sentences from financial news. The data is catagorised by sentimennt, where 0=negative, 1=neutral and 2= positive.
The dataset is loaded using the Hugging Face datasets library and split into training and testing sets.

Model:
We convert the data into a pandas dataframe , and removes empty rows. We split the data into a training and test set, and convert it back to a huggingface dataframe.
Next we are tokenizing text data using the BERT-base-cased tokenizer and creating tokenized versions of the training and test datasets. Then we setup different trainning arguments as, epohs and batchsize.Then we train the model with the specifed arguments and dataset. At last we create a Grado app, where the input is a text, and the model will predict whether it is negative, neutral or poositive.






