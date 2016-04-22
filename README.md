#### Jedis 2.8.0 添加客户端统计功能
一、功能：

* 收集每个jedis命令的耗时统计
* 收集每个jedis命令返回值大小区间统计
* 收集jedis客户端的相关异常


二、对于Jedis2.8.0的改动

	基于jedis 2.8.0，改动非常小，只有三个文件：
    1.redis.clients.jedis.Connection
    2.redis.clients.jedis.JedisClusterCommand
	3.pom.xml
    具体可以参考：https://github.com/sohutv/jedis-2.8.0-stat/commit/0d82201172df25f769ced2786c88a5b928060c13


三、注意：

	这个jedis必须依赖cachecloud中的cachecloud-open-jedis-stat模块才可以使用。
    cachecloud github: https://github.com/sohutv/cachecloud