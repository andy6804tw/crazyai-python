# 運算 Operations

## 數學運算 Math operations

- 加法、減法

```py
x=3+2
print(x) # 5

y=3-2
print(y) # 1
```

- 乘法

```py
x=3*2
print(x) # 6
```

- 除法

```py
# 除法
x=3/2
print(x) # 1.5

# 除法(小數點無條件捨去)
y=3//2
print(y) # 1

# 餘數
z=8%3
print(z) # 2
```

## 位元運算子 bitwise
位元運算子（Bitwise operator），數位設計上有AND、OR、NOT、XOR 與補數等運算，在Python中可以通過以"0b"或者"-0b"開頭的字符串來表示二進制，如下所示：

```py
x=0b111
y=0b101

print(x&y) # 5
print(x|y) # 7
```

## 小試身手
請寫出一個程式能夠輸入使用者出生西元年並計算出目前幾歲，使用 `datetime
` 函式庫並使用 `input` 方法提取使用者輸入。

```py
import datetime
DOB=input("Enter your DOB:")
CurrentYear=datetime.datetime.now().year
Age=CurrentYear-int(DOB)
print("Your age is {}".format(Age))
```

![](/assets/img4-1.png)

