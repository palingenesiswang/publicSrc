# Android提升规划

## 1.语言基础

#### （1）Java

- 常用数据结构及使用场景
  - ArrayList
  - Vector
  - CopyOnWriteArrayList
  - HashMap
  - ConcurrentHashMap
  - HashTable
- Java虚拟机
  - 内存管理
  - GC回收
  - 类加载
- 多线程
  - 线程池
  - 锁
  - 线程同步
- AOP编程实现
  - JDK动态代理
  - ASM直接操作字节码
  - CGLIB实现
- javassist
  - 字节码加载前直接修改切入方法
  - 注解器APT：DataBinding、ButterKnife、EvenBus3……
- 异常处理
  - 检查性异常
  - 运行时异常处理
- io流及相关
  - 堵塞性IO
  - 非堵塞性IO
- 高级特性
  - 反射
  - 代理
  - 泛型
  - 枚举
  - ~~正则~~
  - jdk 1.8 1.9 1.10 1.11 新特性

#### （2）Kotlin

**优点：**

1. **简洁性:** 提供了很多标准函数，大大减少样板代码的数量。
2. **安全性：**避免空指针异常等错误。
3. **互操作性：**充分利用 JVM、Android 和浏览器的现有库。
4. **工具友好:** 可用任何 Java IDE 或者使用命令行构建。

**特点：**

		1. 函数式编程：let、run、with、apply、also、 Lambda 表达式
  		2. **协程**
  		3. *Kotlin Native：非jvm平台（ios、嵌入式…）支持与C互操作*

---

### 2.Android进阶技术点

- 进程相关

  - 进程原理
  - AIDL原理

- 性能优化及工具

  - 内存
  - CPU
  - 耗电量
  - 网络请求
  - UI布局
  - 线程
  - 数据库

- Android源码相关

  - Binder机制
  - Activity启动流程
  - Handler原理
  - AMS原理
  - PMS原理
  - WMS原理
  - View绘制
  - Touch事件传递机制

- 编译打包流程

  - java/kotlin 源码到最终apk的过程

- 热修复及实现原理

  - 底层替换
  - 类加载
  - instant Run

- 逆向工程原理

  - apk加固方案

- 插件化

  - Hook：注册 Activity 进行占坑，使用占坑 Activity 通过 AMS 验证，还原插件 Activity

- NDK

  - 调用 JNI 以及回调 Java 的方式

- 自定义控件

  - onMeasure，onLayout，onDraw 调用时机， Touch 事件分发机制。

- 动画View Animation

- 属性动画 Proprerty Animation

- WebView js交互：JSBridge……

- **Gradle 的特性以及 DSL 语法**（允许第三方插件在 class 文件转为 dex 文件前操作编译好的 class 文件）

  -  Gradle Transform API 

- 安全

  - HTTPS 通信原理
  - 数据加密方式： MD5，RSA …
  - webview 安全性
  - 代码混淆
  - 数据验签
  - 组件通信安全
  - 服务器通信

- CI持续集成（开发工具）

  - Jenkins 
  - Gitlab CI 

- Sersor传感器

  - 陀螺仪
  - 加速传感器
  - 方向传感器
  - 重力传感器
  - 光线传感器

- *国际化*

- ART、Dalvik虚拟机区别

  -  AOT，Ahead-Of-Time 预编译

- dex文件结构

- 单元测试

  - JUnit4
  - AndroidJUnitRunner
  - Mockito 框架的使用

- 自动化测试

  - Monkey / Monkey Runner 
  - Espresso 
  - UI Automator
  - ……

- 模块开发

  - 分层
  - 模块间跳转通信

- 代码重构（书籍）

  - **《重构改善既有代码的设计》**
  - **《重构与模式》**

- 动态化框架

  -  **App Bundles**

- **Jetpack**

  - foundation

    > 核心系统能力、kotlin扩展、混合dex（multidex）和自动化测试支持的组件

  - Architecture

    > 架构组件帮助管理UI生命周期、数据持久化……

  - Behavior

    > ​	应用程序与标准android服务集成：通知、权限、共享、助手……

  - UI

    > widgets、帮助程序

**常用第三方库**

- 响应式编程：RxJava、RxAndroid，Google 的Agera
- 网络库：Retrofit，OkHttp
- 图片：Fresco，Gilde，Picasso
- 依赖注入：Dagger2
- 数据库：Realm，ORMLite，GreenDAO，ObjectBox
- 数据总线：EventBus，otto
- 内存泄漏检测工具 LeakCanary 等

---

### 3. OOAD 和设计模式

- **面向对象三大特性：**
  - 封装
  - 继承
  - 多态
- **五大基本原则（SOLID 原则）**：
  - 单一职责原则
  - 开放封闭原则
  - 里氏替换原则
  - 依赖倒置原则
  - 接口分离原则

- **设计模式**（常用）：
  - 工厂
  - 单例
  - 适配器
  - 桥接
  - 组合
  - 代理
  - 命令
  - 观察者
  - 策略
  - 状态模式

---

### 4. App架构设计

- MVC
- MVP
- MVVM
- MVI
- VIPER
- Clean Architecture
- Flux

---

### 软技能：**《软技能——代码之外的生存指南》**



