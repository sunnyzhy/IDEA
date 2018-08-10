# maven打包命令
```
mvn clean package -DskipTests
```

# java运行命令
```
java -Xms512m -Xmx512m -XX:MaxPermSize=256m -jar xxx.jar --server.port=xxxx
```

# IDEA打包
1. **打开Maven Projects**

2. **选择Lifecycle package**

3. **点击 Toggle "Skip Tests" Mode，禁用 test**

4. **clean**

5. **package**

# IDEA远程调试
1. **Run -> Edit Configurations**

2. **添加一个新配置，选择Remote**

3. **配置远程服务地址和端口，端口一定要跟下面命令行里的 address 相同**

4. **启动调试**

```
# java -jar -Xmx256m -Xms256m -Xdebug -Xrunjdwp:transport=dt_socket,server=y,suspend=n,address=80 /usr/local/jar/xxx.jar
```
```
address指定调试端口，根据实际环境修改。
```
