## Code
```.py
class Account:
    def __init__(this_account):
        this_account.balance = 0
        this_account.holder_name = ""
        this_account.holder_email = ""
        this_account.number = [200,99203,1]

    def get_account_no(this_account)->str:
        number = this_account.number
        number = f"{this_account.number[0]}-{this_account.number[1]}-{this_account.number[2]}"
        return number

    def get_balance(this_account)-> int:
        return this_account.balance

    def set_holder_name(this_account, name=str)-> str:
        if this_account.holder_name == name:
            raise TypeError("This name already exists")
        if isinstance(name, int):
            raise TypeError("Please enter a name")
        this_account.holder_name = name
        msg = f"Holder's name set to {this_account.holder_name}"
        return msg

    def set_holder_email(this_account, email=str)-> str:
        if str(email).count("@") != 1:
            raise ValueError("Please input an available email")
        this_account.holder_email = email
        msg2 = f"Holder's email set to {this_account.holder_email}"
        return msg2

    def deposit(this_account, amount=int)-> str:
        this_account.balance = amount
        msg3 = f"New balance: {this_account.balance} USD"
        return msg3
```
## Code for test
```.py
import pytest
from quiz35 import Account

def test_empty_account():
    bk = Account()
    assert bk.balance == 0
    assert bk.holder_name == ""
    assert bk.holder_email == ""
    assert isinstance(bk.number, list)
    number = bk.get_account_no().split("-")
    assert  len(number)==3 and len(number[0])==3 and len(number[1])==5 and len(number[2])==1

def test_create_account():
    bk = Account()
    assert bk.get_balance() == 0
    assert bk.set_holder_name(name="Bob") == "Holder's name set to Bob"
    assert bk.set_holder_email(email="bob@company.xyz") == "Holder's email set to bob@company.xyz"
    assert bk.deposit(amount=100) == "New balance: 100 USD"
    assert bk.get_balance() == 100


def test_value_errors():
    bk = Account()
    with pytest.raises(ValueError):
        bk.set_holder_email(email="bob@bob@bob")
        bk.set_holder_name(name=["Bob"])
        bk.set_holder_name(name=100)

```
![](https://github.com/MeisaChi/Unit3_repo/blob/main/Sceenshots/quiz35.png)
