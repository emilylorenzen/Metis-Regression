Linear Regression Project Proposal
# Predicting winning bids on homes recently sold in Portland, OR
## **Question/Need**
More often than not, the listed price for real estate is not the selling price. The discrepancy in listed and selling price is particularly highlighted by the recent real estate market in Portland, OR. Due to low supply and high demand, ~60% of homes sold in April 2021 were sold at a price higher than listed. A potential buyer must guess what is the losest bid they can submit in order to win. A linear regression model can assist buyers and their real estate agents in deciding the optimal bid price. 

## **Data**
Redfin.com maintains data on recently sold homes over the past year. To address the question described above, I will scrape data for home sales in Portland, OR over the past month. In the case there is not enough data, I will expand my analysis to the past three months. 

A single unit of data will be a sold home, represented by the full address of the home. I will scrape the following features - zipcode, selling price, listing price, views, likes, number of bedrooms and bathrooms, parking type, school grade, size, lot size, yard, view, fireplace, AC, year built, year remodeled, and property type.

The y-target will be the percent difference between the listing price and selling price. 

I predict that properties that sold for the highest percent above listing will be localized to inner residential areas of Portland, near good schools, and will have higher listing prices. I think I'm also going to see a lot of multicolinearity between the features with "luxury" features (fireplace, view, AC, garage), size and number of bedrooms correlated with price.

## **Tools**
Data will be scraped and parsed using requests and BeautifulSoup. When a browser is required, Selenium will be used. Scraped data will be formatted into a list of dictionaries and then loaded into a pandas dataframe for analysis. For data visualization I will use matplotlib and seaborn. I will use sklearn to perform linear regression and evaluate the model. 

## **Minimal Viable Problem**
For the MVP I will initially use 3 features to perform a basic linear regression and evaluate it. The features I will initially examine will be price, days on market, home type, 