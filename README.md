## Django2.0-blog 学习
学习 Django2.0 的时候看到 [博主](https://github.com/HaddyYang) 的课程，随后学习中觉得博主的课程十分适合目前的我，所以在此记录学习所敲击的代码～ 

[Django2.0 视频教程地址](https://space.bilibili.com/252028233/#/channel/detail?cid=28138)

### 使用
Python 版本为 `3.8.x`
- 使用虚拟环境  
使用 virtualenv 管理 Python 库

- 安装指定库  
  ```
  pip install -r requirements.txt
  ```

- 创建缓存表  
热门阅读博客排行及缓存提速使用到缓存功能  
  ```
  python manage.py createcachetable
  ```

- 安装 mysqlclient 
  ```
  pip install mysqlclient
  ```
  macOS 安装方式需要参考[官网指引](https://github.com/PyMySQL/mysqlclient-python#macos-homebrew) 
  - 如果安装 mysqlclient 有问题可以选择安装 pymysql (纯 python 开发，可能存在效率问题？？)
    https://blog.csdn.net/Visrul/article/details/81302391

- 数据导入到 mysql 数据库中 (需要提前创建 `mysite_db` 数据库)
  ```
  python manage.py loaddata data.json
  ```

- 启动本地服务
  ```
  python manage.py runserver
  ```