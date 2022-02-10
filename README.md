# Document-Clustering

Nowadays we are constantly bombarded with new content and new articles, a few hundred to thousand articles, related to various topics, are produced per day and so 
organisation of all these articles is essential or else old content gets lost as we try to accommodate the new one.Thus, an optimal method to identify and organise the arriving document with the old ones is absolutely essential.

### Document clustering, a ML based approach where we apply cluster analysis to textual documents in our case articles (Wikipedia), thereby organising new articles and documents effectively for easy search and retrieval.

By using this method, we can also ensure that the user who searches any document or article is not overwhelmed by the *amount of content and ends up finding the right one faster.*

The Three main concepts used are as follows:
1. Term-frequency(tf)/ Inverse document-frequency(idf) 
2. Elbow Method
3. K-means clustering

#### Term-frequency(tf)/ Inverse document-frequency(idf) :
![This is an image](https://miro.medium.com/max/1400/1*V9ac4hLVyms79jl65Ym_Bw.jpeg)

Term Frequency(TF) is a measure for checking the originality of a word by comparing the number of times a word appears in a document with the number of documents the word appears
in and Inverse document frequency(IDF) is required since might be repetition of few terms like “is”, “or” etc. which are not that important so we need to weigh the frequent terms while scale up the rare or uncommon words which is done by calculating IDF.

#### Elbow-Method and K-Means Clustering:
![This is an image](https://static.javatpoint.com/tutorial/machine-learning/images/k-means-clustering-algorithm-in-machine-learning13.png)

Elbow method is to determine the optimal value for number of clusters in k-means clustering.
Kmeans clustering is a clustering algorithm which first initializes k-points randomly and then by finding Euclidean distance assign all the points to nearest centroids therefore creating k groups then we find the original centroid by calculating the average after which we reassign the whole data points on this new centroid then repeat the last step until the centroid position doesn’t change.

#### Word-Cloud for easy Visualization: 
![This is an image](https://miro.medium.com/max/1400/1*V9ac4hLVyms79jl65Ym_Bw.jpeg)
To display the final output of the project we used wordcloud which is generally used for representing the text data where the size of each word defines its frequency or  importance in the document. This is generally used to find the significant textual data point by indicating with large size. In the process of generating the wordcloud we use   matplotlib, pandas to read the file.
