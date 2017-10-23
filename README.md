# Note
## MongoDB
### 文档
文档是键值对的一个有序集。
### 基本操作
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

