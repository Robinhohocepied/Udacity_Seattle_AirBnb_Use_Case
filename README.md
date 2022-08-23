# [Pricing Analytics for a Home Sharing Platform -----> Blog ](https://medium.com/@robinhocepied/how-to-set-your-next-airbnb-listing-price-smartly-589b49f97cf1)
#### [_Udacity - Data Scientist Nanodegree:_](https://www.udacity.com/school-of-data-science) _Project: Writing a Data Scientist Blog Post_
## Table of Contents

1. [Project Overview](#project)
2. [Requirements](#requirements)
3. [Project Movitivation](#motivation)
4. [Key Files](#files)
5. [Summary of Findings](#summary)
6. [Acknowledgements](#acknowledgements)

### 1. Project Overview<a id="project"></a>
This project has three parts to demonstrate the ability to analyze, visualize and model data acoridng to business-driven questions.

- Part 1: **Exploratory and Explanatory:** Visualization\
    I used Python visualization libraries to systematically explore a dataset, starting from plots of single variables and building up to plots of multiple variables
    
- Part 2: **Modelization:** Prediction\
    I ran 10 models to predict the prices of the Airbnb listings based on a set of cleaned features
    
- Part 3: **Communicate Findings:**[ Blog in Medium and Repo in Github](https://medium.com/@robinhocepied/how-to-set-your-next-airbnb-listing-price-smartly-589b49f97cf1) 
    I documented the results in a Github repo and gathered all the main insights in a non-technical blog article in Medium

### 2. Requirements<a id="requirements"></a>
This project was created in a Jupyter Notebook made available via Anaconda and written in python. 
The following versions of languages and libraries were used in creating this project:
- python==2.7.18
- matplotlib==3.5.1
- numpy==1.22.0
- pandas==1.3.5
- seaborn==0.11.2

### 3. Project Motivation<a id="motivation"></a>

#### Scenario:
As a young professional looking to boost his "Data" career progression I have personally made the choice to move to Seattle next year. This decision was made after some thorough research, where I came to realize Seattle matched every aspect of the lifestyle I wanted to have as a young professional seeking to have an impact in the tech world while having the time to explore the beauty of nature surrounding the city.

Being a couple months away from the move I decided I would spend 2 weekends in Seattle to explore areas where I would feel "at home" and compare neighbourhoods/regions based on a set of criteria that would help me derive the best decision further in time.

Having a bit of free-time, I pushed myself to enroll in a personal challenge: Explore Airbnb Listings Data to create an in-depth understanding of when, where, and what makes the difference in pricing when it comes to rent a property in Airbnb.com. This came right in time, as I always back-up my personal moves/choices wiht some prior rational investigation. Tu put it in another way, moving to Seattle would mean a tighter management of my expenses, this meant, sacrificing some of my personal wishes, such as settling in a artistic neighbourhood, logically the more expensive ones, to find the adequate balance in terms of spending and finding the best location possible.

While reflecting on this exploration, questions started bumping into my mind.. What if I could rent a 2-bedroom place and start renting it on Airbnb, how big of a risk would this be? How are properties priced and how are prices spread out based on location? Are there any high and low seasons in the renting ecosystem? What could influence the pricing?

These helped somehow frame the analysis and write some important key guidelines to keep in mind while making progress.

As per Udacity, after completing this project, I was able to:
- Supplement statistics with visualizations to build an understanding of the data.
- Choose appropriate plots, limits, transformations, and aesthetics to explore a dataset, which allowed me to understand distributions of variables and relationships between features.
- Use design principles to create effective visualizations for communicating findings to an audience.

### 4. Key Files<a id="files"></a>
- `calendar.csv`
- `listings.csv`
- `reviews.csv`
- `Seattle_Airbnb_Exploration_Modelling.ipynb`

    
### 5. Summary of Findings<a id="summary"></a>

- There is a strong Seasonality pattern in the average prices evolution over time. July and August have the highest average prices, indicating weather and rainfall % play an important role in the seasonal offering. Drilling down to the weekly view, as we would expect, Fridays and Saturdays are the most "profitable" days from a lender's perspective.

- Neighbourhood wise, most of the listings are located in the central area of Seattle between Elliot Bay and Lake Washington. The listings with the highest average prices stand close to the central west part, bordering the Elliot Bay and the Puget Sound. West tends to be more expensive than the East, while the South part is less expensive than the North. The prices range from 80 to 180 dollars a night.

- If we look at the Types of Properties, listings are mostly entire homes or appartments, representing 2/3 of the listings. These are 2 to 3 times more expensive than its counterparts (Private and Shared Room) standing at 156 dollars.

- Houses and Apartments account for 90% of the Property Types (16 Types) in the Airbnb listings, with no major difference in the number of listings. All Property types display similar Average Prices, ranging from 95 to 150 dollars (3 exceptions), the most interesting one is the Boat type (first in the list) which seems to be a luxury niche with an Average Price at almost 300 dollars a night.

- Almost half of the Airbnb listings can Accomodate 2 people. Directly followed by 4 and 3 people acounting in total for ~+30% of the listings. This means ~+70% of the Airbnb listings can accomodate not more than a 4-people household. The relationship between the number of accomodates is quite linear in terms of prices, the highest the average price the highest the number of people we can accomodate, with one or two exceptions (however not significant in number of listings)

- For the Prediction of the Listing Price, the Linear Regression offers us the best results if we bear in mind interpretability and results of the 10 models. We get respectively an R-Square of 0.546 and 0.543 for the training and test set. In terms of Interpretability, the feature "Room type/Entire Home/Appartment" displays the highest coefficient (27.41), followed by Bedrooms (20.13) and Cleaning Fee (16.87). To conclude, we are not too enthusiastic about these results. If further improvements were to be done, we could eventually tweak the analysis by optimizing and/or improve the features and hyper parameters embedded in this model to slightly boost the performance.




### 6. Acknowledgements<a id="acknowledgements"></a>
This project was completed as part of the Udacity's [Data Science Nanodegree](https://www.udacity.com/school-of-data-science).
