# Premier League Transfer Spending vs Club Finances 

## What this is about
I wanted to find out whether clubs that earn more money actually spend more on transfers. This came from watching how different Premier League clubs spend compared to their size - some clubs with huge revenues seem cautious in the transfer market while others spend way beyond what you'd expect, Tottenham just finished above relegation two years running while still spending over £237 million halfway through the summer 2026 transfer window. I wanted to see if there was an actual pattern in the data or if it's more random than people think. 
I also had a look at which positions clubs tend to spend the most on.
## The question
Does a club's revenue actually predict how much they spend on transfers? 
Where does most of the transfer money go by position?

## The data
I used two datasets from Kaggle (Global Football Transfer Market 2010-2026, Sergey Nefedov):
- transfers_history.csv - roughly 15,000 transfers including the player, position, fee and clubs involved.
- club_financials.csv - revenue, wages and net transfer spend for clubs by season.

## Tools
Python (pandas and matplotlib) for cleaning the data and making charts. SQL (via DuckDB) for the grouping and aggregation queries.

## What I found
Revenue and transfer spend aren't that strongly linked. The correlation came out at 0.34 so richer clubs do tend to spend a bit more but not as dramatic as many might think. 

The Saudi clubs stood out as spending a much bigger share of their revenue on transfers. Al-Nassr signing Cristiano Ronaldo and Al-Hilal signing Neymar are good examples - moves like these pushed their spending to over half their total revenue in some seasons. That's a far bigger proportion than clubs like Man City or Man United spend, even though City and United earn a lot more money overall.

Clubs like Benfica and Ajax who barely spend anything net - some seasons they actually make more money from transfers than they spend, which is very rare for clubs, particulaly those who are best in their respective leagues. The data does back up their reputation as clubs that focus on developing young players and selling them on for a profit rather than buying expensive ones. 

Centre-backs and central midfielders get bought the most overall in terms of total money spent, which makes sense given how many transfers happen in those positions. But right-backs actually have the highest average fee per transfer. 

## How to run it
Open the notebook in Colab, upload the two CSV files when it prompts you, and run all the cells.

## Author
Harry Dawes


