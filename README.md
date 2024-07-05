# capstone-project-EDA-on-playstore-analysis

This study does a thorough analysis of Play Store app data using Python, with an emphasis on identifying key parameters driving app engagement and success. Using Python libraries such as NumPy, Pandas, Seaborn, and Matplotlib for data manipulation and visualisation, the goal is to deliver actionable insights to improve app performance in the Android market.

The project is based on two datasets: the Play Store Dataset and the User Reviews Dataset, which contain a variety of app information. The Play Store dataset, which contained 10,841 rows and 13 columns, presented a significant problem with 483 occurrences of duplicated records. This redundancy not only compromises the dataset's integrity, but it also distorts analytical results, potentially leading to skewed insights and incorrect conclusions.

Furthermore, the high prevalence of missing values in crucial columns adds to the dataset's complexity. Notably, the 'Rating' column, which is critical for measuring app quality, has 13.60% null values, creating ambiguity and preventing proper ratings. The 'Type,' 'Content Rating,' 'Current Ver,' and 'Android Ver' columns all have variable degrees of missing values, requiring diligent attention to build a thorough and valid dataset.

The User Reviews dataset, which has 64,295 rows and 5 columns, faces its own set of issues, including 33,616 occurrences of duplicated records. Duplicates cause duplication and may exaggerate the influence of specific evaluations, jeopardising the dataset's representativeness.

The data cleaning process becomes even more important when faced with the startling prevalence of missing values in the 'Translated_Review,' 'Sentiment,' 'Sentiment_Polarity,' and 'Sentiment_Subjectivity' columns. With null values ranging about 41.78%, a sizable chunk of the dataset is incomplete, necessitating smart processing to provide a coherent and useful result. This involves recognising non-numerical reviews, converting data kinds, resolving missing values, and removing duplicates. Normalisation, scaling, and outlier treatment help to refine datasets, allowing for valuable insights.

The Exploratory Data Analysis (EDA) phase reveals key insights that go beyond conventional statistical analysis. Visual representations, such as histograms, pie charts, bar charts, and reg plots, help to comprehend user moods, app ratings, genre preferences, and the long-term impact of upgrades.This deeper exploration forms the bedrock for strategic decision-making in app development and optimization.

**Distribution of Sentiment Polarity:**

The histogram shows a clear peak towards the positive side, indicating most apps have predominantly positive sentiment amongst users. This suggests most apps are well-received and appreciated by users.

**Distribution of App Ratings:**

The histogram shows that majority of users are satisfied with the apps, as evidenced by the high concentration of positive ratings.

**Distribution of App Types:**

The larger slice of the pie chart represents the free apps, with 92.3% of the total. The smaller slice representing paid apps, with 7.7% of the total. This indicates that the vast majority of apps on the Google Play Store are free to download and use.

**Top 10 Genres by Installs:**

**Tools** apps are the most popular genre. This is likely due to the increasing reliance on smartphones and tablets for work and productivity.

**Action** apps are the second most popular genre. Action games are typically fast-paced and exciting, and they appeal to a wide range of users.

**Photography** apps are the third most popular genre. This is likely due to the increasing popularity of smartphone photography.

**Entertainment** apps are the fourth most popular genre. Entertainment apps include various streaming services as well as social media apps.

**Communication** apps are the fifth most popular genre. Communication apps include messaging apps and video conferencing apps.

**Content Ratings by Installs:**

The categories **Everyone and Teen** stand out with the highest number of installs, indicating preferences for apps suitable for all ages or users aged 13 and above. These categories encompass apps with minimal or mild content, including educational, entertainment, or social apps.

The **Everyone 10+** category follows with the third-highest installs, suggesting a preference for apps suitable for users aged 10 and above. Such apps may contain more moderate content, such as fantasy or science fiction.

The **Mature 17+** and **Adults only 18+** categories exhibit significantly fewer installs. This implies a limited preference for apps tailored to users aged 17 or older or 18 and older, which may feature intense or graphic content like violence, sexual content, drug use, or gambling.

The **Unrated** category records the fewest installs, suggesting minimal interest in apps lacking official ratings. These apps may have unknown or variable content, potentially unsuitable for some users.

**Size Groups by Installs:**

The size group with the most installs is the below 20 group, followed by the 20-40 group, followed by the 40-60 group, then the 60-80 group, and finally the 80-100 group.
The size group with the least installs is the 80-100 group, which has less than a quarter of the installs of the below 20 group. This suggests that the users prefer smaller apps over larger apps. This could indicate that the users have limited storage space on their devices, or that they are more selective about the apps they download and install.

**Distribution of Ratings by Update Year:**

The average rating has shown an improvement, rising from approximately 3.5 in 2010 to nearly 4.5 in 2018. This indicates a general trend of increasing satisfaction among users with the product over the years.

The red line shows that the overall trend is towards increasing ratings. This is a positive sign for the product.

The slope of the red line is positive, which indicates that the relationship between rating and update year is positive. This means that ratings tend to increase as the update year increases.

**Top 10 Categories by Average Revenue:**

The top 3 revenue-generating categories, namely **Lifestyle, Finance, and Weather**, indicate a willingness among users to invest in products and services associated with their personal lives and finances.

The following 3 categories in revenue ranking **Game, Photography, and Family** are all linked to entertainment and leisure, signaling an increasing trend of expenditure on experiences meant for enjoyment and shared moments.

Contrastingly, the **Sports** category records the lowest average revenue, implying a lack of popularity among users. Similarly, the **Education** category follows closely with the second lowest average revenue, highlighting lower profitability.

The **Personalization** category secures the fourth-lowest average revenue, suggesting a relatively lower level of user interest. Lastly, the **Medical** category ranks third lowest in average revenue, indicating potential challenges in terms of convenience or security for apps within this category.

**Revenue and Android Version of the Top 8 Paid Apps:**

The apps with Android versions 4.0 and above dominate the higher revenue ranks, suggesting a correlation between app compatibility with newer Android versions and revenue generation.

Among the top 8 high revenue apps, six are designed for Android versions 4.0 and above. The exceptions are "Grand Theft Auto: San Andreas" (Android 3.0 and up) and "DraStic DS Emulator" (Android 2.3 and up), both of which are on the lower end of the revenue spectrum.

**Sentiment counts across categories:**

The stacked bar chart reveals a complex interplay of positive and negative sentiments across different categories. While people express positive sentiments towards categories like games, family, health and fitness, travel and local, and dating, there is also a notable presence of negative sentiment associated with most of these same categories.

**Update counts and the distribution of sentiment counts over time:**

There is a general trend of increasing positive sentiments over time. This suggests that people are generally becoming more satisfied with the updates they are receiving.

The number of updates is increasing over time. This suggests that the developers are releasing new updates more frequently.

The number of negative sentiments is relatively stable. This suggests that people are generally not very unhappy with the updates they are receiving.

**Sentiment Polarity by Rating and Installs:**

**Apps with higher ratings tend to have higher average sentiment polarity:** This correlation is logical, as users are more inclined to leave positive reviews for apps they enjoy using.

**Niche Apps with High Sentiment Polarity:** Some apps exhibit high average sentiment polarity despite having relatively low install counts. This indicates the presence of niche apps that are deeply cherished by their user base, even though they may not enjoy widespread popularity.

**Popularity vs. Sentiment Polarity Discrepancy:** The large bubbles representing the most installed apps generally show lower average sentiment polarity. This implies that widespread popularity doesn't consistently align with positive user sentiment.

**Relationship between Sentiment Subjectivity and Sentiment Polarity:**

The scatter plot of Sentiment Polarity and Sentiment Subjectivity shows a moderate positive correlation between the two variables. This means that, in general, as sentiment polarity increases, sentiment subjectivity tends to increase as well. However, the relationship is not very strong. This suggests that there is a tendency for people to express their opinions more strongly when they are feeling positive than when they are feeling negative.

**Correlation among Rating, Reviews, Installs, Price, Sentiment_Polarity, and Sentiment_Subjectivity:**

Rating has a moderate positive correlation with Reviews, Installs, and Sentiment_Polarity. This means that apps with higher ratings tend to have more reviews, more installs, and more positive sentiment in their reviews. Rating has a weak negative correlation with Price. This means that apps with higher ratings tend to be slightly cheaper.

Reviews has a strong positive correlation with Installs. This means that apps with more reviews tend to have more installs. Reviews has a weak negative correlation with Price. This means that apps with more reviews tend to be slightly cheaper.

Installs has a weak negative correlation with Price. This means that apps with more installs tend to be slightly cheaper.

Sentiment_Polarity has a moderate positive correlation with Sentiment_Subjectivity. This means that apps with more positive sentiment in their reviews tend to have slightly more subjective reviews.

**Rating and Installs:** There is a positive correlation between rating and installs, meaning that apps with higher ratings tend to have more installs. This is likely because users are more likely to install apps that have been positively reviewed by other users.

**Rating and Reviews:** There is also a positive correlation between rating and reviews, meaning that apps with higher ratings tend to have more reviews. This is likely because users are more likely to write reviews for apps that they enjoy using.

**Rating and Price:** There is a weak negative correlation between rating and price, meaning that apps with higher ratings tend to be slightly cheaper. This is likely because developers of high-quality apps are able to charge lower prices due to the high demand for their apps.

**Installs and Reviews:** There is a strong positive correlation between installs and reviews, meaning that apps with more installs tend to have more reviews. This is likely because users are more likely to write reviews for apps that they have used extensively.

**Installs and Price:** There is a weak negative correlation between installs and price, meaning that apps with more installs tend to be slightly cheaper. This is likely because developers of popular apps are able to charge lower prices due to the high volume of installs.

**Actionable Recommendations:**

**Strategic Development in Popular Genres:** Acknowledge the popularity of certain genres, such as Tools, Action, Photography, and Entertainment. Consider investing in or refining apps within these genres to align with user preferences and maximize engagement.

**Emphasize Free Apps:** Free apps overwhelmingly dominate the market, indicating the significance of providing an engaging free version to attract users. Given that the majority of apps are free, focus on monetization strategies that complement the free model, such as in-app purchases, ads, or premium features.

**Optimize App Size:** Recognize the preference for smaller apps, as indicated by the popularity of the below 20 and 20-40 MB size groups. Ensure that new app developments and updates prioritize efficiency and minimal storage requirements to align with user preferences for smaller-sized apps.

**Tailor Content Ratings:** Understand the user preference for Everyone and Teen categories and ensure new apps align with these preferences. Be mindful of the limited interest in Mature and Adults-only categories, adjusting content accordingly.

**Strategic Revenue Generation:** Consider app development or improvements in categories that generate higher revenue, such as Lifestyle, Finance, and Weather. Evaluate user preferences within lower-revenue categories to identify opportunities for enhancement.

**Compatibility with Latest Android Versions:** Given the correlation between higher revenue and compatibility with newer Android versions, prioritize app development and updates for the latest versions of the Android operating system.

**User Engagement in Popular Categories:** Recognize the positive sentiments associated with popular categories like Games, Family, Health and Fitness, Travel and Local, and Dating. Strategically engage users through marketing, promotions, and feature enhancements in these categories.

**Continuous Improvement:** Monitor the progression of update counts and user sentiments over time. Respond to user feedback with timely updates to demonstrate a commitment to app improvement.

**Focus on Positive User Sentiment:** Identify the characteristics of apps with consistently positive sentiment and leverage those aspects in future app development. Encourage and amplify positive user experiences through marketing and feature enhancements.

**Address Negative Feedback:** Investigate apps with negative sentiment to pinpoint specific issues causing dissatisfaction. Prioritize improvements in areas highlighted by negative sentiment to enhance user satisfaction and overall app performance.

**Conclusion:**

This project has successfully analyzed the Play Store app dataset using Python, uncovering valuable insights into key factors for app engagement and success. The data visualizations and interpretations provide a comprehensive understanding of user sentiment, app ratings, genre preferences, content suitability, and the impact of updates.

Based on these insights, I have crafted actionable recommendations for the client to optimize app performance and achieve their business objectives. I advise them to focus on fostering positive sentiment, addressing user concerns promptly, catering to user preferences like smaller apps and frequent updates, targeting specific genres and content ratings strategically, and building loyal followings in niche markets.

By embracing a data-driven approach and continuously adapting to user preferences, the client can ensure long-term success in the competitive Android app market.

