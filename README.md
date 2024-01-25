# Netflix_Movies_and_TV_Shows_Clustering_capstone_project


## Business Context

### This dataset consists of tv shows and movies available on Netflix as of 2019. The dataset is collected from Flixable which is a third-party Netflix search engine. In 2018, they released an interesting report which shows that the number of TV shows on Netflix has nearly tripled since 2010. The streaming service’s number of movies has decreased by more than 2,000 titles since 2010, while its number of TV shows has nearly tripled. It will be interesting to explore what all other insights can be obtained from the same dataset.

Integrating this dataset with other external datasets such as IMDB ratings, rotten tomatoes can also provide many interesting findings.

In this project, you are required to do

- Exploratory Data Analysis
- Understanding what type content is available in different countries
- If Netflix has been increasingly focusing on TV rather than movies in recent years.
- Clustering similar content by matching text-based features


Dataset Description


| Variable Name | Description |
|---|---|
| title | Title of the movie or TV show. |
| director | Director of the movie or TV show. |
| cast | List of actors and actresses who starred in the movie or TV show. |
| country | Country where the movie or TV show was produced. |
| date_added | Date on which the movie or TV show was added to Netflix. |
| release_year | Year in which the movie or TV show was released. |
| rating | Rating of the movie or TV show on Netflix. |
| duration | Duration of the movie or TV show in minutes. |
| listed_in | List of genres to which the movie or TV show belongs. |
| description | Description of the movie or TV show. |




Main Libraries used:

- Pandas for data manipulation, aggregation
- Matplotlib and Seaborn for visualization and behavior with respect to the target variable
- NumPy for computationally efficient operations
- NLP

# Conclusion


1. The purpose of the project was to explore how different movie and TV shows on Netflix can be grouped together based on their features, such as genre, director, and rating.

2. For this we started with data wrangling, handling null values, exploratory data analysis. Some of the key insights from our exploratory data analysis are-:

- There are more obervations of Movies than TV shows in our dataset.
- But in the recent years Netflix has been focusing more on Tv-Shows.
- The majority of the rated content on Netflix falls into the TV-MA(indicating that mature content is more popular on Netflix.) and TV-14 categories.
- Number of TV shows and movies on Netflix has increased significantly since 2010.
- Documentaries, Stand-up Comedy, Drama, International movies and comedies are some of the highly popular content on the platform. the reason being people use ott platforms as the source of entertainment and they often love the content that is more relatable to their life and feel real.
- USA and India are topmost countries in producing content over the platform.
- Between 2017-2019, the maximum content is released or added to the platform.
- Maximum number of content is released in the month of December and january.
- Netflix has over 30% original content which shows that netflix invests heavily in creating and promoting their own original content.
- US and UK are closely aligned with their Netflix target ages, means that people in both USA and UK prefer to watch similar type of content.

3. Then we applied textual data preprocessing which involves several steps like-:
- Merging all important columns into one single column.
- Lower Casing
- Removing Punctuations
- Removing Stopwords
- Text Normalization (Stemming and Lematization)
- Text Vectorization (we used tfidf)
4. As there were many features after tfidf vectorisation, we applied dimensionality reduction technique, PCA where we were able to capture 95% of variance in 5000 components.

5. Then in clustering part, we used several clustering techniques, including silhouette score,elbow visualiser, k-means clustering, dendrogram, and agglomerative clustering.

After analyzing the results of our clustering analysis, we determined that 10 clusters was the optimal number of clusters

6. We also created different word plots to visualise the distribution of genres and words over different clusters.

7. Finally we created recommender system using cosine similarity on our tfidf matrix.

8. Then, we checked the working of our recommender system by passing different movie names to it, and it performed well on them.

# Additional Notes

- Incorporating external datasets, such as IMDB ratings and Rotten Tomatoes, with this dataset can yield numerous intriguing discoveries.

- More time could be given on clustering analysis to try out different clustering algorithms like DBSCAN.

- More time could be given in improving the recommender system and building a working app on this recommender system.

#
