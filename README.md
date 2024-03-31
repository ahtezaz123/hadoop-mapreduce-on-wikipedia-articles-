# HADOOP MAPREDUCE ASSIGNMeNT
This is our python big data analytics assignment using Hadoop MapReduce to do the tasks mentioned below on a dataset of 5 million Wikipedia articles.

# Collaborators
This work was completed with the help of :
- https://github.com/ahtezaz123
- https://github.com/shabanhassan142


# Dependancies 

1. pandas
2. NLTK (Natural Language Toolkit)
3. re (Regular Expressions)
4. math
5. textblob

These dependencies can be installed via pip, Python's package manager, using the following commands:

- pip install pandas
- pip install nltk
- pip install textblob

Additionally, before running the code, NLTK's data files need to be downloaded. This can be done by running the following Python code after installing NLTK:

- import nltk
- nltk.download('punkt')
- nltk.download('stopwords')
- nltk.download('wordnet')

Once these dependencies are installed and the necessary NLTK resources are downloaded, the provided code should execute without any issues.


# 1. Data Preprocessing with NLTK and TextBlob:

For Data Preprocessing we imported necessary libraries including NLTK, TextBlob, and pandas for data manipulation and text preprocessing tasks and downloaded required NLTK resources such as tokenizers, stopwords, and WordNet. Moreover, we applied basic text preprocessing techniques including tokenization, removal of HTML tags, conversion to lowercase, removal of stopwords and then implemented stemming and lemmatization to normalize text tokens.
After that we cleaned the text data by removing HTML tags and converting it to lowercase to ensure consistency and ease of processing.


# 2. Mapper and Reducer Functions:

Developed custom mapper and reducer functions to process text data and calculate term frequencies (TF) and TF-IDF scores.
Utilized regular expressions to tokenize text data and count word occurrences efficiently.
Aggregated word counts for each document in the reducer function and calculated TF scores.
Implemented a second mapper and reducer to compute TF-IDF scores using IDF values obtained from the preprocessed data.

# 3. Integration with Pandas DataFrame:

Loaded preprocessed data from a CSV file into a pandas DataFrame for further analysis.
Performed data cleaning and text preprocessing tasks such as HTML tag removal, tokenization, and removal of stopwords.
Applied stemming and lemmatization techniques to normalize text tokens and reduce dimensionality.

# 4. TF-IDF Calculation:

Calculated IDF (Inverse Document Frequency) for each term in the corpus.
Implemented a second mapper function (second_mapper) to calculate TF-IDF (Term Frequency-Inverse Document Frequency) for each term in each document.
Implemented a second reducer function (second_reducer) to aggregate TF-IDF scores for each term and document.
Applied these mapper and reducer functions to generate TF-IDF values for each term-document pair.

# 5. Query Tokenization:

Tokenized queries using a custom tokenization function (tokenize_query).

# 6.  TF-IDF Retrieval:

Calculated TF-IDF scores for each term in each document and displayed the results.

# 7. IDF Calculation and Integration:

Calculated IDF values for each term in the dataset and added them to the DataFrame.
Extracted term frequencies for each document and represented them using the TF-IDF values.

# 8. Reporting:

Utilized print statements to display various results such as preprocessed data, TF-IDF values, IDF values, and term frequencies for each document.
Overall, the provided code demonstrates a comprehensive approach to text preprocessing, TF-IDF calculation, and information retrieval tasks using Python and relevant libraries such as NLTK and pandas. The code follows a structured approach, making it easier to understand and maintain.

# 9. Conclusion:

The preprocessing and transformation steps significantly improved the quality and consistency of the text data.
Integration with NLTK and TextBlob libraries facilitated efficient text processing and analysis.
The calculated TF-IDF scores provide valuable insights into the importance of terms in individual documents relative to the entire document collection.
