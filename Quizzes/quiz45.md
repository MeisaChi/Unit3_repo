# Code for finding the deposit, withdrawal and the balance
```.py
select sum(amount) from transactions where transaction_type = 'deposit' group by account_id
select sum(amount) from transactions where transaction_type = 'withdraw' group by account_id
select sum(balance) from accounts group by account_id
```
## Deposit
![](https://github.com/MeisaChi/Unit3_repo/blob/main/Sceenshots/quiz45_deposit.png)

## Withdraw
![](https://github.com/MeisaChi/Unit3_repo/blob/main/Sceenshots/quiz45_withdraw.png)

## Balance
![](https://github.com/MeisaChi/Unit3_repo/blob/main/Sceenshots/quiz45_balance.png)

# Calculations
|id|Deposit|Withdraw|Balance|Real Value|Match|
|-|-|-|-|-|-|
|1|1800|800|1000|1000|O|
|2|5900|900|5000|5000|O|
|3|1800|300|1500|1500|O|
|4|4300|300|4000|4000|O|
|5|2800|800|2000|2000|O|
|6|6400|400|6000|6000|O|
|7|2000|300|1700|1700|O|
|8|6100|600|5500|5500|O|
|9|1400|200|1200|1200|O|
|10|4800|300|4500|4500|O|
|11|1600|300|1300|1300|O|
|12|5200|600|5000|4600|X|
|13|2300|100|1400|2200|X|
|14|6400|400|6000|6000|O|
|15|2500|200|1500|2300|X|
|16|7600|600|7000|7000|O|
|17|2600|200|1600|2400|X|
|18|6600|600|6000|6000|O|
|19|2700|200|1700|2500|X|
|20|7600|600|7000|7000|O|


# Answer
```.py
select * from customers where customer_id = 12 or customer_id = 13 or customer_id = 15 or customer_id = 17 or customer_id = 19
```
![](https://github.com/MeisaChi/Unit3_repo/blob/main/Sceenshots/quiz45_answer.png)

