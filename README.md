# node服务cpu监控工具
## 1.[esay-monitor](https://www.npmjs.com/package/easy-monitor)
node服务cpu监控工具
轻量级的 Node.js 项目内核性能监控 + 分析工具，在默认模式下，只需要在项目入口文件 require 一次，无需改动任何业务代码即可开启内核级别的性能监控分析。

### 特点：
* 服务器状态概览信息展示
* 实时 CPU 函数性能分析，帮助定位程序的性能瓶颈点
* 实时 Memory 堆内内存结构分析，帮助定位到内存疑似泄漏点

### 快速开始
npm install easy-monitor

const easyMonitor = require('easy-monitor');
easyMonitor('你的项目名称');



