# Malicious Address Prediction

## Data Stats:
* Total no. of instances: 534
    * Malicious addresses: 267
    * Non-Malicious addresses: 267
* No. of attributes: 17

## List of attributes:
1. address
2. comment
3. no_of_out_transactions
4. tot_ether_sent
5. no_of_in_transactions
6. tot_ether_recieved
7. monthly_out_txn
8. monthly_in_txn
9. active_months
10. eth_balance
11. time_b/w_out_txn
12. time_b/w_in_txn
13. tot_token_value_recieved
14. tot_token_value_sent
15. monthly_ether_sent
16. monthly_ether_recieved
17. label
    
<h2> <a href='https://github.com/mshilpaa/ethereum-data-analysis/blob/master/Malicious_Address_Prediction/Data_Analytics.ipynb'>Distribution of the data: </a></h2>

<img src='https://github.com/mshilpaa/ethereum-data-analysis/blob/master/Malicious_Address_Prediction/images/Log1p(data)-1.png' />
<img src='https://github.com/mshilpaa/ethereum-data-analysis/blob/master/Malicious_Address_Prediction/images/Log1p(data)-2.png' />
<img src='https://github.com/mshilpaa/ethereum-data-analysis/blob/master/Malicious_Address_Prediction/images/Log1p(data)-3.png' />
<img src='https://github.com/mshilpaa/ethereum-data-analysis/blob/master/Malicious_Address_Prediction/images/Log1p(data)-4.png' />
<p align='center'>Fig.1: Log of the data</p>
 
From the above plot we see a clear distinction between the malicous and non-malicous address. 

The distinguishing attributes are:  Active months, ether balance, time between in and out transactions, tokens sent and received . All of these are low for malicious addresses. 

This can be a characteristic of a spam address which sends advertisements etc. to other addresses. These can be sent by a bot so time between transactions are low. Since their objective is sending spam messages, ether balance in their account is low, since ether is not needed by them to do their job.

 
<h2> <a href='https://github.com/mshilpaa/ethereum-data-analysis/blob/master/Malicious_Address_Prediction/Algorithms.ipynb'>Alogorithms Applied:</a></h2>

| Algorithm | Accuracy|
| --- | --- |
| Random Forest | 94.94 |
| MLP(Multi Layer Perceptron) | 92.13 |
| Logistic Regression | 87.64 |
| KNN (k=2) | 86.51 |

## References
<a href='https://github.com/MyEtherWallet/ethereum-lists/tree/master/src/addresses'>Malicious addresses repository</a>




