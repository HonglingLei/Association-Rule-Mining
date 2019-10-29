README
================

Overview
----------
I used supermarket receipts to analyze associations (Support, Confidence, Lift, etc.) between consumer goods. Instead of employing Apriori Algorithm - the traditional solution - I used a simpler method which generates the same results within a shorter execution time. Loops are avoided so it took only 0.04 second to analyze 9995 receipts.

Motivation
--------
As Usman Malik wrote, "Association rule mining is a technique to identify underlying relations between different items. Take an example of a Super Market where customers can buy variety of items. Usually, there is a pattern in what the customers buy. For instance, mothers with babies buy baby products such as milk and diapers. Damsels may buy makeup items whereas bachelors may buy beers and chips etc. In short, transactions involve a pattern. More profit can be generated if the relationship between the items purchased in different transactions can be identified."

Data
--------
[Sample - SuperStore.xls](https://github.com/HonglingLei/association-rule-mining/blob/master/Sample%20-%20Superstore.xls) is my raw data. It contains 9995 receipts; each containing `Row ID`,	`Order ID`,	`Order Date`,	`Ship Date`,	`Ship Mode`,	`Customer ID`,	`Customer Name`,	`Segment`,	`Country`,	`City`,	`State`,	`Postal Code`,	`Region`,	`Product ID`,	`Category`,	`Sub-Category`,	`Product Name`,	`Sales`,	`Quantity`,	`Discount`,	`Profit`.

Code
--------
My [code](https://github.com/HonglingLei/association-rule-mining/blob/master/%5BCode%5D%20Sample%20Superstore%20Association.ipynb) is detailedly commented so each step should be easy to understand. As you can see, this optimized method does not contain any loop (my first version had 3 loops and 2 ifs) so it runs much faster.

Results
--------
Demo results can be seen in my code file. The file includes `XID`, `YID`, `n_XY`, `n_X`, `n_Y`, `n_Transactions`, `Support`, `Confidence`, and `Lift`. Click [here](https://github.com/HonglingLei/association-rule-mining/blob/master/Sample%20Supperstore%20Association%20Results.xls) to download the complete excel.

Additional Reading 
--------
If you would like to know more about association rule mining, here are some suggested sources.
- [Association Rule Mining via Apriori Algorithm in Python](https://stackabuse.com/association-rule-mining-via-apriori-algorithm-in-python/) by Usman Malik
- [Association Analysis: Basic Concepts and Algorithms](https://github.com/HonglingLei/association-rule-mining/blob/master/Association%20analysis.pdf) 
- [Association rules - mixtend](http://rasbt.github.io/mlxtend/user_guide/frequent_patterns/association_rules/)

