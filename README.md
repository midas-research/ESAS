# ESAS
Public implementation of ESAS

Features : 
# Contextual Feature Overlap (1) 
File Name : Feature1_ContextFeatures.ipynb
* Rake is used to take out key words from all the questions.
* Page-Rank (Google) is used to give importance to all the words, saving them in a CSV file from most to least important.
* Wikipedia Article for top 1st word in removed in for each prompt.
*Cosine Similarity between each essay and its respective prompt – wikipedia article is found and saved.

# POS Overlap (2)
File Name : Feature2_POS_Tags_Overlap.ipynb
For a question answer pair: 
Extract POS tags from.the question and calculate max_count_tag which could be a noun, verb, adjective or adverb. 

Extract the POS tags from the answer and then take an intersection of the max_count_tags. 

Divide this by the length of max_count_tag which will be the ratio for the corresponding question-answer pair.

# Concept Overlap(3) 
File Name :Feature3_ConceptOverlap_UsingBERT.ipynb
           Feature3_ConceptOverlap_UsingDoc2Vec.ipynb

*Find doc2vec or Bert embeddings for sample response of each prompt.
*Find Doc2Vec or Bert embedding for each response.
*Compare cosine similarity of the response with the respective prompt’s sample response.
