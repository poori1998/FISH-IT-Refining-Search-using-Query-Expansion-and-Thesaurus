# FISH-IT-Refining-Search-using-Query-Expansion-and-Thesaurus

The proposed project is related to refining the list of retrieved documents by using a thesaurus and using the concept of query expansion. 
We use an electronic thesaurus to obtain the words related to the user query and search is performed on a new altered, more specific query.

First, we obtain the query entered by the user, then we proceed by preprocessing it ,i.e., we remove punctuations, and stopwords, then we continue stemming them and finally, we tokenize all the words in the query. 
Now with the help of WordNet (WordNet is a lexical database for the English language. It groups English words into sets of synonyms called synsets, provides short definitions and usage examples, and records a number of relations among these synonym sets or their members. WordNet can thus be seen as a combination of dictionary and thesaurus), by including nltk.corpus, we find synonyms for each token in the query and then append them to it , therefore forming a modified, expanded, and more broad query. 
We then search for results with the help of this new query via Google. We observe that the results obtained now are more specific and more relevant as compared to a search done w.r.t the initial query. 

>>The Frontend consists of the GUI made with tkinter (Tkinter is a Python binding to the Tk GUI toolkit. It is the standard Python interface to the Tk GUI toolkit, and is Python's de facto standard GUI. Tkinter is included with standard Linux, Microsoft Windows and Mac OS X installs of Python).
 The upper label consists of the name of the GUI and also includes a logo . On the bottom , we have a label box where the user is supposed to enter his or her initial query. This query is then fetched by the backend and worked upon with, thereby creating the expanded query. This new query is shown at the bottom most part of the GUI. The new query is linked to google and the results are obtained.
In the above example, the initial query is “gift ideas for teachers”. The query is split, preprocessed and tokenized . As seen in the image, the query is changed to its form containing the synonyms of the tokenized words(the synset obtained from WordNet). 
Google now does not search for “gift ideas for teachers”, instead it searches for the expanded form of it.	
