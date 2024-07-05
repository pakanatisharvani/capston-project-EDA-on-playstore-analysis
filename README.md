# capstone-project-EDA-on-playstore-analysis

This study does a thorough analysis of Play Store app data using Python, with an emphasis on identifying key parameters driving app engagement and success. Using Python libraries such as NumPy, Pandas, Seaborn, and Matplotlib for data manipulation and visualisation, the goal is to deliver actionable insights to improve app performance in the Android market.

The project is based on two datasets: the Play Store Dataset and the User Reviews Dataset, which contain a variety of app information. The Play Store dataset, which contained 10,841 rows and 13 columns, presented a significant problem with 483 occurrences of duplicated records. This redundancy not only compromises the dataset's integrity, but it also distorts analytical results, potentially leading to skewed insights and incorrect conclusions.

Furthermore, the high prevalence of missing values in crucial columns adds to the dataset's complexity. Notably, the 'Rating' column, which is critical for measuring app quality, has 13.60% null values, creating ambiguity and preventing proper ratings. The 'Type,' 'Content Rating,' 'Current Ver,' and 'Android Ver' columns all have variable degrees of missing values, requiring diligent attention to build a thorough and valid dataset.

The User Reviews dataset, which has 64,295 rows and 5 columns, faces its own set of issues, including 33,616 occurrences of duplicated records. Duplicates cause duplication and may exaggerate the influence of specific evaluations, jeopardising the dataset's representativeness.

The data cleaning process becomes even more important when faced with the startling prevalence of missing values in the 'Translated_Review,' 'Sentiment,' 'Sentiment_Polarity,' and 'Sentiment_Subjectivity' columns. With null values ranging about 41.78%, a sizable chunk of the dataset is incomplete, necessitating smart processing to provide a coherent and useful result. This involves recognising non-numerical reviews, converting data kinds, resolving missing values, and removing duplicates. Normalisation, scaling, and outlier treatment help to refine datasets, allowing for valuable insights.

The Exploratory Data Analysis (EDA) phase reveals key insights that go beyond conventional statistical analysis. Visual representations, such as histograms, pie charts, bar charts, and reg plots, help to comprehend user moods, app ratings, genre preferences, and the long-term impact of upgrades.This deeper exploration forms the bedrock for strategic decision-making in app development and optimization.

 **Distribution of Sentiment Polarity: **

The histogram shows a clear peak towards the positive side, indicating most apps have predominantly positive sentiment amongst users. This suggests most apps are well-received and appreciated by users.
