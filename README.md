# j2ee
1，Configuration接口：配置Hibernate，根据其启动Hibernate，创建SessionFactory对象；

2，SessionFactory接口：初始化Hibernate，充当数据存储源的代理，创建session对象，SessionFactory是

      线程安全的，意味着它的同一个实例可以被应用的多个线程共享，是重量级二级缓存；

3，session接口：负责保存、更新、删除、加载和查询对象，是一个非线程安全的，避免多个线程共享一个session，是轻量级，一级缓存。

4，Transaction接口：管理事务。可以对事务进行提交和回滚；

5，Query和Criteria接口：执行数据库的查询。
