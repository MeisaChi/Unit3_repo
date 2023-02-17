# Code
```.py
import sqlite3

connection = sqlite3.connect("quiz46.db")

haiku = """Code flows like a stream
Algorithms guide its way
In silence, it solves
"""

cursor = connection.cursor()
query = f"""Create table if not exists words(
    id integer primary key,
    word text not null,
    length int not null
)
"""

cursor.execute(query)
connection.commit()

for word in haiku.split():
    query1 = f"Insert into words(word, length) values('{word}',{len(word)})"
    cursor.execute(query1)
connection.commit()

query2 = f"select avg(length) from words"
out = cursor.execute(query2).fetchone()
connection.commit()
connection.close()
print(f"The average word length is {out}")
```

# Evidance
![](https://github.com/MeisaChi/Unit3_repo/blob/main/Sceenshots/quiz46.png)
![](https://github.com/MeisaChi/Unit3_repo/blob/main/Sceenshots/quiz46_2.png)
