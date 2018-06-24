## ubuntu下apt安装
```
sudo apt install maven
```

## 下载Maven

1. 打开Maven官网下载页面：http://maven.apache.org/download.cgi
下载:apache-maven-3.5.0-bin.tar.gz

1. 解压下载的安装包到某一目录，比如：/Users/yuanweipeng/Documents/maven

## 配置环境变量

打开terminel输入以下命令：
```
vi ~/.zshrc
```

在次文件中添加设置环境变量的命令:
```
export M2_HOME=/Users/yuanweipeng/Documents/maven/apache-maven-3.5.0
export PATH=$PATH:$M2_HOME/bin
```

添加之后保存并推出，执行以下命令使配置生效：
```
source ~/.zshrc
```

## 查看配置是否生效

输入：mvn -v命令，输出如下：
```
Apache Maven 3.5.0 (ff8f5e7444045639af65f6095c62210b5713f426; 2017-04-04T03:39:06+08:00)
Maven home: /Users/yuanweipeng/Documents/maven/apache-maven-3.5.0
Java version: 1.8.0_121, vendor: Oracle Corporation
Java home: /Library/Java/JavaVirtualMachines/jdk1.8.0_121.jdk/Contents/Home/jre
Default locale: zh_CN, platform encoding: UTF-8
OS name: "mac os x", version: "10.12.6", arch: "x86_64", family: "mac"
```

则配置成功。