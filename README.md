After analysing the datasets, we were able to find answers to some important and intriguing issues that would help businesses better understand their target markets and the items they are selling, thereby enabling them to expand and generate more revenue.

Instances & Observations we discovered after Analyzing the datasets:
Product level analysis
A total of 3683 different goods are available.
The top ten items by sales volume are 84077, 22197, 85099B, 84879, 85123A, 21212, 23084, 22492, and 22616. The item with the most sales volume, 21977, had nearly 24k units sold.

Additionally, more than 300 products have sold quantities of less than 10.

More than 400 products have only had less than five orders placed for them.

More than 400 products have only had less than five orders placed for them.

With a unit price of $49.95, 22833 is the tenth most expensive product overall, but it has the highest sales volume of 149 units.

The product with the lowest price, 16045, has the biggest sales volume among the 10 products with the lowest prices, 8900.

The top 10 products account for 8.28% of total sales.

'22423', '85123A', '85099B', '47566', 'POST', '84879', '23084', '22502', '79321', and '22086' are the top 10 items with the greatest sale value.

The highest transaction price for Stockcode 22423 was more than $130,000.

Less than $100 is the sale price of 23% of the products.

By creating a word cloud, it was discovered that items like light holders, water bottles, hanging hearts, lunch bags, dolls, red retrospots, metal signs, Christmas, and giant bags are commonly requested.

Customer level analysis
There are 4370 customers in total.

The top 3 clients, "17841," "14911," and "14096," have a combined total of more than 5000 transactions.

13.5% of clients have made fewer than 10 transactions.

15.8% of transactions had 10 to 20.

'14646', '18102', '17450', '14911', '12415', '14156', '17511', '16684', '13694', and '15311' are the top 10 consumers with the greatest purchase value.

'14646' and '18102' are the two customers with the greatest purchase values, each over $250,000.

90% of clients spend less than $3,500 on their overall purchases.

99% of people have less than $17,000.

Only 1% of customers make purchases totaling more than $17,000.

Geographical analysis
receiving orders from 37 various nations.
United Kingdom alone accounts for 89% of orders and has the greatest client base (81.50% of total sales).

Saudi Arabia and the Czech Republic have the fewest orders.

USA and Czech Republic have the greatest percentages of cancelled orders (62% and 20%, respectively), meaning that 62% of all orders have been cancelled.

DateTime analysis
The volume of daily transactions increased in the third quarter.

Closed on Saturday, don't get any orders on Saturday;

average sale on Sunday is low compared to other weekdays;

daily sale is high in second half compared to first half;

highest sale in November; sale is high in last four months compared to other months;

most orders are generated between 9am and 5pm; high number of orders in afternoon;

moderate number of orders in morning; and fewest numbers of orders in evening.

Conclusion on Customer segmentation (Clustering) :
Starting with the RFM model, we divided the client base into various groups according to their recentness, frequency, and monetary value. By calculating RFM_score and assigning RFM_group, we divided our clients into various categories.

RFM_group: RFM_group is the sum of the R, F, and M scores, with 444 being the best and 111 being the worst.
RFM_score: Where 12 is the greatest and best score and 3 is the lowest and worse score, RFM_score is the total of R, F, and M scores.
After that, we created three clusters using the Kmeans clustering algorithm, the elbow approach, and the silhouette method.

The 3258 clients in the first cluster label_0 have an average recency of 40, an average frequency of 103, and an average revenue of about 1950 dollars.

The second cluster label_1 has 1100 consumers with an average recency of 247 and a minimum recency of 138, meaning that these customers have not made any purchases in the previous four months. Additionally, the second cluster label_1 has only a low average frequency of 27 and a very low average value of roughly $472, compared to the first cluster_0.

The third cluster label_2 has just 12 clients, a maximum recency of 25, an average recency of only 5, an average frequency of 2813, and an average value of more than 100k dollars, all of which are significantly higher than those of clusters 0 and 1.

Then, using the agglomerative hierarchical clustering algorithm, we formed three clusters once more using the dendogram to determine the optimal number of clusters. These clusters resembled those produced by kmeans. These clusters are named Premium customers, regular customers, and not so regular customers towards the conclusion.

Premium customers :Customers with very high frequency and monetary value but recent activity are considered premium customers.
Regular customers :Customers with average frequency and monetary value but recent activity are considered regular customers.
Not so regular customers: Customers haven't made any purchases in the recent 4–5 months, and the purchases they have made have been modest in value and frequency.
