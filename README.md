# Class-Reccomennder
Allows users to key in classes they have taken which the system then recommend a class from the list of classes they are eligible for.

Using McgGill database for classes from the faculty of Science, we cleaned the data into columns of pre-requisites before fine-tuning a Genism Word2Vec model using the description of the classes and we evaluate classes similarity based on the cosine similarity between the word-embeddings of the class description.
