# PNP Collection



## Android Framework Power变迁史

- Android K

  Android 4.4 针对硬件传感器批处理引入平台支持，这是一项新的优化功能，可以显著降低传感器持续活动所消耗的电量。

- Android L

  新增的 Job Scheduling API 允许您通过将作业推迟到稍后或指定条件下（如设备充电或连入 WLAN 时）运行来优化电池寿命。

  新增的 dumpsys batterystats 命令可生成电池使用情况统计信息，您可通过它了解整个系统的耗电情况，以及了解您的应用对设备电池的影响。

  新增了“电池耗电历史”工具，可将来自 dumpsys batterystats 的统计数据转换成可视化格式，以便进行与电池有关的调试。您可以在 https://github.com/google/battery-historian 上找到该工具

- Android M

  Optimize for Doze and App Standby 

- Android N

  Android 6.0 推出了低电耗模式，即设备处于空闲状态时，通过推迟应用的 CPU 和网络活动以实现省电目的的系统模式，例如，设备放在桌上或抽屉里时。

  现在，在 Android 7.0 中，低电耗模式又前进了一步，随时随地可以省电。只要屏幕关闭了一段时间，且设备未插入电源，低电耗模式就会对应用使用的 CPU 和网络限制。这意味着用户即使将设备放入口袋里也可以省电。

  Project Svelte：后台优化

- Andorid O

  后台执行限制 

  Android 8.0 引入了对 JobScheduler 的多项改进。由于您通常可以使用计划作业替代现在受限的后台服务或隐式广播接收器，这些改进可以让您的应用更轻松地符合新的后台执行限制。

- Android P

  Android 9（API 级别 28）引入了一些新功能来改进设备电源管理。 这些变化，连同先前版本中已经存在的功能，有助于确保将系统资源提供给最需要它们的应用。

  电源管理功能可以分为两个类别：

  应用待机群组
  系统将根据用户的使用模式限制应用对 CPU 或电池等设备资源的访问。 这是 Android 9 中新增的一项功能。
  省电模式改进
  开启省电模式后，系统会对所有应用施加限制。 这是一项已有的功能，但在 Android 9 中得到了改进。
  注：这些变化适用于所有应用，无论它们是否以 Android 9 为目标。

- Android Q

  深色主题

- Android R

  在 Android 11 中使用 NDK Thermal API 监控设备上的温度变化，然后采取相应措施以降低耗电量和设备温度。该 API 类似于Java Thermal API；您可以使用它接收任何热状态更改的通知或直接轮询当前状态。

  Frame rate API（VRR）
  Android 11 提供了一个 API，可让应用告知系统其预期帧速率，从而减少支持多个刷新率的设备上的抖动。有关如何使用此 API 的信息，请参阅帧速率指南。

- Android S

  前台服务启动限制



[深入探索 Android 电量优化](https://juejin.cn/post/6844904195523346439)

[Android 功耗分析方法和优化](https://www.cnblogs.com/linhaostudy/p/13610236.html)

[Android功耗改进](https://paul.pub/android-power/)



## Goolge Power Config

[Android Power Config](https://source.android.com/devices/tech/power?hl=zh-cn)



## Linux电源管理

[All](http://zhannei.baidu.com/cse/search?s=16798210514584749375&entry=1&q=Linux%E7%94%B5%E6%BA%90%E7%AE%A1%E7%90%86)

[整体架构](http://www.wowotech.net/pm_architecture.html)

[Generic PM之基本概念和软件架构](http://www.wowotech.net/linux_kenrel/generic_pm_architecture.html)

[runtime_pm.txt](https://android.googlesource.com/kernel/mediatek/+/android-mediatek-pike-3.10-marshmallow-mr1-wear-release/Documentation/power/runtime_pm.txt)

[Android电源管理基础知识整理](https://www.jianshu.com/p/0a19e6f7ad02)

[The Linux kernel user’s and administrator’s guide - Power Management](https://www.kernel.org/doc/html/v4.18/admin-guide/pm/index.html)

[Deep understanding of Linux kernel process sleep](https://cdmana.com/2021/08/20210812125803967c.html)



## Doze/Device Idle Controller

[Android 8.1 Doze模式分析(一)——Doze简介和DeviceIdleController的启动](https://blog.csdn.net/FightFightFight/article/details/81348088)

[Android 8.1 Doze模式分析（二）对网络的限制](https://blog.csdn.net/liu362732346/article/details/86573585?utm_medium=distribute.pc_relevant.none-task-blog-2%7Edefault%7EBlogCommendFromMachineLearnPai2%7Edefault-12.control&depth_1-utm_source=distribute.pc_relevant.none-task-blog-2%7Edefault%7EBlogCommendFromMachineLearnPai2%7Edefault-12.control)

[Android 8.1 Doze模式分析(二)——Light Doze模式](https://blog.csdn.net/FightFightFight/article/details/81366285?utm_medium=distribute.pc_relevant.none-task-blog-2%7Edefault%7EBlogCommendFromMachineLearnPai2%7Edefault-1.control&depth_1-utm_source=distribute.pc_relevant.none-task-blog-2%7Edefault%7EBlogCommendFromMachineLearnPai2%7Edefault-1.control)

[Android 8.1 Doze模式分析（三）Light Doze模式流程分析](https://blog.csdn.net/liu362732346/article/details/86580670?utm_medium=distribute.pc_relevant.none-task-blog-2%7Edefault%7EBlogCommendFromBaidu%7Edefault-6.control&depth_1-utm_source=distribute.pc_relevant.none-task-blog-2%7Edefault%7EBlogCommendFromBaidu%7Edefault-6.control)

[Android 8.1 Doze模式分析(三)——Deep Doze模式](https://blog.csdn.net/FightFightFight/article/details/81367516?utm_medium=distribute.pc_relevant.none-task-blog-2%7Edefault%7EBlogCommendFromMachineLearnPai2%7Edefault-15.control&depth_1-utm_source=distribute.pc_relevant.none-task-blog-2%7Edefault%7EBlogCommendFromMachineLearnPai2%7Edefault-15.control)

[Android 8.1 Doze模式分析（三）释放WakeLock](https://blog.csdn.net/liu362732346/article/details/86577388?utm_medium=distribute.pc_relevant.none-task-blog-2~default~baidujs_title~default-0.control&spm=1001.2101.3001.4242)

[Android 8.1 Doze模式分析(四)——Doze模式的退出](https://blog.csdn.net/FightFightFight/article/details/81391900?utm_medium=distribute.pc_relevant.none-task-blog-2%7Edefault%7EBlogCommendFromBaidu%7Edefault-10.control&depth_1-utm_source=distribute.pc_relevant.none-task-blog-2%7Edefault%7EBlogCommendFromBaidu%7Edefault-10.control)

[Android 8.1 Doze模式分析(五) Doze白名单及Debug方式](https://blog.csdn.net/FightFightFight/article/details/81392488?utm_medium=distribute.pc_relevant.none-task-blog-2~default~baidujs_title~default-5.control&spm=1001.2101.3001.4242)

[Android 8.1 Doze模式分析（五）Doze对Alarm的限制](https://blog.csdn.net/liu362732346/article/details/86596525?utm_medium=distribute.pc_relevant.none-task-blog-2%7Edefault%7EBlogCommendFromMachineLearnPai2%7Edefault-14.control&depth_1-utm_source=distribute.pc_relevant.none-task-blog-2%7Edefault%7EBlogCommendFromMachineLearnPai2%7Edefault-14.control)

[说说安卓6.0的Doze和App Standby功能](https://cn.apkjam.com/6ds.html)

[Doze模式详解](https://www.jianshu.com/p/8e243193d1a4)

[Doze模式第 1 篇 - DeviceIdleController的启动](https://lishuaiqi.top/2017/10/01/Doze1-deviceIdleControllerStartProcess/#2-2-DeviceIdleController-readConfigFileLocked)

[Doze模式第 2 篇 - DeviceIdleController 动态机制](https://lishuaiqi.top/2017/11/25/Doze2-deviceIdleControllerDynamic/)

[Doze专题](https://chendongqi.me/tags/#Doze)

[Android Doze模式源码分析](https://www.cnblogs.com/l2rf/p/6373794.html)

[Doze Sensing AnyMotionDetector运动检测机制](https://wwmmyy.github.io/2017/02/15/Doze-Sensing%E8%BF%90%E5%8A%A8%E6%A3%80%E6%B5%8B%E6%9C%BA%E5%88%B6/)

[android 6.0的DozeMode低功耗模式 及 引起的程序保活問題（一）](https://www.itread01.com/content/1550193133.html)

[安卓 省电模式、低电耗(Doze)模式、应用待机(standby)模式、唤醒锁](https://www.daimajiaoliu.com/daima/4796b8511900400)

[Android Doze模式适配实验记录](https://blog.csdn.net/gaoxiaoweiandy/article/details/95778748)



- *Making Job Scheduler into a Mainline Module* - DeviceIdleController

  JS service side classes are put in `service-jobscheduler.jar`. It's *not* included in services.jar, and instead it's put in the system server classpath, which currently looks like the following: `SYSTEMSERVERCLASSPATH=/system/framework/services.jar:/system/framework/ethernet-service.jar:/system/framework/com.android.location.provider.jar:/system/framework/service-jobscheduler.jar`

  `SYSTEMSERVERCLASSPATH` is generated from `PRODUCT_SYSTEM_SERVER_JARS`.

  JS framework side classes are put in `framework-jobscheduler.jar`, and the rest of the framework code is put in `framework-minus-apex.jar`, as of http://ag/9145619.

  However these jar files are *not* put on the device. We still generate `framework.jar` merging the two jar files, and this jar file is what's put on the device and loaded by Zygote.



## Android 8.1 PowerManagerService分析

[Android 8.1 PowerManagerService分析(一)](https://blog.csdn.net/FightFightFight/article/details/79532191)

[Android 8.1 PowerManagerService分析(二) ——updatePowerStateLocked()方法](https://blog.csdn.net/FightFightFight/article/details/80341728?utm_medium=distribute.pc_relevant.none-task-blog-2%7Edefault%7EBlogCommendFromMachineLearnPai2%7Edefault-4.essearch_pc_relevant&depth_1-utm_source=distribute.pc_relevant.none-task-blog-2%7Edefault%7EBlogCommendFromMachineLearnPai2%7Edefault-4.essearch_pc_relevant)

[Android 8.1 PowerManagerService分析(三)——WakeLock机制](https://blog.csdn.net/FightFightFight/article/details/79733559?utm_medium=distribute.pc_relevant.none-task-blog-2~default~baidujs_utm_term~default-0.essearch_pc_relevant&spm=1001.2101.3001.4242)

[Android 8.1 PowerManagerService分析(四)——亮屏流程分析](https://blog.csdn.net/FightFightFight/article/details/79808100)

[Android 8.1 PowerManagerService分析(五)——灭屏流程分析](https://blog.csdn.net/FightFightFight/article/details/81192495)



## WakeLock

[Android 8.1 PowerManagerService分析(三)——WakeLock机制](https://blog.csdn.net/FightFightFight/article/details/79733559?utm_medium=distribute.pc_relevant.none-task-blog-2~default~baidujs_utm_term~default-0.essearch_pc_relevant&spm=1001.2101.3001.4242)

[Android Q之后hal针对wakelock的机制变化](https://juejin.cn/post/6947092185930350622)

[SystemSuspend Service](https://source.android.com/devices/architecture/systemsuspend?hl=zh-cn)

[从Android应用层及Framework层的角度分析WakeLock锁机制](https://bbs.huaweicloud.com/blogs/212620)

[Android wakelock && suspend](https://www.codenong.com/cs109321108/)

[Android R PowerManagerService模块(2) WakeLock机制](https://juejin.cn/post/6947092185930350622)

[Linux Kernel and Android 休眠与唤醒(中文版)](http://www.thinksrc.com/2010/04/18/suspend-cn.html#sec-1)

[唤醒锁: 检测 Android* 应用中的 No-Sleep（无法进入睡眠）问题](https://yuanwei.blog.csdn.net/article/details/50868341)



## Android App Standby

[Android9.0 应用待机群组](https://blog.csdn.net/kc58236582/article/details/82018654)

[Android P 应用分组介绍](https://github.com/lqktz/document/blob/master/android_doc/App_Standby_Bucket.md)

[Android UsageStatsService（应用使用统计服务）的学习与调研](https://www.jianshu.com/p/c99b008ff2ef)

[Android UsageStatsService：要点解析](https://blog.csdn.net/wuqingyidongren/article/details/53306162)

[UsageStats使用状态管理](https://lishuaiqi.top/tags/UsageStats%E4%BD%BF%E7%94%A8%E7%8A%B6%E6%80%81%E7%AE%A1%E7%90%86/)



## Android 8.1 Battery系列

[Android 8.1 Battery系列(一) BatteryService分析](https://blog.csdn.net/FightFightFight/article/details/82353373)

[Android 8.1 Battery系列(二) BatteryStatsService分析](https://blog.csdn.net/FightFightFight/article/details/82384336)

[Android 8.1 Battery系列(三) PowerProfile和power_profile.xml](https://blog.csdn.net/FightFightFight/article/details/82428483)

[9月](https://blog.csdn.net/FightFightFight/article/month/2018/09)

[Android 电源管理之电池管理系统(BMS)](http://huaqianlee.github.io/2017/11/21/Android/BMS-of-Android-Power-Management/)

[Android10.0电源框架源码分析](http://www.cjcbill.com/2020/03/01/battery-frame/)

[BatteryService及BatteryStatsService分析](https://www.kancloud.cn/alex_wsc/android-deep2/413468)

[Android 电池管理系统解析](https://blog.csdn.net/madannasf/article/details/105199234)



## Battery Saver Mode

[Use Battery Saver on a Pixel phone](https://support.google.com/pixelphone/answer/6187458?hl=en)

[How to Enable Extreme Battery Saver on Google Pixel](https://gadgetstouse.com/blog/2020/10/08/enable-extreme-battery-saver-on-google-pixel/)

[AndroidO Battery saver省电助手实现原理](https://blog.csdn.net/yun_hen/article/details/78143442)

[Android P 省电模式(LowPowerMode)(二) ------ 省电行为](https://www.jianshu.com/p/5c732a446495/)

[Android 省电模式自定义，打造更适合自己的长续航体验](https://sspai.com/post/67475)

[Android powersave模式网络限制流程](https://blog.csdn.net/b178903294/article/details/115397093)

[Android 8.1省电模式分析](https://blog.csdn.net/weixin_39352694/article/details/86298908)

[Xiaomi "Ultra Battery saver"](https://community.kaspersky.com/kaspersky-safe-kids-16/xiaomi-ultra-battery-saver-disables-safe-kids-14770)

[How to customize Android’s built-in battery saver mode](https://www.xda-developers.com/customize-android-battery-saver-mode/)



## AlarmManagerService

[AlarmManager深入分析](https://www.cnblogs.com/muhuacat/articles/5261081.html)

[Linux fd 系列 — 定时器 timerfd 是什么？](https://www.modb.pro/db/100208)

[AlarmThread 触发流程](https://www.jianshu.com/p/d75810c1fa9e)

[理解AlarmManager机制](http://gityuan.com/2017/03/12/alarm_manager_service/)

[AlarmManager第 2 篇 - set Alarm 流程分析](https://lishuaiqi.top/2017/07/25/AlarmManager2-setAlarm/#1-AlarmManager-setAlarm)

[AlarmManager闹钟管理](https://lishuaiqi.top/categories/AndroidFramework%E6%BA%90%E7%A0%81%E5%88%86%E6%9E%90/AlarmManager%E9%97%B9%E9%92%9F%E7%AE%A1%E7%90%86/)



## Android 8.1 DisplayPowerController

[Android 8.1 DisplayPowerController(一) 亮灭屏流程](https://blog.csdn.net/FightFightFight/article/details/81320519)



## AppHibernationService

[(A12新增)](https://cs.android.com/android/platform/superproject/+/master:frameworks/base/services/core/java/com/android/server/apphibernation/AppHibernationService.java;l=1;bpv=1) 

System service that manages app hibernation state, a state apps can enter that means they are not being actively used and can be optimized for storage. The actual policy for determining if an app should hibernate is managed by PermissionController code.



## PowerStatsService

[A12新增](http://aospxref.com/android-12.0.0_r3/xref/frameworks/base/services/core/java/com/android/server/powerstats/PowerStatsService.java)

This class provides a system service that estimates system power usage per subsystem (modem, wifi, gps, display, etc) and provides those power estimates to subscribers.



## 关键技术

[应用功耗优化](https://www.jianshu.com/p/c7e871677610)

[使用Android vitals提升app性能和质量](https://zhuanlan.zhihu.com/p/40571031)

[【Android Developer】性能和功耗](https://developer.android.com/topic/performance?hl=zh-cn)

[Android Framework 框架系列之 MTK 功耗解决方案](https://daimajiaoliu.com/daima/61061631e498404)

[MTK平台待机功耗分析流程](https://kknews.cc/digital/v5lapmy.html)

[手机功耗测试指南](https://segmentfault.com/a/1190000024546990)

[功耗问题处理指南](https://www.cnblogs.com/wangjie1990/p/11327614.html)

[Android进程永生技术终极揭秘：进程被杀底层原理、APP应对被杀技巧](https://cloud.tencent.com/developer/article/1591535)

[Android功耗改进](https://paul.pub/android-power/)

[Android后台调度任务与省电](https://www.ktanx.com/blog/p/4827)



## CPU & Memory

[Part 1: RAM](https://chanjarster.github.io/post/kernel/know-memory-ram/)

[Part 2: CPU caches](https://chanjarster.github.io/post/kernel/know-memory-cpu-cache/)

[Part 3: Virtual Memory](https://chanjarster.github.io/post/kernel/know-memory-cpu-virtual-memory/)

[Part 4: NUMA support](https://chanjarster.github.io/post/kernel/know-memory-cpu-numa-support/)



## IC相关

[低功耗设计基础：DVS, AVS和DVFS都是如何降低功耗的？](https://zhuanlan.zhihu.com/p/270671041)



## Thermal

 [Thermal 框架梳理](https://dongka.github.io/2018/06/25/thermal/thermal_framework/)

[Android/Linux Thermal框架分析及其Governor对比](Android/Linux Thermal框架分析及其Governor对比)

[Android 热缓解框架解析](https://blog.csdn.net/feelabclihu/article/details/107873407)

[性能or低温？-- Thermal温升机制](https://zhuanlan.zhihu.com/p/64431532)



## Tencent Matrix

[Tencent Matrix介绍](https://github.com/Tencent/matrix#matrix_android_cn )

Matrix is an APM (Application Performance Manage) used in Wechat to monitor, locate and analyse performance problems. It is a plugin style, non-invasive solution and is currently available on iOS, macOS and Android.



## 性能

[那些年，我们一起经历过的 Android 系统性能优化](http://tinylab.org/android-perf-optimize-solutions-of-mobile-manufacturers/)

[Android性能优化（一）之启动加速35%](https://juejin.cn/post/6844903459951476744)

[CPU体系架构-MMU](https://nieyong.github.io/wiki_cpu/CPU%E4%BD%93%E7%B3%BB%E6%9E%B6%E6%9E%84-MMU.html)

[CPU体系架构-ARM/MIPS/X86](https://nieyong.github.io/wiki_cpu/index.html)

[细说Cache-L1/L2/L3/TLB](https://zhuanlan.zhihu.com/p/31875174)

[沧浪之水：Android上的FreeSync(上、中、下)](https://zhuanlan.zhihu.com/p/217298155)



## Cached App Optimizer

App Compact

App Freezer



Android系统中默认关闭

​    @VisibleForTesting static final Boolean DEFAULT_USE_COMPACTION = false;

​    @VisibleForTesting static final Boolean DEFAULT_USE_FREEZER = false;



## Android电池电量管理

[Android App 电量统计原理与优化](http://www.androidos.net.cn/doc/2021/8/4/839.html)

[Android耗电统计算法](http://gityuan.com/2016/01/10/power_rank/)



## Jobscheduler service

[深入理解JobScheduler与JobService的使用](https://juejin.cn/post/6951224625095245861)

[JobScheduler源码探究](https://blog.csdn.net/allisonchen/category_7436117.html)



## Android性能专项测试

[Android性能专项测试](https://www.kancloud.cn/digest/itfootballprefermanc/100904)



## IOS 功耗

[iOS性能优化之耗电量](https://juejin.cn/post/6844903695755247624)

[iOS进阶--App功耗优化看这篇就够了](http://www.cocoachina.com/articles/21428)

[Energy Efficiency and the User Experience](https://developer.apple.com/library/archive/documentation/Performance/Conceptual/EnergyGuide-iOS/)

[IOS Power Manager 2.0](https://developer.apple.com/library/archive/technotes/tn/tn1190.html#//apple_ref/doc/uid/DTS10003029)

[Power Management & The Energy Saver API](https://developer.apple.com/library/archive/technotes/tn/tn1086.html#//apple_ref/doc/uid/DTS10002927)

[Performance Overview](https://developer.apple.com/library/archive/documentation/Performance/Conceptual/PerformanceOverview/Introduction/Introduction.html#//apple_ref/doc/uid/TP40001410)

[Improving Your App's Performance](https://developer.apple.com/documentation/metrickit/improving_your_app_s_performance/)

[iOS-Performance-Optimization](https://github.com/skyming/iOS-Performance-Optimization/blob/master/README.md)



## IO

[彻底搞懂 IO 底层原理](https://mp.weixin.qq.com/s/9UIiEfPKxKRYxY366QqQoQ)



## 芯片知识

[IP](https://baijiahao.baidu.com/s?id=1704133260569135703&wfr=spider&for=pc)

[细说Cache-L1/L2/L3/TLB](https://zhuanlan.zhihu.com/p/31875174)

[到底什么是Cortex、ARMv8、arm架构、ARM指令集、soc？一文帮你梳理基础概念](https://developer.51cto.com/art/202010/628945.htm)



## MPAM

[CPU共享资源隔离的利器MPAM特性介绍](http://www.elecfans.com/d/1581957.html)

[openEuler 21.03 特性解读 | CPU 共享资源隔离的利器 - MPAM](https://cloud.tencent.com/developer/article/1816451)



## GPU

[CPU架构和GPU分类详解](http://ee.mweda.com/rd/184844_2.html)

[Adreno](https://developer.qualcomm.com/software/adreno-gpu-sdk/gpu)

[Mali](https://developer.arm.com/ip-products/graphics-and-multimedia/mali-gpus)

PowerVR

NVIDIA GeForce ULP

AMD Radeon™ RX Graphics Cards

Vivante GCXX系列GPU



## CPU



OP4E3F:/sys/devices/system/cpu/cpu0/cpufreq # ls -l



## Linux内核启动流程

[linux内核启动流程](https://blog.csdn.net/perfect1t/article/details/81741531)

Linux5.15 

**Cpu driver 载入流程：**

内核引导程序 --> start_kernel --> arch_call_rest_init --> rest_init --> kernel_thread(kernel_init, NULL, CLONE_FS) --> kernel_init --> kernel_init_freeable --> --> do_basic_setup --> driver_init --> cpu_dev_init

**Android init启动流程：**

内核引导程序 --> start_kernel --> arch_call_rest_init --> rest_init --> kernel_thread(kernel_init, NULL, CLONE_FS) --> kernel_init --> **run_init_process** --> kernel_execve

**CPU Hotplug 启动流程**

内核引导程序 --> start_kernel --> arch_call_rest_init --> rest_init --> kernel_thread(kernel_init, NULL, CLONE_FS) --> kernel_init --> kernel_init_freeable --> --> do_basic_setup --> driver_init --> cpu_dev_init

cpu subsys -- > subsys_system_register

cpu_dev_register_generic



[cpu-freq / governors.txt](https://android.googlesource.com/kernel/common/+/a7827a2a60218b25f222b54f77ed38f57aebe08b/Documentation/cpu-freq/governors.txt)

[【原创】Linux cpufreq framework](https://www.cnblogs.com/LoyenWang/p/11385811.html)

[【原创】Linux cpuidle framework](https://www.cnblogs.com/LoyenWang/p/11379937.html) 



[Linux CPU core的电源管理(1)_概述](http://www.wowotech.net/pm_subsystem/cpu_core_pm_overview.html)

[Linux CPU core的电源管理(2)_cpu topology](http://www.wowotech.net/pm_subsystem/cpu_topology.html)

[Linux CPU core的电源管理(3)_cpu ops](http://www.wowotech.net/pm_subsystem/cpu_ops.html)

[ARM64 SMP多核启动（上）-　spin-table](https://cloud.tencent.com/developer/article/1857514?from=article.detail.1857516)

[ARM64 SMP多核启动（下）-　PSCI](https://cloud.tencent.com/developer/article/1857516?from=15425)

[Linux CPU core的电源管理(5)_cpu control及cpu hotplug](http://www.wowotech.net/pm_subsystem/cpu_hotplug.html)



[Linux cpufreq framework(1)_概述](http://www.wowotech.net/pm_subsystem/cpufreq_overview.html)

[Linux cpufreq framework(2)_cpufreq driver](http://www.wowotech.net/pm_subsystem/cpufreq_driver.html)

[linux cpufreq framework(3)_cpufreq core](http://www.wowotech.net/pm_subsystem/cpufreq_core.html)

[linux cpufreq framework(4)_cpufreq governor](http://www.wowotech.net/pm_subsystem/cpufreq_governor.html)

[linux cpufreq framework(5)_ARM big Little driver](http://www.wowotech.net/pm_subsystem/arm_big_little_driver.html)



[Linux电源管理(15)_PM OPP Interface](http://www.wowotech.net/pm_subsystem/pm_opp.html)



[Linux电源管理-wakelock](https://cloud.tencent.com/developer/article/1603945)

[Linux电源驱动-Linux Cpuidle Framework](https://cloud.tencent.com/developer/article/1603973)

[ARM64 SMP多核启动（上）-　spin-table](https://cloud.tencent.com/developer/article/1857514?from=article.detail.1857516)

[ARM64 SMP多核启动（下）-　PSCI](https://cloud.tencent.com/developer/article/1857516?from=15425)

[Linux电源管理-Linux regulator framework概述](https://cloud.tencent.com/developer/article/1603958)

[Linux电源管理-Linux Regulator Framework代码分析](https://cloud.tencent.com/developer/inventory/921/article/1603596)

kernel/power/energy_model.c

kernel/sched/

CPU QOS

[Linux PM_QoS介绍](https://blog.csdn.net/feelabclihu/article/details/116810959)

[Linux PM QoS framework(1)_概述和软件架构](http://www.wowotech.net/pm_subsystem/pm_qos_overview.html)

[DMA之理解](https://blog.csdn.net/zhejfl/article/details/82555634)

[DMA详解](https://www.jianshu.com/p/b19a7c46f465)

[一文了解MIPI 协议中的SPMI接口介绍](https://blog.csdn.net/kaibi8239/article/details/115111414)



## SMP/AMP/HMP

SMP——Symmetric Multi-Processing ，对称多处理器结构

AMP——Asymmetric Multi-Processing ，非对称多处理器结构

HMP——Heterogeneous Multi-Processing，混合架构



SMP：对称架构，同架构的多核芯跑同一个OS。比如4个A53跑同一个linux系统。

AMP：异构系统，多核跑多个OS，比如一个核跑RTOS，另外一个核跑linux

HMP：混合架构，不同架构的多核跑一个OS，比如2个A72核＋2个A53的核，但是跑一个linux系统。



## Battery Historian

[Battery Bugreport](https://bathist.ef.lc/)

在 https://bathist.ef.lc/ 网站上直接加载log解析，不需要配置本地环境

bugreport抓取方法

测试前
adb shell dumpsys batterystats --reset                  //重置电池的历史统计数据，进行全新收集
adb shell dumpsys batterystats --enable full-wake-history  //通过该命令，获取带有具体时间线的电池使用的详细的数据

adb shell dumpsys alarm > ./alarm1.txt

拔掉USB

测试后：
adb shell bugreport > bugreport.txt

adb shell dumpsys alarm > ./alarm2.txt

关闭全量唤醒报告
adb shell dumpsys batterystats —disable full-wake-history



参数说明

CPU running: CPU运行状态，是否被唤醒。                                                                                                                                                                  

Kernel only uptime: 只有内核运行时间。

Userspace wakelock:该属性是记录Android中PowerManagerService的wake_lock模块的工作时间。是否有停止的时候等。(ps：系统为了节省电量，CPU在没有任务忙的时候就会自动进入休眠。有任务需要唤醒CPU高效执行的时候，就会给CPU加wake_lock锁）                                                           

Top app: 该栏显示当前时刻哪个app处于最上层，就是当前手机运行的app（用来判断某个app对手机电量的影响，这样也能判断出该app的耗电量信息。该栏记录了应用在某一个时刻启动，以及运行的时间，这对我们比对不同应用对性能的影响有很大的帮助）。

Screen: 屏幕是否点亮。这一点，可以用于考虑睡眠状态和点亮状态下电量的使用信息。                                                                                            

Activity Manager Proc:活跃的用户进程。                            

Doze:是否进入doze模式                                                                                                                                                                                                  

Device active:和Doze相反

Phone call: 是否发生打电话事件。                                                                                                                                                                                 

GPS: 是否有调度GPS的事件。

JobScheduler: 发生Job Scheduler的事件，异步作业调度。                                                                                                                                         

SyncManager: 发生Sync事件，同步操作。                                                                                                 

Phone scanning: 手机是否在扫描手机信号网络。                                                                                                                                                         

Phone state: 手机电话状态，in（有数据网络）/out（无数据网络）/off(飞行模式)两种。

Network connectivity: 数据网络连接类型， 有TYPE_MOBILE和TYPE_WIFI。                                                                                                               

Mobile network type: 网络信号类型，比如edge/hspa/hspap/none，none表示无信号。

Mobile radio active: 表明手机是否有信号，空白表明手机无信号。移动蜂窝信号 BP侧耗电                                                                                       

Mobile signal strength: 手机信号强度，有great/good/moderate/poor/none五种等级。                               

Wifi full lock: 持有Wifi full lock的事件。                                                                                                                                                                       

Wifi scan: 是否有Wifi 扫描网络的事件。

Wifi supplicant: 是否有wifi请求。                                                                                                                                                                                  

Wifi radio: 是否正在通过wifi传输数据。             

Wifi signal strength: wifi信号强度（great\good\moderate\poor）。                                                                                                                          

Wifi on: 是否开启wifi。

Wifi running:wifi组件是否在工作(未传输数据)                                                                                                                                                               

Health:电池健康状态的信息，这个信息一定程度上反映了这块电池使用了多长时间。这一栏记录电池状态在何时发生改变。

Audio: 是否有使用audio模块。                                                                                                                                                                                       

Video: 是否有使用video模块

Foreground process: 前台进程。                                                                                                                                                                                   

Temperature: 手机电池温度。  

Battery level: 电量，可以看出电量的变化。                                                                                                                                                                 

Plugged: 是否有插充电器或者usb。

Crashes(Logcat): 某个时间点出现crash的应用。                                                                                                                                                           

Logcat misc:是否在导日志



System Status/History Stats/App Stats窗口说明

**System Status** 

   System Stats主要有Duration/Realtime，Metric，Device’s Power Estimates，Userspace Wakelocks，SyncManager Syncs，Mobile Radio Activity Per App，Mobile Traffic Per App，WiFi Scan Activity Per App，WiFi Full Lock Activity Per App，Kernel Wakesources，Kernel Wakeup Reasons，  App Wakeup Alarms，GPS Use By App这些小类型，这些都是描述系统相关的特性。   

| 类型                            | 说明                                                         |      |
| ------------------------------- | ------------------------------------------------------------ | ---- |
| Duration/Realtime               | 表明这份bugreport记录多长时间的记录。                        |      |
| Metric                          | 一些常规的统计数据，亮屏时间和熄屏时间等                     |      |
| Device’s Power Estimates        | 预估的耗电详情，这个比手机应用的耗电详情更仔细和全面         |      |
| Userspace Wakelocks             | 列出Android系统Wakelocks的情况，这个主要查是否有模块/应用长时间持有Wakelocks而导致无法待机的情况 |      |
| SyncManager Syncs               | 列举同步相关事件                                             |      |
| Mobile Radio Activity Per App   | 列举使用数据网络的时长                                       |      |
| Mobile Traffic Per App          | 列举使用数据网络的流量                                       |      |
| WiFi Scan Activity Per App      | 列举引起WiFi Scan的应用                                      |      |
| WiFi Full Lock Activity Per App | 列举获取WiFi full lock的情况                                 |      |
| Kernel Wakesources              | 列举Kernel层的锁，查看是否由于某些kernel锁被持有而无法待机   |      |
| Kernel Wakeup Reasons           | Kernel唤醒的原因                                             |      |
| App Wakeup Alarms               | 列举系统的alarm                                              |      |
| GPS Use By App                  | 列举使用GPS的app                                             |      |

**History Stats**

   History Stats是记录unplugged的信息，即插着充电器或者usb的信息不统计。它将Bugreport以unplugged进行分段统计。比如下图：总共有6段unplugged的记录（包括掉电量，时长，起始和结束时间）,点击Summary x,就会显示对应unplugged的统计信息，包含有Device State Summary，DataConnectionSummary，ConnectivitySummary，PerAppSyncSummary，WakeupReasonSummary，FirstWakelockAfterSuspend，PhoneStateSummary，ScheduledJobSummary，WifiSupplicantSummary，PhoneSignalStrengthSummary，WifiSignalStrengthSummary，TopApplicationSummary，DozeModeSummary等Summary

**App Selection和App Stats**

   App Selection可以选择某个app来查看这个app的详细耗电情况，其耗电情况体现在App Stats界面。

   App Stats主要包括app包名，版本号，UID，耗电量，在前台运行的时长，使用震动器的时长，使用多少个wakeup alarm，网络信息，Wakelocks信息，Service信息，进程信息，Scheduled Job等。



## Analyze_Suspend

[Analyze_Suspend](https://github.com/arnoldlu/common-use/tree/master/tools/analyze_suspend)



## timerfd

[Linux fd 系列 — 定时器 timerfd 是什么？](https://zhuanlan.zhihu.com/p/409434419)



## Kernel - Power

linux-5.15\Documentation\power



## Kernel - freezing of tasks

[linux 系统进程冻结（freezing of task）](https://blog.csdn.net/wangquan1992/article/details/115110457)

linux-5.15\Documentation\power\freezing-of-tasks.rst
linux-5.15\Documentation\power\suspend-and-cpuhotplug.rst

linux-5.15\kernel\power\hibernate.c
linux-5.15\kernel\power\suspend.c

linux-5.15\kernel\power\user.c

linux-5.15\kernel\power\process.c
linux-5.15\kernel\freezer.c



## Kernel - Suspend Flow

linux-5.15\kernel\power\main.c

linux-5.15\kernel\power\suspend.c



## Kernel - energy model

E:\Seal_Work\重要文件\Other\linux-5.15\Documentation\power\energy-model.rst




## 高通平台GPU动态调频DCVS

[高通平台GPU动态调频DCVS](https://blog.csdn.net/memory01/article/details/97272031)









