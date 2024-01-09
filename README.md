# Similarity_Measure

This is an assessment for Fetch Rewards, which calculates the similarity between two sentences. Change `text_1`, `text_2`, and `text_3` if you want to calculate the similarity between other some other sentences.  

### Punctuation and stop words

Here, I've considered both punctuation and stop words for the calculations but to make it much better they should not be considered as they appear in every sentence and it will give `0` in the calculation of tf-idf. $TF = \frac{Term \ Frequency \ in \ Document}{Total \ Terms \ in \ Document}, IDF = \frac{log(Total \ Documents)}{Documents \ with \ Term} \ and \ TF-IDF = TF*IDF$

### Words to matter in similarity comparison 
The common words between two sentences should be taken into account when finding out the similarity. This is calculated using tf-idf

### Ordering of words

The ordering of words does matter when calculating similarity and it can be implemented using `Transformers`. It is not implemented here.

### Metric to calculate similarity

The similarity measure is calculated using the cosine simimalrity $Cos(\theta) = \frac{A•B}{||A||*||B||}$. Here, A and B are two vectors, so we need to convert the input text to vectors. It handles sparse data and also is not affected by the magnitude of the vectors.

### Data Structures to be used

The most common and efficient data structure used is the hash map or dictionary. It stores the frequency of the words so that retrieval is only O(1) when calculating the tf-idf and similarity.

### Results 

Sentences 1 and 2 have a higher similarity of 74% than sentences 1 and 3 with 63%.

# Instructions to run

The `similarity_measure.ipynb` has a Google Colab Notebook link. It has the texts, just need to select `Rull all` from the `Runtime` tab.
