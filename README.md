 #   🍿🥤                                                             **Netflix Movies and TV Shows Clustring**
 
I have clustered similar movies and TV Shows available on Netflix taking into account of attributes like Description, Cast, Director, Genre etc of a particular movie/show.
![image](https://user-images.githubusercontent.com/87980985/212687453-28d4d6f1-c6d4-484e-8c0c-615aca0a3afa.png)

  AlmaBetter Verfied Project - AlmaBetter


## **📖Introduction**
Netflix, the world’s largest on-demand internet streaming media and online DVD movie rental service provider.it Founded August 29, 1997, in Los Gatos, California by Marc and Reed. It has 69 million members in over 60 countries enjoying more than 100 million hours of TV shows and movies per day Netflix is the world’s leading internet entertainment service with enjoying TV series, documentaries, and feature films across a wide variety of genres and languages. I was curious to analyze the content released in Netflix platform which led me to create these simple, interactive, and exciting visualizations and find similar groups of people.



## **📖 Problem Statement**
In 2018, they released an interesting report which shows that the number of TV shows on Netflix has nearly tripled since 2010. The streaming service’s number of movies has decreased by more than 2,000 titles since 2010, while its number of TV shows has nearly tripled. It will be interesting to explore what all other insights can be obtained from the same dataset.

Integrating this dataset with other external datasets such as IMDB ratings, rotten tomatoes can also provide many interesting findings.

## **Steps Involved:**

* Exploratory Data Analysis

* Understanding what type content is available in different countries

* Is Netflix has increasingly focusing on TV rather than movies in recent years.

* Clustering similar content by matching text-based features

## **📖 Data Summery**

* **show_id :** Unique ID for every Movie / Tv Show

* **type :** Identifier - A Movie or TV Show

* **title :** Title of the Movie / Tv Show

* **director :** Director of the Movie

* **cast :** Actors involved in the movie / show

* **country :** Country where the movie / show was produced

* **date_added :** Date it was added on Netflix

* **release_year :** Actual Releaseyear of the movie / show

* **rating :** TV Rating of the movie / show

* **duration :** Total Duration - in minutes or number of seasons

* **listed_in :** Genere

* **description:** The Summary description

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
