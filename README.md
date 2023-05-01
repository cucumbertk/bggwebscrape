# bggwebscrap
This is my senior research about "How boardgame features affect thier rating score". 
Files 01 - 06 are run in google colaboratory, 07- 09 are run in Jupyter Notebook.

Starting from file 01, the code show us how to scrape the BGG web from scratch by using BeautifulSoup and Selenium. 
We will get top 2000 game ids, names, urls and ranks from the ranking page, then using this data to scrape individual info from each game page. (scraped on 11/01/2023)
Save the file that contained all stats we need as 'bgg_scrape.csv'


file 02 : changing Categories and Mechanics of the games from list to dummy variables.

file 03 : cleaning the text in desccriptions of the games into readable form.

file 04-05 : creating words feature by CountVectorizer, then filter them by Glove dictionary.

fil 06 : selecting words feature by frequency.

file 07 : Using Lasso Regression to find coefficient of the Categories / Mechanics / Stats / Words feature.
          Using XGBoost to find feature importance of the Categories / Mechanics / Stats / Words feature.
          Using Partial Dependence Plot to find effects of the features in XGBoost.
          
file 08 : Compare R-Squared of Lasso model and XGBoost model. Choose the better one
