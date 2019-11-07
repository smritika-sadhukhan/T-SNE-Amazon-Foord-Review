# T-SNE-Amazon-Foord-Review


In this assignment I was asked to have TSNE plot for the POSITIVE and NEGATIVE reviews of the customer using the following technigues :


1) BAG OF WORDS
2) TFIDF W2V
3) AVG W2V
4) TFIDF
 
 
 
STEP ARE AS FOLLOWS :
 
1) I have imported all the modules that i might required
2) Connected the notebook with "database.sqlit"​
3) Changed all the scores with more than 3 to 'positive' and less than 3 to 'negative' and did not consider score 3
4) Removed all the dublicates or information that are irrelevant and got the FINAL dataset
5) Text processing to clean the text using STOPWORDS and finaly got CLEANEDTEXT



FOR BOW

1) Using count_vectoriser()  transform  final['CleanedText'] to find "final_counts"
2) Standerdising the data using " final_count.toarray()
2) using the standerdised data and score ploted  the tsne plot


FOR TFIDF

1) Using tdidfVectoriser()  transform  final['CleanedText'] to find "final_tf_idf"
2) Standerdising the data using "final_tf_idf.toarray()"
2) using the standerdised data and score ploted  the tsne plot



FOR AVGW2V

1)Appling word 2 vector got list of words(w2v_words) with 50 dimention
2)applied avgw2v to find the sentence_vector
3)used sentence_vector to standerdise the data
4) using the standerdised data and score ploted  the tsne plot

FOR TFIDF_W2V

1)Created the model using "tdidfVectoriser()" 
2)applied tdfidf avg using the model to find tfidf_sent_vectors
3)used tdidf_sent_vector to standerdise the data
4) using the standerdised data and score ploted  the tsne plot
