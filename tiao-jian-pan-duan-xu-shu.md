# 條件判斷敘述

## if...else
if是用來作控制流程的邏輯判斷，當條件成立的時候會執行 if 陳述式裡的程式，而不成立時則執行另外一個陳述式。

以下程式要求使用者輸入出生的年份，再利用內建 datetime 取得目前年份相減計算得出 Age 再使用 Age 變數判斷是否大於等於 18，若成立則印出你的年齡並告知你是成年，反之。

```py
import datetime
DOB=input("Enter your DOB:")
CurrentYear=datetime.datetime.now().year
Age=CurrentYear-int(DOB)
if(Age>=18):
    print("Your age is {} and you are Adult".format(Age))
else:
    print("Your age is {} and you are not Adult".format(Age))
```

## if...else if...else
若條件式判斷超過兩個時可以使用 `else if` 來表示，你可以發現在 Python 中或者是使用 `elif` 的縮寫來表示，跟其他大多數的程式語言有點不太一樣。

```py
Degree=input("enter your degree:")
if(int(Degree)>=90):
    print("your Score is A")
elif(int(Degree)>=80 and int(Degree)<90):
    print("your Score is B")
elif (int(Degree) >= 70 and int(Degree) < 80):
    print("your Score is C")
elif(int(Degree)>=60 and int(Degree)<70):
    print("your Score is D")
else:
    print("you fail")
```

## 總結
在 Python 中條件敘述判斷若裡面要執行多行時只要縮排就好，不像其他語言中要用大括號來表示這是一個執行區域．

```py
if 判斷條件1 : 
    執行語句1-1 …… 
    執行語句1-2 …… 
    執行語句1- 3… 
elif 判斷條件2 : 
    執行語句2 …… 
else : 
    執行語句3 …… 
```