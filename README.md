# Political-speeches-classification

This was the third assignment for the course "Applied Machine Learning" of AUEB's Management Science and Technology Department. We had to classify speeches given in the parliament to the political party the speaker belonged (or stills belongs). 

Firstly, I had to do some data cleaning and selection and then I used some methods from scikit learn such as Naive Bayes, Logistic Regression and SVMs to classify the speeches. During this phase I also used GridSearch for Hyperparameter tuning and had to tackle the problem of unbalanced data (some parties had far more speeches than others). Before applying these algorithms, I also had to choose an appropriate representation for the texts to "feed" into the ML algorithms.

After the "traditional" machine learning methods, I used neural networks (implemented with keras) to classify the speeches. The results were worse than those of the previous methods, but still acceptable.

Finally, I tried to write a function that takes as input a party, a starting word and a desired text length and generates a (hypothetical) speech of the given party, starting with the given word and with the given length (in words, excluding the starting word). The function manages to use the desired vocabulary according to the party given and achieves a little structure in the speeches produced, but fails to do so in the level humans speak. In other words it (kind of) produces speeches that could have been given by a drunk politian of the respective party.

The data used can be found here: https://zenodo.org/record/2587904
