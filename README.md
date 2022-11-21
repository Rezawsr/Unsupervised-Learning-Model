## UNSUPERVISED LEARNING MINI PROJECT

### CONTEXT

> E-commerce has become a new channel to support businesses development. Through e-commerce, businesses can get access and establish a wider market presence by providing cheaper and more efficient distribution channels for their products or services. E-commerce has also changed the way people shop and consume products and services. Many people are turning to their computers or smart devices to order goods, which can easily be delivered to their homes.

### CONTENT
> This is a sales transaction data set of UK-based e-commerce (online retail) for one year. This London-based shop has been selling gifts and homewares for adults and children through the website since 2007. Their customers come from all over the world and usually make direct purchases for themselves. There are also small businesses that buy in bulk and sell to other customers through retail outlet channels.

> The data set contains 500K rows and 8 columns. The following is the description of each column.

> - **TransactionNo (categorical)**: a six-digit unique number that defines each transaction. The letter “C” in the code indicates a cancellation.
> - **Date (numeric)**: the date when each transaction was generated.
> - **ProductNo (categorical)**: a five or six-digit unique character used to identify a specific product.
> - **Product (categorical)**: product/item name.
> - **Price (numeric)**: the price of each product per unit in pound sterling (£).
> - **Quantity (numeric)**: the quantity of each product per transaction. Negative values related to cancelled transactions.
> - **CustomerNo (categorical)**: a five-digit unique number that defines each customer.
> - **Country (categorical)**: name of the country where the customer resides.

### GOAL

> Gather useful intrinsic information by combining RFM model and some unsupervised learning model. 

> For each segments, analyze the data, and try to answer the following questions:

> - How was the sales trend over the months?
> - What are the most frequent purchased products?
> - How many products does the customer purchase in each transaction?
> - How does each cluster/group contribute to the company's revenue?
> - What are the interval date between transactions?
> - Based on your findings, what strategy could you recommend to the business to gain more profit?
> - ***add more if necessary***

> Also, there is a small percentage of order cancellation in the data set. Most of these cancellations were due to out-of-stock conditions on some products. Under this situation, customers tend to cancel an order as they want all products delivered all at once. 

> Therefore, try to build a supervised learning model to solve this problem.

> Source from UCI Machine Learning Repository: [link to dataset](https://archive.ics.uci.edu/ml/datasets/online+retail)



## SUMMARY
>Through the data exploration that we did, we came to the following conclusion:

> - There are 2% of customers who cancel, while there are 98% who do not cancel.
> - Sales trend over a month varied each cluster

####  What are the most frequent purchased products?
> - With a total of 1933 items sold, the WHITE HANGING HEART T-LIGHT HOLDER is the most popular product in ___cluster 0___.
REGENCY CAKESTAND 3 TIER came in second with 1734 item sold. 
> - In ___cluster 1___, the most frequently purchased item was the SPACEBOY LUNCH BOX with a total of 25 items, followed by the ROUND SNACK BOXES SET OF 4 WOODLAND with a total of 24 items
> - In cluster 2, the most frequently purchased items were JUMBO BAG RED RETROSPOT with a total of 171 items sold, followed by REGENCY CAKESTAND 3 TIER with a total of 163 items sold. 
#### How many products does the customer purchase in each transaction?
> - In cluster 0, the highest number of products purchased by customers for each transaction is 399.
> - In Cluster 1, the highest number of products purchased by customers for each transaction is 125.
> - In Cluster 2, the highest number of products purchased by customers for each transaction is 542.

> ___At the same time, cluster 2 is the largest purchase in each transaction.___

### How does each cluster/group contribute to the company's revenue?
> - Cluster 0 contributes to the company's revenue as much as $6233024.783999999

> - Cluster 1 contributes to the company's revenue as much as $723409.68

> - Cluster 2 contributes to the company's revenue as much as $1343631.35

> ___It can be concluded that cluster 0 is the cluster with the highest revenue contribution for the company.___

### What are the interval date between transactions?
> - Interval Cluster 0( Min: 0 Max: 373 )
> - Interval Cluster 1( Min: 0 Max: 8 )
> - Interval Cluster 2( Min: 0 Max: 38 )

### The Strategies That we recommend to businesses to gain more profit are:

> - Increasing the stock of product, because there is 2% customer cancelled the order due to out-of-stock conditions on some products
> - Maybe we can create a discount voucher for each cluster to increase salles and also keeping the customers on making transactions.
> - Even though cluster 1 has low shopping frequency, they are the cluster that has the highest monetary, so maybe we can create a loyalty program to increase their shopping frequency so we dont lose them

