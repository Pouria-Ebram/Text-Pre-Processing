# Text-Pre-Processing
This is a Python implementation of a text pre-processor used to obtain a vocabulary dictionary and a vectorised version of a pdf file containing text from Monash university units information

In this analysis I extract data from a PDF-based corpus containing 200 Monash University units information. I have converted the pdf file using https://pdftotext.com/ to a text file for pre-processing using this Jupyter notebook code. The original pdf file includes units synopsis and units outcomes in two seperate sections which we have extracted.

The pre-processing tasks at a high level include:

    1- Normalising units information with respect the words location in sentences according to specification request
    2- Tokenisation of units information
    3- extraction of bigrams using PMI measure
    4- re-tokenisation of units information with respect to the bigrams
    5- Removal of context independant and dependant stop words and rare words from the vocabulary
    6- Stemming of the tokens using the nltk PorterStemmer
    7- Creating a text file including the sparse count vector for each unit
