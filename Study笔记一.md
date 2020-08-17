# Mysql学习

## 索引

高效的获取数据的**数据结构**

![image-20200817183528255](https://gitee.com/raylee-lilei/cdn/raw/master/image-20200817183528255.png)

### **索引优劣**

提高检索效率

降低排序成本



表结构占用空间

降低insert delete等操作的速度



### **B Tree** 

通过下面的元素构建BTree

![image-20200817193741071](https://gitee.com/raylee-lilei/cdn/raw/master/image-20200817193741071.png)

![image-20200817193827310](../../../../AppData/Roaming/Typora/typora-user-images/image-20200817193827310.png)

![image-20200817193906240](https://gitee.com/raylee-lilei/cdn/raw/master/image-20200817193906240.png)



![image-20200817193932522](../../../../AppData/Roaming/Typora/typora-user-images/image-20200817193932522.png)

![image-20200817194011226](https://gitee.com/raylee-lilei/cdn/raw/master/image-20200817194011226.png)

![image-20200817194031721](https://gitee.com/raylee-lilei/cdn/raw/master/image-20200817194031721.png)

![image-20200817194050698](https://gitee.com/raylee-lilei/cdn/raw/master/image-20200817194050698.png)

![image-20200817194143583](https://gitee.com/raylee-lilei/cdn/raw/master/image-20200817194143583.png)

![image-20200817194206603](https://gitee.com/raylee-lilei/cdn/raw/master/image-20200817194206603.png)

二叉树树高的问题通过BTree提高对磁盘的读写效率



### **B+Tree**

n叉BTree含有n-1个key ,B+树有n个key



叶子节点通过双向链表连接

非叶子节点不存数据

每个节点数据的个数和他的节点一样多，子节点的最大值存放在父节点里面

![image-20200817194931736](https://gitee.com/raylee-lilei/cdn/raw/master/image-20200817194931736.png)



### 索引分类

单值索引：一个索引只包含一个列（在一个列上建索引），一个表可以有多个列去建索引

唯一索引： 一个列中的所有值都是唯一 的 就可以在这个列中间唯一索引，这里列里面允许有NULL

复合索引：一个索引中包含多个列



