# Similarity_Measure

This is an assesment for Fetch Rewards, which calculates the similarity between two sentences. Change `text_1`, `text_2`, `text_3` if you want to calculate similarity between other some other sentence.  

The similarity measure is calculated using the cosine simimalrity `$Cos(\theta) = \frac{A•B}{||A||*||B||}$`. Here, A and B are two vectors, so we need to convert the input text to vectors. 

This was acheived by calculating the TF-IDF matrix, $TF = \frac{Term \ Frequency \ in \ Document}{Total \ Terms \ in \ Document}, IDF = \frac{log(Total \ Documents)}{Documents \ with \ Term} and TF-IDF = TF*IDF$


