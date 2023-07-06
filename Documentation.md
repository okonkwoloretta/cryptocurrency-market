# Exploring the Bitcoin Cryptocurrency Market

The astonishing increase of Bitcoin market capitalization in 2017
![Picture2](https://github.com/okonkwoloretta/cryptocurrency-market-/assets/116097143/9a45b996-3d41-4d9c-a3a3-1f7bfe5d35df)


## Bitcoin and Cryptocurrencies: 

Since the [launch of Bitcoin in 2008](https://newfronttest.bitcoin.com/bitcoin.pdf), hundreds of similar projects based on blockchain technology have emerged. 
We call these cryptocurrencies (also coins or cryptos in the Internet slang). 
Some are extremely valuable nowadays, and others may have the potential to become extremely valuable in the future1. 
In fact, on the 6th of December of 2017, Bitcoin has a [market capitalization](https://en.wikipedia.org/wiki/Market_capitalization) above 
WARNING: The cryptocurrency market is exceptionally volatile2 and any money you put in might disappear into thin air. 
Cryptocurrencies mentioned here might be scams similar to [Ponzi Schemes](https://en.wikipedia.org/wiki/Ponzi_scheme) or have many other issues (overvaluation, technical, etc.). 
Please do not mistake this for investment advice.
Update on March 2020: Well, it turned out to be volatile indeed 
That said, let's get to business. I will start with a CSV I conveniently downloaded on [datacamp](https://app.datacamp.com/workspace/w/c86df0b5-c211-453d-9947-9b7938960da0/edit), 
they got theirs on the 6th of December of 2017 using the coinmarketcap API .
(NOTE: The public API went private in 2020 and is no longer available) 


## Aim
The aim of this project is to analyze the cryptocurrency market, with a focus on Bitcoin, using historical data from December 6, 2017. 
The project aims to gain insights into the market capitalization of cryptocurrencies, their volatility, and the distribution of large market capitalizations.
Additionally, the project provides recommendations based on the analysis and concludes with key takeaways.

## Data Cleaning Processes

- Reading the Dataset:
The provided CSV file, 'coinmarketcap_06122017.csv,' is read into a pandas DataFrame named dec6.

- Filtering and Counting:
Rows without a market capitalization (where market_cap_usd is greater than 0) are filtered out, resulting in a DataFrame named cap.
The count of values in the cap DataFrame is obtained using the count() function.

- Top 10 Market Capitalization: 
The first ten rows of the cap DataFrame are selected, and the 'id' column is set as the index in a DataFrame named cap10.
The 'market_cap_perc' column is calculated, representing the percentage of each cryptocurrency's market capitalization relative to the total market capitalization.

- Bar Plot of Market Capitalization:
A bar plot is created to visualize the top 10 cryptocurrencies by market capitalization using the cap10.market_cap_perc data.
The plot provides insights into the distribution of market capitalization among the top cryptocurrencies.

## Analysis

- Cryptocurrency Volatility: 
The 'percent_change_24h' and 'percent_change_7d' columns are extracted from the dataset, and a DataFrame named volatility is created.
The DataFrame is sorted by 'percent_change_24h' and 'percent_change_7d' to identify the top 10 losers and winners in terms of percentage changes.

- Large Market Capitalizations:
Cryptocurrencies with a market capitalization greater than $10 billion are selected and stored in the largecaps DataFrame.
This step allows for further analysis of the distribution of large market capitalizations.

- Counting Market Capitalizations: 
The number of cryptocurrencies in different market capitalization categories is calculated using the capcount function.
The categories include "biggish" (> $300 million), "micro" (between $50 million and $300 million), and "nano" (< $50 million). A bar plot is created to visualize the counts in each category.

## Insights
The top 10 cryptocurrencies by market capitalization are identified, providing insights into the dominance of certain cryptocurrencies in the market.
The volatility analysis reveals the cryptocurrencies with the highest percentage changes in a 24-hour and 7-day period, highlighting the potential risks and opportunities in the market.
The distribution of large market capitalizations showcases the concentration of value in cryptocurrencies with market capitalizations above $10 billion.
The categorization of market capitalizations provides a broader perspective on the size and distribution of cryptocurrencies in the market.

## Recommendations

Based on the analysis and insights obtained, the following recommendations can be made:

- Diversification: Investors should consider diversifying their cryptocurrency portfolios to mitigate risks associated with high volatility and concentration of market capitalization.

- Research and Due Diligence: Prior to investing, individuals should conduct thorough research and due diligence on individual cryptocurrencies, considering factors such as their technology, team, and market potential.

- Risk Management: Given the volatility of the cryptocurrency market, it is advisable to set clear management strategies, including setting stop-loss orders, 
diversifying investments across different asset classes, and allocating only a portion of the portfolio to cryptocurrencies.

## Conclusion

In conclusion, this project explored the Bitcoin cryptocurrency market using historical data from December 6, 2017. 
The analysis provided insights into market capitalization, volatility, and the distribution of large market capitalizations. 
The findings highlight the dynamic nature of the cryptocurrency market and the importance of careful research and risk management when investing in cryptocurrencies. 
It is crucial for individuals to stay updated on market trends and developments while making informed investment decisions.

Please note that the analysis and recommendations provided in this documentation are based on historical data from December 6, 2017, and may not reflect the current state of the cryptocurrency market. 
Cryptocurrency markets are highly volatile and subject to rapid changes. Therefore, it is essential to conduct further research and consult with financial professionals before making any investment decisions in the cryptocurrency market.

## Code
You can find the code used for this project on [Here]().
