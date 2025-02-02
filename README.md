# Project Brief

Authors: Kenny Nguyen, Peter Miyoshi, Ryan McGhee

This is our final project for our INFO 201 course at the University of Washington. We decided on a domain of interest (gaming) and extracted meaningful insights from datasets pertaining to it, namely through visualizations and data science fundamentals.

Our end product was a collaborative data-driven website deployed in Shiny and coded in R. It can be found [here](https://ken-ux.shinyapps.io/final-project-ken-ux/).

Below is a write-up that details our process through questions and answers.

# Part 1: Domain of Interest
The domain we're interested in is **gaming, particularly video games**.

- **Why are you interested in this field/domain?**

We are interested in gaming as a domain because it explores a realm of technology that is becomingly increasingly popular and more complex with the advancement of gaming platforms, companies, and technological innovations (VR, mobile, etc.) Our group has played different video games throughout our lives and it would be interesting to see how our perspective of its evolution parallels trends we uncover.

- **What other examples of data driven project have you found related to this domain (share at least 3)?**

1. [A Survey of ‘Game’ Portability](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.303.2716&rep=rep1&type=pdf) by Ahmed BinSubaih, Steve Maddock, and Daniela Romano is a survey detailing different gaming elements required for portability of a video game between gaming engines. They coalesce data from 40 different game engines to highlight aspects of specific gaming elements which allow easier portability of games between engines. (_Think about how a Nintendo DS game can be ported as a mobile game._)

2. [Predicting video game hits with Machine Learning](https://towardsdatascience.com/predicting-hit-video-games-with-ml-1341bd9b86b0) by Ignacio Chavarria is an article about how extrapolated data from popular video games—denoted by their unit sales—such as their genre or platform can be used to predict games in development that may become a "hit".

3. [Improving video game project scope decisions with data: An analysis of achievements and game completion rates](https://www.sciencedirect.com/science/article/abs/pii/S1875952118300181) by Eric Bailey and Kazunori Miyata is a research article which takes open-source data from Steam, a digital distributor of games, and finds factors such as ratings or price that correlate with users who actually complete their game by unlocking all achievements.

- **What data-driven questions do you hope to answer about this domain (share at least 3)?**

We hope to answer these types of questions:

1. How has the diversity of game genres changed over time?
    - This question can be answered by looking at the amount of game genres that are present in current years versus older ones.
2. What game genres are most/least popular with certain age groups or over time? (_Other demographic factors can include gender, country, race, etc._)
    - This question can be answered by comparing the relative popularity of game genres with defined age groups.
3. How has use of certain gaming platforms evolved over time? (_As a follow-up, has the advent of mobile devices and gaming systems affected popular use of those platforms?_)
    - This question can be answered through the most used gaming platforms for the most popular games.
4. How has the price of console games changed over time?
    - This question can be answered by tracking the average price for a game (which can also be categorized by the console it is on) during its release year.
5. How has the ratio of women to men who play video games changed over time?
    - This question can be answered by demographic data which shows the frequency of women versus men who play games.

# Part 2: Finding Data

Dataset 1
---
For: _data/games-features.csv_

- **Where did you download the data (e.g., a web URL)?**

https://data.world/craigkelly/steam-game-data

- **How was the data collected or generated? Make sure to explain who collected the data (not necessarily the same people that host the data), and who or what the data is about?**

The data was collected through publicly available Steam API's and steamspy.com, a website that also uses Steam API to note sales of game titles.

- **How many observations (rows) are in your data?**

13,357.

- **How many features (columns) are in the data?**

78.

- **What questions (from above) can be answered using the data in this dataset?**

The dataset can help answer the first and third questions about game genres changing over time and the rise of certain platforms for gaming. These are most readily answered by the release date and platform columns.

Dataset 2
---
For: _data/vgsales-12-4-19_

- **Where did you download the data (e.g., a web URL)?**

https://www.kaggle.com/ashaheedq/video-games-sales-2019

- **How was the data collected or generated? Make sure to explain who collected the data (not necessarily the same people that host the data), and who or what the data is about?**

The data was generated through a scrape of vgchartz.com.

- **How many observations (rows) are in your data?**

37,102.

- **How many features (columns) are in the data?**

16.

- **What questions (from above) can be answered using the data in this dataset?**

This data set can help answer questions regarding change in genre popularity over time, and perhaps may help answer questions regarding popularity of different platforms for gaming. These questions are answered through the genre, year, platform, and global_sales columns

Dataset 3
---
For: _data/game_info.csv_

- **Where did you download the data (e.g., a web URL)?**

https://www.kaggle.com/jummyegg/rawg-game-dataset/data

- **How was the data collected or generated? Make sure to explain who collected the data (not necessarily the same people that host the data), and who or what the data is about?**

The data was collected from RAWG API and is a game database for discovering new games on over 50 platforms.

- **How many observations (rows) are in your data?**

345,667.

- **How many features (columns) are in the data?**

27.

- **What questions (from above) can be answered using the data in this dataset?**

This data set can help provide insight for the diversification of games over time, especially over multiple platforms, and relative popularity of games/genres. An analysis of the genre, platforms, and added_status_owned columns can answer the questions.
