## 破解X-pack后的docker镜像
1. Linux 请 设置  ` sysctl -w vm.max_map_count=262144 `  或者 ` echo "vm.max_map_count=262144" > /etc/sysctl.conf `
2. `git clone https://github.com/depfish/docker-compose-elk.git`
3. `cd docker-compose-elk && docker-compose up -d`
4. 访问 `ES: http://127.0.0.1:9200/` 访问 `Kibana: http://127.0.0.1`  
>用户名/密码如下：
```
Changed password for user kibana
PASSWORD kibana = XPw5BqpjbUOuq8swFoBE

Changed password for user logstash_system
PASSWORD logstash_system = QLZ3IckPZu0lBWrMosHE

Changed password for user beats_system
PASSWORD beats_system = YsR8xqwSohTpIUD9ULQJ

Changed password for user elastic
PASSWORD elastic = 6LKJcMrlcIZPc9mN0G3G
```


>ELK破解参考教程：
* https://www.plaza4me.com/article/20180825223849878
* https://blog.csdn.net/yunfei1992/article/details/80987966
* https://www.cnblogs.com/jcici/p/9400369.html