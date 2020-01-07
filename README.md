# node服务cpu监控工具
## 1.[esay-monitor](https://www.npmjs.com/package/easy-monitor)
node服务cpu监控工具
轻量级的 Node.js 项目内核性能监控 + 分析工具，在默认模式下，只需要在项目入口文件 require 一次，无需改动任何业务代码即可开启内核级别的性能监控分析。

### 特点：
* 服务器状态概览信息展示
* 实时 CPU 函数性能分析，帮助定位程序的性能瓶颈点
* 实时 Memory 堆内内存结构分析，帮助定位到内存疑似泄漏点

### 缺点：
* cpu，Memory 没有历史记录，cpu监控和pm2 monit 命令有差别

### 快速开始
npm install easy-monitor

const easyMonitor = require('easy-monitor');
easyMonitor('你的项目名称');
#### 已部署测试环境
测试环境访问地址：http://52.9.161.206:12333/index

#### 1,cpu实时监控
![Image text](https://s3-us-west-1.amazonaws.com/imgtest.firmoo.com/images/users/2020/0107/4227359635.png)

2.cpu分析火焰图
使用压测工具压测：开启cpu 分析，得到火焰图，并列出最耗时的5个函数：
![Image text](https://s3-us-west-1.amazonaws.com/imgtest.firmoo.com/images/users/2020/0107/3556853912.png)

#### 3.内存泄漏检测：
![Image text](https://s3-us-west-1.amazonaws.com/imgtest.firmoo.com/images/users/2020/0107/3064481883.png)

## 1.[pm2官方监控](https://app.pm2.io/bucket/5e1417080b29039111e044b3/backend/overview/servers)
 #### 1.创建项目
 ![Image text](https://s3-us-west-1.amazonaws.com/imgtest.firmoo.com/images/users/2020/0107/1308208061.png)
 
 #### 2.修改dockerfile 和容器环境变量
 ![Image text](https://s3-us-west-1.amazonaws.com/imgtest.firmoo.com/images/users/2020/0107/2427202519.png)
 
 #### 3.启动容器，查看监控页面
 ![Image text](https://s3-us-west-1.amazonaws.com/imgtest.firmoo.com/images/users/2020/0107/4116958480.png)
 ![Image text](https://s3-us-west-1.amazonaws.com/imgtest.firmoo.com/images/users/2020/0107/1626597578.png)
 
 ##### 免费版只能建立4个项目，平台给的权限如下：
 ![Image text](https://s3-us-west-1.amazonaws.com/imgtest.firmoo.com/images/users/2020/0107/1019297983.png)
 
 ##### 收费版功能比较全面，能看到历史记录等，大体功能如下：
 
 ![Image text](https://s3-us-west-1.amazonaws.com/imgtest.firmoo.com/images/users/2020/0107/2779724437.png)
  
  

