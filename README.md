# 目标
简单地实现爬取静态网页数据并保存到本地数据库，为进一步数据分析做准备
# 环境与工具
**ubuntu 12.04 LTS**,**mysqld 5.5**，**python3.6**及以下库：**requests**、**re**、**pymysql**、**pandas**
# 准备工作
- 安装**mysql**：
`sudo apt-get install mysql-server mysql-client`
- 开启**mysql**服务：
- 因为以后要做数据分析，所以**pandas**包是很有必要的，另外需要先安装相关的依赖包：
`sudo -H pip install pandas`
# 代码实现
代码来自[一个咸鱼的Python爬虫之路（四）：将爬取数据存入mysql - FRANKLV - 博客园](https://www.cnblogs.com/franklv/p/6911061.html),只是我用**jupyter notebook**来作交互，修改了其中本地数据库的相关配置，要让配置能正确有效，需要操作一下本地**mysql**数据库,具体参考[ubuntu 下MySQL基本操作 - 简书](https://www.jianshu.com/p/7a0f4625698e)

这里简单的爬取淘宝上咖啡的价格数据，只用到**requests**模块和一些简单的正则表达式就能输出比较优美的数据表来，当然并不能满足更为庞杂动态数据挖掘的要求，权当作为入门引子
