# 集合 Collections
## 串列 list 與元組 tuple
在程式語言中通常可以利用序列式方式去記錄資料，在 Python 中，我們使用 list 串列和 tuple 元組來儲存序列式資料。兩者最大的不同在於 tuple 是不可以改變的。

### 元組 tuple
由於 tuple 是不可以改變的所以在新增變數時就立即給予值，此外要存取元素方法可以像下面範例：

```py
array=(1,2,3,4,5) 
print(array) # (1, 2, 3, 4, 5)
print(array[0:3]) # (1, 2, 3)
```


## 串列 list
串列是一連串順序性的元素組成，我們可以新增、讀取、刪除和修改串列。

- 建立串列
```py
list0 = [] # 建立空串列
list1 = list() # 建立空串列
list2 = ['python', 'js', 'SQL'] # 建立串列並賦值
```

        ```py
# 串列拆字
array=list('python')
print(array) # ['p', 'y', 't', 'h', 'o', 'n']
```


- 使用索引值和範圍來取得元素
索引值(index)通常是從 0 開始，-1 從結尾數回來，範圍取值的使用方法為 [開始:結束]。
```py
array=[1,2,3,4,5]
print(array[1:3]) # [2, 3]
print(array[-1]) # [5] 
```

        > index [-1] = [4]


- 串列呼叫方法
```py
array=[1,2,3,4,5]
print(array) # [1, 2, 3, 4, 5]
array.append(7) # 在串列最尾插入值
print(array) # [1, 2, 3, 4, 5, 7]
array.insert(5,6) # 在指定索引位置插入值
print(array) # [1, 2, 3, 4, 5, 6, 7]
```


- 刪除指定元素
```py
array=[1,2,3,4,5]
del array[0] # 刪除指定元素
print(array) # [2, 3, 4, 5]
```

## 字典 Dictionary
在 Python 中 Dictionary 就很像是 Java 中的 HashMap 簡單來說一個鍵(key)對應到一個值(value)。

- 建立一個 Dictionary 物件
```py
# 建立一個 Dictionary 物件
person=dict(name="Andy",age=12)
print(person["age"]) # 12
print(person) # {'name': 'Andy', 'age': 12}
```

- 新增或修改一筆資料
```py
person=dict(name="Andy",age=12)
person["age"]=22 # 新增或修改一筆資料
print(person) # {'name': 'Andy', 'age': 22}
```

- 刪除一筆資料
```py
person=dict(name="Andy",age=12)
del person["age"] # 刪除一筆資料
print(person) # {'name': 'Andy'}
```

- 查詢某 key 是否存在
```py
person=dict(name="Andy",age=12)
print("name" in person) # True
```