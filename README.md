 #   🍿🥤                                                             **Netflix Movies and TV Shows Clustring**
 
![image](https://user-images.githubusercontent.com/87980985/212687453-28d4d6f1-c6d4-484e-8c0c-615aca0a3afa.png)

In this project i have clustered similar movies and TV Shows available on Netflix taking into account of attributes like Description, Cast, Director, Genre etc of a particular movie/show.

 AlmaBetter Verfied Project - AlmaBetter


## **📖Introduction**
Netflix, the world’s largest on-demand internet streaming media and online DVD movie rental service provider.it Founded August 29, 1997, in Los Gatos, California by Marc and Reed. It has 69 million members in over 60 countries enjoying more than 100 million hours of TV shows and movies per day Netflix is the world’s leading internet entertainment service with enjoying TV series, documentaries, and feature films across a wide variety of genres and languages. I was curious to analyze the content released in Netflix platform which led me to create these simple, interactive, and exciting visualizations and find similar groups of people.



## **📖 Problem Statement**
In 2018, they released an interesting report which shows that the number of TV shows on Netflix has nearly tripled since 2010. The streaming service’s number of movies has decreased by more than 2,000 titles since 2010, while its number of TV shows has nearly tripled. It will be interesting to explore what all other insights can be obtained from the same dataset.

Integrating this dataset with other external datasets such as IMDB ratings, rotten tomatoes can also provide many interesting findings.

## **Steps Involved:**


**1. Exploratory Data Analysis:**

* **a. Understanding the data-** In this step after loading the data I performed head, tail, columns, info, dtypes, describe functions to get basic information about our dataset.

* **b. Checking for missing & duplicated values-**  Then I checked for missing values in our dataset using is null function. Some of our features had missing values that I filled with ‘unknown’

**2. Cleaning Dataset & Feature Engineering-** As some of our features has got null values, I filled all null values with ‘unknown’ using fillna method. Then I extracted date, month and year from date added column. Renamed the listed in column to genres.

**3. Data Visualization –** In data visualization I got some insights like, in type of content, around 69% content as movies and remaining 31% as TV shows are present on Netflix. Then in genres International movies, dramas and comedies are most occurred types. In content addition day wise we can clearly spot the insights that Netflix majorly add the content on the 1st day of every month. In rating column most of the given rating is for mature adults (TV-MA) for both TV shows and Movies. In countries column US, India and UK are the top 3 most occurred countries. Then another graph shows that from 2017 number of Movies added increased tremendously, but at the same time TV shows added from 2017 are also increased but as comparison to Movies they are very less in numbers

**4. Feature Engineering-** After data visualization I did feature engineering in which I added a new column which contains all the text and categorical column data, so that we can work on entire text data. Then used snowball stemming to stem the text into the column. After stemming and other cleaning operations I applied TF-IDF vectorizer on the text. Applied Principal Component Analysis (PCA) to reduce the dimensions of X.


**5. Model Building**

* **KMeans Clustering-** K-Means Clustering is an Unsupervised Learning algorithm, which groups the unlabeled dataset into different clusters The K-Elbow Visualizer implements the “elbow” method of selecting the optimal number of clusters for K-means clustering. Then no. of cluster k=15 selected. After that fitted the model on data and then predicted the labels. Then assigned the clusters in datasets and then visualized each cluster using word cloud.

**6. Evaluating Models**

* **Silhouette Score -** Silhouette analysis can be used to study the separation distance between the resulting clusters. The silhouette plot displays a measure of how close each point in one cluster is to points in the neighboring clusters and thus provides a way to assess parameters like number of clusters visually. This measure has a range of [-1, 1]. We selected number of clusters as 15 which in above calculations showing 0.78 as silhouette score


## **📖 Data Summery**

This dataset consists of tv shows and movies available on Netflix as of 2019. The dataset is collected from Fixable which is a third-party Netflix search engine. In 2018, they released an interesting report which shows that the number of TV shows on Netflix has nearly tripled since 2010. The streaming service’s number of movies has decreased by more than 2,000 titles since 2010, while its number of TV shows has nearly tripled. It will be interesting to explore what all other insights can be obtained from the same dataset. Integrating this dataset with other external datasets such as IMDB ratings, rotten tomatoes can also provide many interesting findings.



![image](https://user-images.githubusercontent.com/87980985/213904069-06e1523e-2ce8-40c4-a499-896568d80bea.png)

### **First 5 rows of dataset**

![Screenshot 2023-01-22 122014](https://user-images.githubusercontent.com/87980985/213904290-c8165987-7e98-4f94-8140-846cd4da0c33.png)

## **Conclusion**

**1) We observe that in this dataset 4,000+ movies and almost 2,000 shows with movies being the majority. This makes sense since shows are always an ongoing thing and have episodes.in terms of title, there are far more movie titles (69.1%) than TV show titles (30.9%).**

**2) Films typically are available in multiple countries as shown in the dataset. Therefore, we need to seperate all countries within a film before we can analyze the data(create first_country column). After seperating countries and removing titles with no countries available, we can plot a Top 10 list to see which countries have the highest availability of films on Netflix. Unsurprisingly, the United States stands out on top since Netflix is an American company. India surprisingly comes in second followed by the UK and Canada.**

**3) In terms of genres, international movies takes the cake surprisingly followed by dramas and comedies. Even though the United States has the most content available, it looks like Netflix has decided to release a ton of international movies. The reason for this could be that most Netflix subscribers aren't actually in the United States, but rather the majority of viewers are actually international subscribers.**

**4) From the lineplot we can conclude that the most number of TV Shows released in 2017 and for Movies it is 2020.Spain have the newest content overall(both Movie & TV-Shows)**

**5) The end & beginnings of each year seem to be Netflix's preference for adding content.Least number of contents are added in the month of February.**

**6) On netflix there is much more content for a more mature audience. For the mature audience, there is much more movie content than there are TV shows. However, for the younger audience (under the age of 17), it is the opposite, there are slightly more TV shows than there are movies.**

**7) The most popular actor on Netflix movie, based on the number of titles, is Anupam Kher.**

**8) The most popular actor on Netflix TV Shows based on the number of titles is Takahiro Sakurai.**

**9) In text analysis (NLP) I used stop words, removed punctuations , stemming & TF-IDF vectorizer and other functions of NLP.**

**10) We Applied different clustering models like Kmeans, Agglomerative clustering, DBSCAN on data we got the best cluster arrangements.**

**11)  By applying different clustering algorithms to our dataset .we get the optimal number of cluster is equal to 3.**

## **📚 References**

 https://www.kaggle.com/code/onyonixch/netflix-movies-tv-shows-eda-and-clustering
 
 https://www.youtube.com/watch?v=d320GGtY-3s


