# 迴圈(Loop Control)
迴圈在程式語言中就是迭代陳述，能夠讓程式碼反覆的執行，可以減少重複造成程式碼的攏長，在這邊分別介紹 `while` 迴圈和 `for`迴圈。 

## while迴圈
`while`迴圈必須要有一個計數變數，所以在迴圈一開始必須設定一個變數並設初始值，`while()`中的括號要設定迴圈跑的次數(規則)，通常都是用判斷式來設定迴圈跑的次數，最後切記迴圈的最後一行一定要將變數加一否則會形成無窮迴圈。

```py
i=1
while(i<5):
    print("number {}".format(i))
    i=i+1

print("App is done")
```

![](/assets/img6-1.png)

## for迴圈
在 Python 中迴圈走訪，會有 `for in` 後面可以放集合或是 `range()`，以下為一個簡單的例子依續印出0~4，這邊注意一下`range(5)`是跑0~4。

```py
for i in range(5):
    print("number {}".format(i))

print("App is done")
```

![](/assets/img6-2.png)

`for` 迴圈的第二種方法是可以直接跑字串或是集合內的元素，依序的將值走訪。
```py
for letter in 'Python':
    print('當前字母 :', letter)

fruits = ['banana', 'apple', 'mango']
for fruit in fruits:
    print('當前水果 :', fruit)

print("Good bye!")
```

![](/assets/img6-3.png)

## Break and Continue
此兩個關鍵字只出現於迴圈當中使用，`break` 顧名思義就是馬上終止跳出迴圈，而 `continue` 就是直接跳過執行下一個迴圈內容所以 `continue` 之後的內容就不會執行到。

第一個範例是字串走訪，當遇到 `t` 時就 `break` 跳出迴圈不繼續走訪剩餘字元。

```py
word="Python"
for letter in word:
    if (letter == 't'):
        break;
    print(letter)
```

![](/assets/img6-4.png)

第二個範例跟第一個類似只是將 `break` 改成 `continue`，執行後你會發現字元 `t` 跳過並無被印出來，由此可證當執行 `continue` 時會直接跳過並執行下一個新的程序。

```py
word="Python"
for letter in word:
    if (letter == 't'):
        continue;
    print(letter)
```

![](/assets/img6-5.png)