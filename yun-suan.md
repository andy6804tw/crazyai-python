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

## 布林運算子 boolean operations
在程式語言中布林運算扮演很重要角色，任何物件都可以用來作為真值判斷，可以應用在 `if...else` 或迴圈中，在以下範例中我們可以用 `and(&)` 與 `or(|)` 運算子來做真假運算。

```py
x=True
y=False

print(x and y) # False
print(x or y) # True
print(3>5) # False
print(3<5) # True
```

## 運算優先 priorites
數學運算的優先權，是從左至右先乘除後加減，若遇到括號則先處理括號內容。

```py
print(3+10*5) # 53
print((3+10)*5) # 65
```

## 型態轉換 Convert between Data Type
在 Python 中轉換任何型態非常方便，內建提供函式快速可以將字串轉成任何型態或是將任何型態轉成字串。

```py
x="10"
print(type(x)) # <class 'str'>
# 字串轉整數型態
xInt=int(x)
print(type(xInt)) # <class 'int'>
# 字串轉浮點數型態
xFloat=float(x)
print(type(xFloat)) # <class 'float'>
# 整數轉字串型態
y=10
yStr=str(y)
print(type(yStr)) # <class 'str'>
```

在 Python 中所有的型態包括如下：
- str
- int
- float
- long
- list
- set()
- dict()
- tuple()

## 切割 slice
以下是簡單地將串列使用 `:` 來做片段擷取數值。

```py
list=[1,3,5,7,9]
print(list) # [1, 3, 5, 7, 9]
print(list[1:3]) # [3, 5]
```

接著進階使用方法，我們還可以在指定的位置插入新的串列。

```py
list[:]=range(10)
print(list) # [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
list[1:3]=(99,99) # 在1和3間插入(2的數值覆蓋捨去)
print(list) # [0, 99, 99, 3, 4, 5, 6, 7, 8, 9]
list[:0]=(-2,-1) # 在最前面插入
print(list) # [-2, -1, 0, 99, 99, 3, 4, 5, 6, 7, 8, 9]  
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

