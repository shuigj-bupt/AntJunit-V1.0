# AntJunit-V1.0

jenkins上Ant环境配置
- export mvnhome=/usr/local/apache-maven-3.6.0/bin
- PATH=$PATH:$HOME/bin:$mvnhome
- export ANT_HOME=/usr/local/apache-ant-1.9.13
- PATH=$PATH:$HOME/bin:$ANT_HOME/bin:$mvnhome

# 设置build name 
- 安装 jenkins插件 Build Name Setter + user build var 两个插件
- #${BUILD_NUMBER}-${PROJECT_NAME}-${ENV,var="VARIABLENAME"}-${ENV,var="BUILD_USER"}

在job中配置如下：

jenkins添加该插件后，在job中配置如下

# 目录结构需要修改，文档有错误

![代码结构](https://github.com/zhaoxy8/AntJunit-V1.0/blob/master/Doc/code.png)

# jenkins全局ANT配置
![jenkins全局ANT配置](https://github.com/zhaoxy8/AntJunit-V1.0/blob/master/Doc/Ant.png)

# job配置

![job配置](https://github.com/zhaoxy8/AntJunit-V1.0/blob/master/Doc/jenkins.JPG)
