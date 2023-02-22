# Python Code
```.py
import sqlite3
from secure_password import check_password

class database_bitcoin:
    def __init__(self, name):
        self.connection = sqlite3.connect(name)
        self.cursor = self.connection.cursor()

    def search(self, query):
        result = self.cursor.execute(query).fetchall()
        return result

    def close(self):
        self.connection.close()

x = database_bitcoin("bitcoin_exchange.db")

query = "SELECT * from ledger"
result = x.search(query)
x.close()

for row in result:
    id = row[0]
    sender_id = row[1]
    receiver_id = row[2]
    amount = row[3]
    hash = row[4]
    string_hash = f"id {id},sender_id {sender_id},receiver_id {receiver_id},amount {amount}"
    if check_password(hashed_password=hash, user_password=string_hash):
        print(f"\033[1;32mid:{id} Signature matches \n")
    else:
        print(f"\033[1;31mid:{id} Error signature \n")
```

# Answer
![](https://github.com/MeisaChi/Unit3_repo/blob/main/Sceenshots/quiz48.png)
