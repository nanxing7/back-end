# Vector源码阅读

## 📝 **Vector源码分析**

分析流程参考ArrayList集合,地址如下

https://think-studio.github.io/back-end/back-end-basic/java%E9%9B%86%E5%90%88/01-ArrayList%E6%BA%90%E7%A0%81%E9%98%85%E8%AF%BB.html



## 解析

Vector比较ArrayList来说,更多的是直接在方法上进行加锁了;加锁的粒度还是比较粗的



比如： add,set,get 等操作和读取集合的方法,都是有进行方法上synchronized进行加锁操作;方法里执行的逻辑其实和ArrayList是相似的

