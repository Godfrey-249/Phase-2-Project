# Phase-2-Project
This is the Phase 2 project By Data Science Moringa Group 2

## PROJECT OVERVIEW.

### 1. BUSINESS UNDERSTANDING.
#### BUSINESS PROBLEM.
Your company now sees all the big companies creating original video content and they want to get in on the fun. They have decided to create a new movie studio, but they don’t know anything about creating movies. You are charged with exploring what types of films are currently doing the best at the box office. You must then translate those findings into actionable insights that the head of your company's new movie studio can use to help decide what type of films to create.

#### OBJECTIVES.  
1. Understand runtime trends considering ratings. 
2. Potential movie directors that have the highest audience ratings.
3. Studios with the highest returns.
4. Production budget that yields the most profit return and evaluate the Impact of budget on success.
5. Compare the worldwide and domestic market profits.
6. Understand Genre Performance in terms of ratings
7. Identify Profitable Films
8. Analyse Audience Sentiment and Engagement.
9. Find month of release with the highest profits.

### 2. DATA UNDERSTANDING.
#### Sources of Data.
The Data used was from various locations, and the following data was used;
- rt_movies.tsv
- bom.movies.csv
- rt_reviews.csv
- im.db
- tn_movies.csv.


### 3. DATA PREPARATION.
- Dealing with blank cells.
- Dropping unnecessary columns.
- Changing Data Types.
- Merging Data.

### 4. DATA ANALYSIS AND VISUALIZATION
![Image](https://github.com/user-attachments/assets/11bbb850-276e-4c10-aa47-8e54ec8b276b)

- From the analysis above, movies that focused on the foreign market recorded higher profits than those that focused on the domestic market. We can therefore recommend the studio to focus more on the foreign markets.

![Image](https://github.com/user-attachments/assets/8f97ebc1-2713-4b40-9813-806dc7abb786)

- May, June and July have fewer movies being released but have relatively higher revenue income and would therefore recommend the company to consider creating a film during these months due to low traffic from newer movies but still maximixe on the profits
- Movies released in November and December have higher revenue generation compared to other months. i would therefore recommend the company to consider releasing their movies during these months.

![Image](https://github.com/user-attachments/assets/c8857128-d114-488f-ac3e-4981cfac8e3d)

- The attributes used to evaluate movie perfomance and ratings include the run time in minutes and the movie popularity using movie count.

- It is advisable for the movie studio to highly consider venturing into movies with shorter run time as the longer the periods the lower the ratings as shown above.

- It is also advisable for the movie studio to venture into genres such as Dramas and Documentaries as from the analysis above, these genres earned the spot as the most popular genres over others such as Adventures, Biographies and Crime movies.

### TABLEAU DASHBOARD 

<img width="1470" alt="Screenshot 2025-04-30 at 10 42 21" src="https://github.com/user-attachments/assets/63fe5ed5-6fe8-496b-a82c-9f4621a1b70c" />


[Tableau dashboard link](https://public.tableau.com/app/profile/faith.kamande/viz/GroupTableauProject_17459957815580/Dashboard)
### STATISTICAL DATA INTERGRATION

1. Testing long and short movie ratings
- Null hypothesis - There is less difference between long and short movie ratings.
- Alternate hypothesis - There is a difference between long and short movies.

After using `ttest_ind` test rejected the null hypothses since `p-value = 2.0779210380104707e-44` is less than 0.05.

Therefore there is a significant difference in audience ratings between short and long movies, suggesting that movie runtime has an influence on how audiences rate films.

2. Testing the difference in Foreign and Domestic Revenue.
- Null hypothesis - There is no significant difference in forign and domestic revenue
- Alternate hypothesis -There is significant difference in foreign and domestic revenue

After usinig the `mannwhitneyu` test we rejected the null hypothesis since `p-value = 0.0000` was less than 0.05.

Therefore there is a significant difference in Profits between gross == True and gross == False groups.

### RECOMMENDATIONS

1. Genres and runtimes based on ratings - 

Profitable films are often franchise-based, family-friendly, superhero-related, and supported by strong international appeal.We can therefore recommend considering the franchise-based, family-friendly and superhero-related movies/Films.

It is also advisable for the movie studio to venture into genres such as Dramas and Documentaries as from the analysis above, these genres earned the spot as the most popular genres over others such as Adventures, Biographies and Crime movies.


2. Preferable markets based on domestic and foreign returns -

From the analysis above, movies that focused on the foreign market recorded higher profits than those that focused on the domestic market. We can therefore recommend the studio to focus more on the foreign markets.

3. Movie production features: directors, budgets and release dates -

From the analysis, we came to a conclusion that the movies with the lowest budgets recorded higher returns.This therefore means that for the studio to gain high returns it is not necessary for them to spend a lot in production as less budgets produce higher returns

It is advisable for the movie studio to highly consider venturing into movies with shorter run time as the longer the periods the lower the ratings as shown above.

From the analysis we can conclude that Robert Tutak,Taylor Morden and MIchiel Brongers are the top rated Directors in the film indurstry. We can therefore reccomend patnering with them in various projects.

May, June and July have fewer movies being released but have relatively higher revenue income and would therefore recommend the company to consider creating a film during these months due to low traffic from newer movies but still maximixe on the profits

Movies released in November and December have higher revenue generation compared to other months. I would therefore recommend the company to consider releasing their movies during these months.




