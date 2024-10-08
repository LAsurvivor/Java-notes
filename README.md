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
14. Rest和Restful区别
15. Restful的理解
16. 如何跨域
17. Spring cloud和dubbo的区别？Dubbo通信底层怎么做的？



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
17. 市面上哪些软件使用udp连接？视频对话是udp吗？
18. 三握四挥
19. close_wait/time_wait原理
20. Get/Post的区别
21. 死锁是什么？手写一个死锁
22. 死锁的四个条件是什么（互斥条件/请求和保持条件/不可剥夺条件/循环等待条件）
23. 互斥锁和自旋锁的区别
24. 403/304/500状态码的含义
25. 重定向和转发的区别
26. http和https的区别
27. 浏览器url输入https的请求会发生什么？
28. 长连接和短链接的区别
29. 对称加密和非对称加密是什么？
30. XSS攻击是什么？如何防止？DDOS攻击实现原理？怎么防护？
31. 消息队列的原理和使用消息队列的好处（异步处理提高系统性能/降低系统耦合性）
32. 使用消息队列会带来什么问题？
33. 有哪些消息队列？
34. DNS协议理解
35. 为什么有了IP还要有Mac地址？
36. 估计一台服务器同时可以发送的tcp/ip请求数量
37. 丢包和沾包的理解
38. cname和A记录的区别
39. ls -l指令涉及哪些系统调用



## Java相关

1. Java对象生成过程
2. 类加载的过程（加载/链接/初始化）
3. 静态内部类会被编译成几个class？
4. 为什么内部类可以访问外部类的class方法？
5. Java集合（容器）有哪些？
6. ArrayList/LinkedList/Vector区别？哪个是线程安全的？
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
19. cms和G1的区别？优缺点？
20. fullgc怎么排查？（dump->MAT)
21. 怎样fullgc？
22. fullgc的原因
23. 新生代内部划分（Eden/Survivor1/Survivor2）
24. 永久代和metaspace的区别
25. Java设计模式有哪些？（单例模式/适配器模式/模板模式/装饰器模式/代理模式/工厂模式）
26. 单例怎么实现？画图、手写双重检验锁单例（饿汉/懒汉/双重检验/volatile）
27. 双重检验为什么需要加volatile？（防止指令重排）
28. 有什么和双重检验等效的单例写法？
29. 如何让用户只能调用类的方法创建实例而不是通过new创建实例？（构造函数加private）
30. 为什么要双重检验
31. 双重检验锁定有哪些缺陷？
32. 享元模式/工厂/适配的理解
33. synchronized底层实现？JDK1.6前后对synchronized实现的变化？
34. synchronized(this)和synchronized(classname.class)的区别
35. ReentrantLock的底层实现原理？(AQS/CAS)
36. synchronized和ReentrantLock的区别
37. Java有哪两种流？（字符流和字节流）
38. Java IO有哪些？（同步阻塞BIO/同步非阻塞NIO/异步非阻塞AIO）
39. 什么情况下会发生阻塞？
40. 多路复用有哪些系统调用？实现原理？（select/pselect/poll/epoll）
41. netty是否了解？
42. wait和sleep的区别
43. 实现双线程的线程唤醒（Condition的signal和await）
44. Java concurrent包用过什么？
45. ConcurrentHashMap如何实现？
46. ConcurrentHashMap和SynchronizedHashMap的区别
47. 可重入锁和不可重入锁的理解
48. volatile/CAS/AQS的理解
49. volatile的底层实现？volatile是不是原子性的？volatile的有序性如何保障？
50. Java在哪个阶段做了原子指令重排？
51. final/finally/finalize分别是什么？
52. ==和equals的区别
53. 静态代理和动态代理的理解
54. 泛型的理解
55. 常见的异常类有哪些？
56. Integer和int的区别



## 数据库相关

1. 乐观锁与悲观锁的区别？如何实现？
2. 什么是共享锁、排他锁、意向锁？怎么写？
3. 间隙锁的理解
4. 行锁、页锁、表锁的理解？InnoDB默认支持哪些？
5. Mysql的底层数据结构是什么？为什么要用这个结构？（B+树）
6. Mysql索引优化
7. InnoDB和Myisam的区别？Mysql引擎的理解
8. 脏读/幻读/不可重复读的区别（幻读-增删/不可重复读-修改）
9. 对索引的理解？建立索引需要注意哪些问题？
10. 什么是回表查询？
11. sql和nosql的区别
12. nosql有哪些？和sql的区别
13. ACID的理解（原子性/一致性/隔离性/持久性）
14. 隔离级别的理解（串行化/可重复读/读已提交/读未提交）
15. 什么隔离级别可以防止幻读？
16. InnoDB的默认隔离级别是什么？
17. 左前缀原则是什么？
18. 数据库三范式是什么？
19. 判断某一个表是否符合第三范式要求，若不符合请修改表结构
20. 双表的联合查询
21. 聚簇索引和非聚簇索引的区别
22. 什么时候索引会失效，请举例
23. mvcc版本号控制https://segmentfault.com/a/1190000039097849
24. 用过哪些数据库
25. 为什么要列式存储
26. MongoDB怎么保证高可用
27. 为什么要用MongoDB
28. MySQL的引擎
29. Innodb5.1版本新增的内容有没有了解
30. MySQL的隔离级别
31. MySQL怎么防止幻读的，间隙锁的了解
32. MySQL怎么保证高可用，主从模式，binlog
33. 乐观锁和悲观锁的区别

## 数仓

1. 为什么要数仓
2. 哪些数据会给数仓处理
3. 你知道哪些是热点数据

## 缓存/中间件相关

1. Redis的主从模式/哨兵模式/集群模式的理解
2. Redis缓存雪崩/缓存穿透/缓存击穿的理解
3. Redis的基本数据类型（跳表）
4. Redis是单线程的吗？为什么这么设计？
5. Redis过期键删除策略理解
6. Redis的持久化理解
7. Kafka/RabbitMQ/RocketMQ的理解
8. 消息队列的优缺点（优点有异步、解耦、削峰）
9. 为什么需要缓存中间件？
10. Redis分布式锁http://kaito-kidd.com/2021/06/08/is-redis-distributed-lock-really-safe/
11. Redis如何实现高并发的（非阻塞IO）



## 数据结构相关

1. 红黑树/B树/B+树的区别
2. 红黑树相比二叉平衡树的优点
3. TreeMap的实现原理
4. HashMap的实现原理
5. 查找算法有哪些
6. 排序算法有哪些？复杂度分别是多少？
7. 手写快排
8. 手写优先队列（最大堆）
9. 拓扑排序相关题（实现有向图->记录入度出度->队列）
10. 背包问题
11. 不使用其他库来实现某算法
12. 每秒输入一个数，实现一个方法，可以输出之前输入的所有数中第k大的数（优先队列）



## 系统设计相关

1. 给你4台服务器分别1T用来存放一个用户的数据，用户只知道自己有2T的空间；设计IO。若用户一次性要存放2T的文件该怎么存？
2. 接上题。按照上题的策略，若4台服务器给两个用户使用应该如何存储？若用户想提升空间怎么办？
3. 数据库连接池设计


## Infra

1. 从输入网址到服务的过程，dns，网关，负载均衡，服务发现，REST，RPC
2. k8s的pod的一些使用
3. k8s有那些service
4. 负载均衡算法有哪些
5. 了解nginx吗
6. 如何让一些特定请求打到指定服务器（一致性哈希等方式）
7. 了解哪些流量算法（漏桶、令牌桶、拥塞控制）
8. Docker容器网络通信（默认桥接模式）
9. Docker指令有哪些

## DevOps

1. ps指令查看某个用户
2. awk指令
3. top指令
4. netstat指令
5. vim怎么用
6. 系统是怎么获取cpu占用情况的
7. shell脚本怎么写


## 其他

1. Git基本开发流程和项目管理方法？
2. Git有哪些命令？
3. Git如何版本迭代？
4. Git和svn区别
5. 为什么学Java


## JS/TS

1. hooks钩子了解吗
2. beforeMounted/afterMounted/beforeCreated/afterCreated的执行顺序
3. Dom树什么时候建立
4. 虚拟dom和真实dom的联系
5. 用过哪些组件
6. YARN为什么比npm高效，底层原理

## Python

1. 写单例
2. Pandas的表是列式存储还是行式存储
3. Python语法糖

## Go

1. channel底层实现原理
2. 什么时候channel会阻塞
3. buffered channel有序写入，读取时可以保证有序吗
4. Goroutine为什么高效，为什么有很大的并发度，和线程区别
5. Go的协程调度原理
6. 协程的上下文切换会涉及哪些寄存器，会存放哪些信息
7. Go的垃圾回收机制（CMS，三色）

## C++

1. 智能指针，手写shared_pointer
2. shared_pointer引用计数怎么实现（在堆上开辟内存）
3. 直接用普通指针创建智能指针和用make_shared来创建智能指针的区别
4. unique_pointer是怎么做到独占的
5. Lambda表达式
6. 编译时多态和运行时多态
7. 怎么实现多态，虚函数表存在哪里
8. 为什么要右值引用
9. 为什么要有左右值的区分
10. map, unordered_map, vector的插入、查询时间复杂度
11. 原子操作实现原理
12. 析构函数能是虚函数吗
13. 虚函数表实现
14. 指针常量和常量指针的区别
15. 范型编程的了解
16. 指令集
17. 指针和引用的区别
18. explicit和implicit
19. C++ debug工具有哪些（如何识别内存泄漏）
20. volatile/mutable/atomic
21. 返回值优化
22. char[]和string转化遇到的问题
23. deque/queue的内部实现（deque取值可以o(1)复杂度）
24. 4种cast方法
25. push_back和emplace_back的区别


