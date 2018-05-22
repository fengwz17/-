# webchat
先搭建一个BBS论坛，然后加入聊天功能
## 环境配置
### 官网下载MySQL installer
### python配置Django框架
### 安装python包pymysql
  pymysql是Python中操作MySQL的模块，其使用方法和MySQLdb几乎相同。但目前pymysql支持python3.x而后者不支持3.x版本。
  
  修改在django中默认的数据库访问MySQL。
  
  关于Django1.6中DATABASES的设置不用做任何修改，跟MySQLdb一样，settings.py里的配置不变,但是要在项目目录下的__init__.py文件（webchat/webchat/__init__.py）加入下面两句
  
  1  import pymysql
  
  2  pymysql.install_as_MySQLdb()
  
