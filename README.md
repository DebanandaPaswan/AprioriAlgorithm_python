# AprioriAlgorithm_python
Apriori algorithm works on the principle of Association Rule Mining.

In this project, it is implemented in python in jupyter.

Theory of Apriori Algorithm
There are 3 major components of Apriori algorithm.

1. Support
Frequency of occurence of a itemset. Support (A) = (Transactions containing (A)) / (Total Transactions)

2. Confidence
It refers to the likelihood that an item B is also bought if item A is bought.

Confidence(A->B) = (Transactions containing both (A and B)) / (Transactions containing (A))

3. Lift
Lift refers to the increase in the ratio of the sale of B when A is sold.

Lift = (Confidence (A->B))/(Support (B))

Association rule by Lift
lift = 1 -> There is no association between A and B

lift < 1 -> A and B are unlikely to be bought together

lift > 1 -> greater the lift greater is the likelihood of buying both products together.

#Cross_sell detection for e_commerce recommender system.
->find group_by transaction_id and item_id
->merge the group_by with Apriori rules output with Left_on="item_id" and right_on="antecedents" 
