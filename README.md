# Java开发面试题汇总

**说明：**以下为个人整理的部分Java开发面试题，供分享



## Spring相关

1. Spring的IoC/AOP是什么？底层是怎么实现的？
2. AOP的静态代理和动态代理是怎么实现的？
3. Spring mvc的框架是怎样的？
4. Spring boot是什么？
5. Spring boot和Spring MVC是什么关系？
6. Spring bean和Java bean的区别
7. Bean的作用域是什么？
8. Bean对象的循环依赖是什么？如何解决？
9. JPA是什么？
10. 了解jdbc吗？
11. JWT是什么？
12. Spring Security的底层实现？
13. Spring有哪些注解？
14. Restful的理解
15. 如何跨域
16. Spring cloud和dubbo的区别？Dubbo通信底层怎么做的？



## 操作系统/计算机网络相关

1. 线程与进程的区别
2. 进程间的通信方式有哪些？（管道/消息队列/共享内存/信号量/信号/Socket）
3. 线程通信方式理解
4. 进程调度算法
5. 协程是什么？
6. 为什么会涉及上下文切换？
7. 有哪些熟悉的syscall?
8. Linux大概有多少syscall?
9. 为什么要有虚拟地址和物理地址的映射？
10. 虚拟地址和物理地址的表达方式有什么差异？
11. 多线程的理解
12. 线程有哪些状态？线程分别如何进入这些状态？
13. 内存泄漏原因？举例
14. Linux有哪些命令？
15. Windows和Linux的IO模型有什么区别？
16. Tcp/Udp的区别
17. 三握四挥
18. close_wait/time_wait原理
19. Get/Post的区别
20. 死锁是什么？手写一个死锁
21. 死锁的四个条件是什么（互斥条件/请求和保持条件/不可剥夺条件/循环等待条件）
22. 互斥锁和自旋锁的区别
23. 403/304/500状态码的含义
24. 重定向和转发的区别
25. http和https的区别
26. 浏览器url输入https的请求会发生什么？
27. 长连接和短链接的区别
28. 对称加密和非对称加密是什么？
29. XSS攻击是什么？如何防止？DDOS攻击实现原理？怎么防护？
30. 消息队列的原理和使用消息队列的好处（异步处理提高系统性能/降低系统耦合性）
31. 使用消息队列会带来什么问题？
32. 有哪些消息队列？
33. DNS协议理解



## Java相关

1. Java对象生成过程
2. 类加载的过程（加载/链接/初始化）
3. 静态内部类会被编译成几个class？
4. 为什么内部类可以访问外部类的class方法？
5. Java集合（容器）有哪些？
6. ArrayList/LinkedList/Vector区别
7. HashMap/HashTable区别
8. Java的多态是什么？
9. Java为什么没有多继承？如何实现多继承？
10. 重载和重写的区别
11. 抽象类和接口的区别
12. Java线程池有哪些？意义是什么？
13. JDK线程池有哪些参数？各个参数的意义？有哪些拒绝策略？
14. newCacheThreadPool的使用有什么弊端？
15. Java线程如何交互
16. JVM是什么？
17. JVM的内存管理模型？其中哪些是线程独占的？
18. GC机制有哪些？
19. cms和G1的区别？
20. Java设计模式有哪些？（单例模式/适配器模式/模板模式/装饰器模式/代理模式/工厂模式）
21. 单例怎么实现？画图、手写双重检验锁单例（饿汉/懒汉/双重检验/volatile）
22. 有什么和双重检验等效的单例写法？
23. 如何让用户只能调用类的方法创建实例而不是通过new创建实例？（构造函数加private）
24. 为什么要双重检验
25. 双重检验锁定有哪些缺陷？
26. 享元模式/工厂/适配的理解
27. synchronized底层实现？JDK1.6前后对synchronized实现的变化？
28. synchronized(this)和synchronized(classname.class)的区别
29. ReentrantLock的底层实现原理？(AQS/CAS)
30. synchronized和ReentrantLock的区别
31. Java有哪两种流？（字符流和字节流）
32. Java IO有哪些？（同步阻塞BIO/同步非阻塞NIO/异步非阻塞AIO）
33. 什么情况下会发生阻塞？
34. 多路复用有哪些系统调用？实现原理？（select/pselect/poll/epoll）
35. netty是否了解？
36. wait和sleep的区别
37. 实现双线程的线程唤醒（Condition的signal和await）
38. Java concurrent包用过什么？
39. concurrentHashMap如何实现？
40. volatile/CAS/AQS的理解
41. volatile的底层实现？volatile是不是原子性的？volatile的有序性如何保障？
42. Java在哪个阶段做了原子指令重排？
43. final/finally/finalize分别是什么？
44. ==和equals的区别
45. 静态代理和动态代理的理解
46. 泛型的理解
47. 常见的异常类有哪些？
48. Integer和int的区别



## 数据库相关

1. 乐观锁与悲观锁的区别？如何实现？
2. 什么是共享锁、排他锁、意向锁？怎么写？
3. 间隙锁的理解
4. Mysql的底层数据结构是什么？为什么要用这个结构？（B+树）
5. Mysql索引优化
6. InnoDB和Myisam的区别？Mysql引擎的理解
7. 脏读/幻读/不可重复读的区别（幻读-增删/不可重复读-修改）
8. 对索引的理解？建立索引需要注意哪些问题？
9. 什么是回表查询？
10. sql和nosql的区别
11. nosql有哪些？和sql的区别
12. ACID的理解（原子性/一致性/隔离性/持久性）
13. 隔离级别的理解（串行化/可重复读/读已提交/读未提交）
14. 什么隔离级别可以防止幻读？
15. InnoDB的默认隔离级别是什么？
16. 左前缀原则是什么？
17. 数据库三范式是什么？
18. 判断某一个表是否符合第三范式要求，若不符合请修改表结构
19. 双表的联合查询
20. 聚簇索引和非聚簇索引的区别
21. 什么时候索引会失效，请举例



## 缓存/中间件相关

1. Redis的主从模式/哨兵模式/集群模式的理解
2. Redis缓存雪崩/缓存穿透/缓存击穿的理解
3. Redis的基本数据类型（跳表）
4. Redis是单线程的吗？为什么这么设计？
5. Redis过期键删除策略理解
6. Kafka/RabbitMQ/RocketMQ的理解
7. 为什么需要缓存中间件？



## 数据结构相关

1. 红黑树/B树/B+树的区别
2. 红黑树相比二叉平衡树的优点
3. TreeMap的实现原理
4. HashMap的实现原理
5. 查找算法有哪些
6. 排序算法有哪些？复杂度分别是多少？
7. 手写快排
8. 手写优先队列（最大堆）



## 系统设计相关

1. 给你4台服务器分别1T用来存放一个用户的数据，用户只知道自己有2T的空间；设计IO。若用户一次性要存放2T的文件该怎么存？
2. 接上题。按照上题的策略，若4台服务器给两个用户使用应该如何存储？若用户想提升空间怎么办？



## 其他

1. Git基本开发流程？有哪些命令？
2. Git和svn区别
3. 为什么学Java