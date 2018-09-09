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
