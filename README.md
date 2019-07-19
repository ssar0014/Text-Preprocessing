# Text-Preprocessing

Environment: Python 3.6.8 and Jupyter notebook

Libraries used:
slate3k - To read PDF files as text in Python
re - To use regular expressions in Python
pandas - To make use of Pandas dataframes for ease of use in computation
nltk - To use NLP in Python, like Stemming, tokenization, etc


The following code reads a given PDF file with tabular data, parses the data from it, and gives out 2 files - 29819253_vocab.txt and
29819253_countVec.txt, the first file containing vocabulary, and their indices, and the second file containing the occurrences of these words along with their word frequencies


The following code reads tabular data from a PDF file named 29819253.pdf which contains information about subjects offered by a Univeristy. It contains details about the Unit code, synopsis, and outcomes written as a table.

This data is read using the slate3k library which is built on top of the PDFMiner library. It enables us to read tabular data as text. This text is then converted to a Pandas Dataframe.

Regular Expressions were extensively used to extract and clean the data.

From this extracted data inside the dataframe, text preprocessing was done on a set of unit information and then converted into numerical representations which are suitable for input into recommender-systems/ information-retrieval algorithms.

The data-set that was provided contains 400 unit information crawled from Monash University. The pdf file contains a table in which each row contains information about a unit which is unit code, synopsis, and outcomes. The task was to extract and transform the information for each unit into a vector space model.

I have included the jupyter notebook containing detailed code and comments.
