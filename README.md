# node服务cpu监控工具
## 1.[esay-monitor](https://www.npmjs.com/package/easy-monitor)
node服务cpu监控工具
轻量级的 Node.js 项目内核性能监控 + 分析工具，在默认模式下，只需要在项目入口文件 require 一次，无需改动任何业务代码即可开启内核级别的性能监控分析。

### 特点：
* 服务器状态概览信息展示
* 实时 CPU 函数性能分析，帮助定位程序的性能瓶颈点
* 实时 Memory 堆内内存结构分析，帮助定位到内存疑似泄漏点

### 缺点：
* cpu，Memory 没有历史记录

### 快速开始
npm install easy-monitor

const easyMonitor = require('easy-monitor');
easyMonitor('你的项目名称');
#### 已部署测试环境
测试环境访问地址：http://52.9.161.206:12333/index

使用压测工具压测：开启cpu 分析，得到火焰图，并列出最耗时的5个函数：
[百度]:https://s3-us-west-1.amazonaws.com/imgtest.firmoo.com/images/users/2020/0107/3556853912.png

![Image text](https://raw.githubusercontent.com/hongmaju/light7Local/master/img/productShow/20170518152848.png)





