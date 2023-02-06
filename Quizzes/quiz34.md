## Code
```.py
def to_roman(num):
    romandict = {1:"I", 5:"V", 10:"X", 50:"L", 100:"C"}
    if not isinstance(num, int):
        raise TypeError("input must be integer")
    if num <= 0 or num > 100:
        raise ValueError("input must be 1~100")
    num = str(num)
    out = ""
    while num != "":
        if 1<=int(num[0])<= 3:
            out += romandict[10**(len(num)-1)]*int(num[0])
        if int(num[0]) == 4 or int(num[0]) == 9:
            out += romandict[10**(len(num)-1)]
            out += romandict[(int(num[0])+1)*10**(len(num)-1)]
        if 5<=int(num[0])<=8:
            out += romandict[5*10**(len(num)-1)]
            out += romandict[10**(len(num)-1)]*(int(num[0])-5)
        num = num[1:]
    return out
```
## Code for test
```.py
from quiz34 import to_roman

import pytest

def test_to_roman():
    assert to_roman(1) == 'I'
    assert to_roman(4) == 'IV'
    assert to_roman(9) == 'IX'
    assert to_roman(37) == 'XXXVII'
    assert to_roman(44) == 'XLIV'
    assert to_roman(50) == 'L'
    assert to_roman(99) == 'XCIX'
    assert to_roman(100) == 'C'
    assert to_roman(77) == 'LXXVII'
    assert to_roman(93) == 'XCIII'


def test_to_roman_exceptions():
    # check that the program raises a ValueError
    with pytest.raises(ValueError):
        to_roman(101)
```
![](https://github.com/MeisaChi/Unit3_repo/blob/main/Sceenshots/quiz34.png)
