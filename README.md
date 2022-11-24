# Countvectorizer2



#CODE BY AMMAR#



from sklearn.feature_extraction.text import CountVectorizer

document = ["How Are You Mr Ammar",
			"It's Pleasure To Meet You",
			"So You work in a marketing"]

# Create a Vectorizer Object
vectorizer = CountVectorizer()

vectorizer.fit(document)

# Printing the identified Unique words along with their indices
print("Vocabulary: ", vectorizer.vocabulary_)

# Encode the Document
vector = vectorizer.transform(document)

# Summarizing the Encoded Texts
print("Encoded Document is:")
print(vector.toarray())
