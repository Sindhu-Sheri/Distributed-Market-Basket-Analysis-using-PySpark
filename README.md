# Distributed-Market-Basket-Analysis-using-PySpark

Purpose of this project is to find the strength of association between pairs of products purchased together and identify the frequent patterns.

Languages Used: Python(pyspark)

DataSet Used: Online Browsing behavior dataset

**Steps in this project:**

1) A-Priori algorithm using a Spark program to find products which are frequently browsed together.

2) Support to s = 85 (i.e. itemsets need to occur at least 85 times to be considered frequent) and find itemsets of size 2, 3, and 4.

3) With frequent itemsets, generate association rules that has only one items on the right hand-side of the rule (i.e) {X} -> {Y} for frequent 2-itemset, {X,Y} -> Z, {X,Z} -> {Y}, and {Y, Z} -> {X} for frequent 3-itemset and so on and so forth.

4) Generate rules with confidence threshold c = 90%. Sort all association rules by decreasing order of confidence.


**Description of files:**

**a) MarketBasket Analysis.ipynb:** This program has pyspark apriori algorithm implementation to generate frequent itemsets. USing these frequent itemsets association rules are generated of size 2,3 & 4 with support s = 85 & confidence c=90%.

**b) browsing.txt:** This is an online browsing behaviour dataset which is used as an input for the apriori.
