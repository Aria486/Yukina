# Note
## MongoDB
####文档
文档是键值对的一个有序集。
####Shell基本操作
1.创建一张表
```db.users.save({
                     username:'admin' ,
                     password:'admin',
                     register_time : new Date(),
              })```
