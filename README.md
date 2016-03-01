# MonkeyJoker_IOS

***
## README版本更新概况
* 2016.03.1 项目结构暂定


---
### 分支管理策略
* master——发布版本分支
* develop——开发版本分支
* xxx——自命名分支

>平常的功能模块开发push到自己的自命名分支，待完成时merge到develop分支
阶段性开发完成再将develop分支merge到master


* * *

## 项目目录结构
##### 初步结构

* Application   --- AppDelegate和一些系统常量及系统配置文件以及宏定义
* Base   --- 一些基本父类，包括父ViewController和一些公用顶层自定义父类
* Handler   --- 系统业务逻辑层，负责处理系统复杂业务逻辑
* Storage   --- 简单数据存储，主要是一些键值对存储及系统外部文件的存取，包括对NSUserDefault和plist存取的封装
* Network   --- 网络处理层，封装了基于AFNetworking的网络处理层，通过block实现处理结果的回调
* Database   --- 数据层，封装基于FMDB的sqlite数据库存取和管理，对外提供基于Model层对象的调用接口，封装对数据的存储过程。
* Utils   --- 系统工具类，主要放置一些系统常用工具类
* Categories --- 类别，对现有系统类和自定义类的扩展
* Resource   --- 资源库，包括图片，plist文件等
* Sections   --- app的具体模块
- xxx（模块）
- Controller --- 系统控制层，放置ViewController
- View --- 视图层，代码写的视图均放在这里
- Model --- 系统中的实体，通过类来描述系统中的一些角色和业务