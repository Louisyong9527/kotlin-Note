# kotlin-Note
kotlin  note

kotlin基本数据类型6种：Byte Short Int Float Long Double
java基本数据类型8种：  byte short int float long double char boolean


## 运算符
kotlin中无三元运算符，用 if(a>b) a else b 代替


## 类型检测&类型转换
###### is 

if (obj is String) = return obj.length // `obj` 在该条件分支内自动转换成 `String`
        
###### as
val x: String = y as String //若y为null，则抛出异常

val x: String? = y as String? //不会抛出异常

val x: String? = y as? String //as?在失败时返回 null

## for循环   可以循环遍历任何提供了迭代器的对象
迭代:
for (item in collection) print(item)

val items = listOf("apple", "banana", "kiwifruit")
for (index in items.indices) {
    println("item at $index is ${items[index]}")
}

通过索引遍历数组或list
for (i in array.indices) {
    println(array[i])
}
