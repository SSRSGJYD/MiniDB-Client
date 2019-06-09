# MiniDB-Client

Maven project for MiniDB Client

## 简介

此项目是MiniDB数据库的客户端，基于Maven和JavaFX。

MiniDB数据库项目地址：<https://github.com/SSRSGJYD/MiniDB>



## 运行

1. 当Java环境为Java1.8时，下载release版本的Client.jar (<https://github.com/SSRSGJYD/MiniDB-Client/releases>)，在同级目录下执行

   ```shell
   java -jar Client.jar
   ```

2. IDEA

   当Java环境为Java1.9及以上时，在IDEA中设置configuration为：

```shell
main class: application.ClientDialog
VM option: --module-path path\to\javafx-sdk\lib --add-modules=javafx.controls,javafx.fxml
jre: path\to\jdk
```

3. maven

   根据Java环境更改Client/pom.xml文件中的JRE配置，然后在Client目录下执行命令：

```shell
mvn compile exec:java
```



## 功能

- 登录
- 查看数据库、表、属性信息
- 读取sql文件，保存sql文件
- 显示查询结果、执行时间
- 保存查询结果到文件
- 从文件中直接读取sql语句并执行（import操作）

