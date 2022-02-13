# APRIORI ALGORITHM

Association Rule

Association rule learning works on the concept of If and Else Statement, such as if A then B.
A→B
If→Then
Here the If element is called antecedent, and then statement is called as Consequent. 
These types of relationships where we can find out some association or correlation between two items is known as single cardinality. 
 It is all about creating rules, and if the number of items increases, then cardinality also increases accordingly.
So, to measure the associations between thousands of data items, there are several metrics. These metrics are given below:
Support
Confidence
Lift


## SUPPORT
Support is the frequency of item or how frequently an item appears in the dataset. It is defined as the fraction of the transaction T that contains the itemset X. If there are X datasets, then for transactions T, it can be written as:

SUPPORT = FREQUENCY(ITEM)/#TRANSACTIONS

## CONFIDENCE
Confidence indicates how often the items A and B occur together in the dataset when the occurrence of A is already given. It is the ratio of the transaction that contains A and B to the number of records that contain A.

CONFIDENCE=FREQ(A,B)/FREQ(A)

## LIFT
It is the strength of any rule, which can be defined as below formula:
LIFT = SUPPORT(A,B)/(SUPPORT(A))*SUPPORT(B))

Given a set of transactions, we can find rules that will predict the occurrence of an item based on the occurrences of other items in the transaction.

![Capture0](https://user-images.githubusercontent.com/95124698/153754238-262c4e3f-d12f-4aeb-840d-5af7dd8aacf5.PNG)

![Capture](https://user-images.githubusercontent.com/95124698/153754258-eaa31c2f-33ea-477b-a128-634293ef5519.PNG)

![Capture2](https://user-images.githubusercontent.com/95124698/153754262-eea59eef-0c45-4124-b8d0-51c167133168.PNG)

FOR RULES::
1.BREAD,JUICE
2.CHEESE,JUICE

1.BREAD,JUICE

BREAD→JUICE
JUICE→BREAD

CONFIDENCE(A→B)=SUPPORT(A U B)/SUPPORT(A)
  

1.BREAD→JUICE= (3*5)/(5*4)=75%
2.JUICE→BREAD= (3*5)/(5*4)=75%
3.CHEESE→JUICE = (3*5)/(5*3)=100%
4.JUICE→CHEESE = (3*5)/(5*4)=75%
 
SINCE, ALL CONFIDENCE VALUES ARE GREATER THAN THE VALUE OF CONFIDENCE WHICH IS GIVEN HENCE ALL THE RULES CAN BE USED.


