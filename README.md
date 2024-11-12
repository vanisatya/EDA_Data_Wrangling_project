Exploratory Data Analysis and Visualization of NYC Airbnb Listings
Objective: The project aims to perform Exploratory Data Analysis (EDA) on the Airbnb NYC 2019 dataset to gain insights into listing trends, pricing patterns, and neighborhood distribution. The analysis focuses on data wrangling, handling missing values, and creating meaningful visualizations to present findings about the Airbnb market in New York City.

1. Data Exploration:
•	Dataset Overview:
  The dataset contains 48,895 Airbnb listings with features such as name, host_id, neighbourhood_group, room_type, price, number_of_reviews, availability_365, and more.
	The primary goal is to understand how location, room type, and pricing interact in different parts of NYC.
•	Initial Insights:
	Neighbourhood groups: Listings are primarily distributed across five major boroughs: Manhattan, Brooklyn, Queens, Bronx, and Staten Island.
	Room types: The listings are categorized into different types, including Entire home/apt, Private room, Shared room, and Hotel room.
	Price distribution: The prices vary significantly, with certain neighborhoods having much higher prices than others.
•	Data types: Numeric (price, number_of_reviews, availability_365), categorical (neighbourhood_group, room_type), text (name, host_name).

2. Data Wrangling:
•	Missing Values:
	Columns like name and host_name have missing values, which are not crucial for analysis, so they are ignored.
	Other missing values, such as those in reviews_per_month, are handled by filling with 0, assuming that no reviews were given.
	Outliers in price: Listings with unusually high prices (above $1,000) are considered outliers and either capped or removed for a more reasonable analysis.

3. Data Visualization:
•	Distribution of Listings by Borough:
Created a bar chart to show the number of Airbnb listings in each borough (neighbourhood_group). Manhattan and Brooklyn had the most listings, with fewer in Staten Island and the Bronx.
Visualization: Bar plot (using seaborn).
•	Price Distribution by Neighbourhood Group:
Used a box plot to display the price distribution in different boroughs. Manhattan had the highest median price, while the Bronx had the lowest.
Visualization: Box plot (using seaborn).

4. Key Insights:
•	Neighbourhood Price Trends:
o	Manhattan had significantly higher prices compared to other boroughs, particularly in areas like Midtown and Downtown. Brooklyn also had expensive listings, but areas in Queens and the Bronx were much more affordable.
•	Room Type Pricing:
o	Entire apartments and homes are the most expensive, while private and shared rooms are more affordable. Manhattan dominates in the number of expensive listings.

5. Conclusions:
•	The Airbnb market in NYC is highly concentrated in Manhattan and Brooklyn, with prices being significantly higher in these boroughs.
•	There is a wide variation in prices depending on room type and location, making it essential to analyze both factors when studying rental markets.
•	Data wrangling techniques such as handling missing values, removing outliers, and normalizing price distributions were essential for accurate analysis and visualization.

Tools Used:
•	Data Wrangling: pandas (for data cleaning, transformation, and feature engineering)
•	Data Visualization: matplotlib, seaborn (for creating visual plots and statistical visualizations)
This project demonstrates the ability to perform EDA, clean and preprocess raw data, and generate actionable insights using Python-based data science tools.
