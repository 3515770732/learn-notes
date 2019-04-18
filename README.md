**redis 学习**

 官网网址： https://redis.io/documentation
 
 
 **不同类型的操作命令**
 
**` String类型`  ( 一个键最大能存储512MB)**

 set name value _如 set chen 001_
 
 get name       _如 get chen_
 
 **`hash类型`( 每个 hash 可以存储 232 -1 键值对（40多亿）)**

hmset hashname keyname value  _如 hmset myhash field1 001_

hget  hashname keyname        _如 hget  myhash field1_

**`list类型`(列表最多可存储 232 - 1 元素 (4294967295, 每个列表可存储40多亿)，输出倒叙)**

lpush name value      _如 lpush mylist redis   lpush mylish rabbitmq_

lrange name           _如 lrange mylist_

**`set类型`（集合中最大的成员数为 232 - 1(4294967295, 每个集合可存储40多亿个成员)）**

sadd name value   _如 sadd myset  redis_

smembers name     _如 smemerbs   myset_ 

**`zset(sorted set：有序集合)`**

zadd name score value   如 zadd myzset 0 redis 

zrangebyscore myzset 0 0






 