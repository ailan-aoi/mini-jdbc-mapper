# mini-jdbc-mapper

用注解把数据库表映射成 Java 对象，再通过 JDBC 做查询和插入，并自带一个简单连接池。

写于 2020 年，用来练习「表和类怎么对应、连接从哪来、一行结果怎么填回对象」。

## 里面有什么

- 注解：`@Table`、`@Column`、`@Id`
- `Query`：`selectAll`、`selectOneById`、`insert`
- `ConnectionPool`：按配置维护连接
- `ClassPathAnnotationApplicationContext` / `ClassPathXMLApplicationContext`：从注解或 XML 读映射

源码在 `easyDatabaseUtil/src`，包名 `com.mec.dataBase`。目录是当时的 Eclipse 工程，MySQL 驱动在 `src/libs`。连接信息看 `dataBaseCfg.properties`。

## 状态

学习代码，源码按最初上传的样子保留。仓库曾用名 `easyDatabaseUtil`，旧地址会重定向到这里。
