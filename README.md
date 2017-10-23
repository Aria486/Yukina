# Note
## MongoDB
### 1.文档
文档是键值对的一个有序集。
### 2.基本操作
1.创建一张表
``` 
db.users.save({
                     username:'admin' ,
                     password:'admin',
                     register_time : new Date(),
              })
```
2.查询数据
```
db.users.find()
```
3.更新表
```
db.users.update(
    { "username": "admin" },
    { "$set": { "password": "123456" } }
)
```
4.插入
```
db.users.insert({
                     username:'test' ,
                     password:'test',
                     register_time : new Date()
              })
 ```
 5.删除（里面是条件，如果什么都不写将会删除整个集合）
 ```
db.users.remove({'username':'admin'})
```
6.唯一索引
```	
db.users.ensureIndex({"username":1},{"unique":true})
```
### 3.基本数据类型
· null：null表示空值或者不存在的字段
```
{"x" : null}
```
· boolean型: ture,false
· 数值: shell默认使用64位浮点数值型
```
{"x" : 3.14}
或
{"x" : 3}

整型: {"x" : NumberInt("3")}和{"x" : Number("3")}
```


