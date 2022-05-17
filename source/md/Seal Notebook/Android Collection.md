# Android Collection



## Open Source

[xiaomi opensource](https://github.com/MiCode/Xiaomi_Kernel_OpenSource/) 

[oppo opensource](https://github.com/oppo-source/ )

[huawei opensource](https://consumer.huawei.com/en/opensource/detail/?siteCode=worldwide&productCode=Smartphones&fileType=openSourceSoftware&pageSize=10&curPage=1  )



## Android 全局

[Android生命之旅](https://hazyman.com/Technology/2020/Android/)

[Android所有版本变化](https://developer.android.com/about/versions)



## SystemServiceRegistry

[SystemServiceRegistry](https://www.jianshu.com/p/db3ced6c933b)

[系统Service调用及注册机制](https://wwmmyy.github.io/2017/04/18/Android%E7%B3%BB%E7%BB%9F%E6%9C%8D%E5%8A%A1%E8%B0%83%E7%94%A8%E6%B5%81%E7%A8%8B%E5%8F%8A%E6%B3%A8%E5%86%8C%E6%9C%BA%E5%88%B6/)

[Android系统服务的注册方式](http://gityuan.com/2016/10/01/system_service_common/)



## AppOpsService

[Android AppOpsService](https://lixiaogang03.github.io/2021/01/11/Android-AppOpsService/)



## Android ShellCommand

[ShellCommand执行流程](https://blog.csdn.net/xuning2516/article/details/84174096)

**pm** install 说明：

在Android O及之前存在单独的Pm.java文件（frameworks/base/cmds/pm/src/com/android/commands/pm/Pm.java）

从Android P开始移除Pm.java文件，直接预置了 pm 可执行文件，其实是使用cmd package（兼容P之前的pm/am 使用习惯）

http://aospxref.com/android-9.0.0_r61/xref/frameworks/base/cmds/pm/

http://aospxref.com/android-9.0.0_r61/xref/frameworks/base/cmds/pm/pm



## StatLogger(统计func 使用latency，状态信息)

http://aospxref.com/android-12.0.0_r3/xref/frameworks/base/core/java/com/android/internal/util/StatLogger.java

[使用实例](http://aospxref.com/android-12.0.0_r3/search?project=frameworks&full=logDurationStat&defs=&refs=&path=&hist=&type=&xrd=&nn=1)



## Binder IPC的权限控制

[Binder IPC的权限控制](http://gityuan.com/2016/03/05/binder-clearCallingIdentity/)



## Android死亡代理

[Binder死亡通知机制之linkToDeath](http://gityuan.com/2016/10/03/binder_linktodeath/)

- RUST程序设计语言

  [RUST 官网](https://www.rust-lang.org/zh-CN/)

  [RUST程序设计语言](https://kaisery.github.io/trpl-zh-cn/ch00-00-introduction.html)

  [src](https://github.com/rust-lang/book/tree/main/src)



## 问题模拟思路

[为什么 Activity.finish() 之后 10s 才 onDestroy ？](https://juejin.cn/post/6898588053451833351)



## Android & Google CDD

[Android](https://source.android.com/)

[CDD](https://source.android.com/compatibility/cdd)

[android-11-cdd](https://source.android.com/compatibility/11/android-11-cdd)



## Git

[Git 技术干货！工作中"Git"的使用实践和常用命令合集](https://xie.infoq.cn/article/1ce91dc60431b1b8845729d41 )

[HiO技术知识周刊：手把手教你使用Git](https://hio.oppo.com/app/ozone/ruanjianjishu/gotoOzoneCircleKbItemDetail?tt_lang=zh-CN&new_client=1&page=ozone&source=index&enc_kbi_id=158043378_157648901&folder_id=274360&ticket=APPURLWITHTICKETe26f5c4db9b11432f6fac040538818d8&client_id=100000&expire_time=1630307099591&msgShowStyle=31 )

[Git 大全](https://gitee.com/all-about-git )

[Git 命令大全](https://gist.github.com/guweigang/9848271 )



## Java进阶

[你理解了 Java 8 的 Consumer、Supplier、Predicate和Function吗？](https://cloud.tencent.com/developer/article/1488128)

[深入浅出 Java 8 Lambda 表达式](http://blog.oneapm.com/apm-tech/226.html)



## Android反编译

JADX反编译

https://github.com/skylot/jadx 

GDA反编译

http://www.gda.wiki:9090/ 

https://github.com/charles2gan/GDA-android-reversing-Tool 

JD反编译

http://java-decompiler.github.io/



## PropertyInvalidatedCache

[PropertyInvalidateCache实现](http://aospxref.com/android-12.0.0_r3/xref/frameworks/base/core/java/android/app/PropertyInvalidatedCache.java)

[PropertyInvalidateCache用法举例](http://aospxref.com/android-12.0.0_r3/xref/frameworks/base/core/java/android/os/PowerManager.java#MAX_CACHE_ENTRIES)



## Boolean锁同步及更新触发动作

同样适用Inter，String等

[用法举例](http://aospxref.com/android-12.0.0_r3/xref/frameworks/base/services/core/java/com/android/server/power/batterysaver/BatterySaverPolicy.java#1310)



## Android Settings数据库Debug

[【Android】 adb shell 下 setting 指令](https://blog.csdn.net/qq_22370409/article/details/89350235)

设置battery_saver_constants 

```
settings put global battery_saver_constants "advertise_is_enabled=true,datasaver_disabled=true,enable_night_mode=true,launch_boost_disabled=true,vibration_disabled=true,animation_disabled=false,soundtrigger_disabled=true,fullbackup_deferred=true,keyvaluebackup_deferred=true,firewall_disabled=true,gps_mode=2,adjust_brightness_disabled=true,adjust_brightness_factor=0.5,force_all_apps_standby=true,force_background_check=true,optional_sensors_disabled=true,aod_disabled=true,quick_doze_enabled=true"
```

删除battery_saver_constants 

```
settings delete global battery_saver_constants
```

查询battery_saver_constants 

```
settings get global battery_saver_constants
```

[AndroidQ SettingsProvider和Settings原理](https://blog.csdn.net/pillarbuaa/article/details/107814333)



## 手机参数

https://www.zhihu.com/column/c_1280250296166240256



## Kernel知识

[Kernel组成](https://www.i4k.xyz/article/p1279030826/105998601)

[Linux IO模式及 select、poll、epoll详解](https://segmentfault.com/a/1190000003063859)



## Comparator

[Comparator结合Collections.binarySearch进行排序插入](https://cs.android.com/android/platform/superproject/+/master:frameworks/base/apex/jobscheduler/service/java/com/android/server/alarm/BatchingAlarmStore.java;l=276;drc=master)

https://blog.csdn.net/agony_sun/article/details/77504199



## Java Predicate

 [Predicate详解](https://www.cnblogs.com/qdhxhz/p/11323595.html)



## ATRACE_CALL

http://aospxref.com/android-12.0.0_r3/xref/frameworks/native/opengl/libs/EGL/egl_trace.h#EglScopedTrace
https://blog.csdn.net/u013741019/article/details/108502461



## AndroidStudio无法自动检查编码错误

https://blog.csdn.net/a_running_wolf/article/details/48708459



## Java CallStack

```
private void printCallStack() {
    StackTraceElement[] stackTrace= Looper.getMainLooper().getThread().getStackTrace();
    Log.e(TAG, "------------"+
            stackTrace[3].getMethodName()+
            " begin------------");
    for (int i = 3; i < stackTrace.length; i++) {
        Log.e(TAG, "    " + stackTrace[i].toString());
    }
    Log.e(TAG, "------------"+
            stackTrace[3].getMethodName()+
            " end------------");
}
```



## HAL HIDL

[使用Android的HIDL+AIDL方式编写从HAL层到APP层的程序](http://www.max-shu.com/blog/?p=1075)

[HIDL系列一](https://chendongqi.me/2019/08/30/hidl-passthrough-with-binderized/)

[HIDL系列二](https://chendongqi.me/2019/09/01/hidl-same-process-passthrough/)

[HIDL系列三](https://chendongqi.me/2019/09/01/hidl-binderizing-passthrough/)

[HIDL系列四](https://chendongqi.me/2019/09/08/hidl-binderizd/)



## HAL AIDL

实现Light AIDL的一个实例

/hardware/interfaces/light/aidl/android/hardware/light/ILights.aidl

[Android Lights AIDL HAL](https://github.com/SoMainline/android-lights-hal)

[Path : Add Power HAL implementation](https://review.lineageos.org/c/LineageOS/android_device_fxtec_pro1/+/292109/2)

[Example to explain the AIDL internal process communication interface using _android in Android](https://topic.alibabacloud.com/a/example-to-explain-the-aidl-internal-process-communication-interface-using-_android-in-android_1_21_20160666.html)

**Power AIDL HAL 的实现**

Power HAL AIDL接口路径：/hardware/interfaces/power/aidl/android/hardware/power/

以default example 实现为例说明：/hardware/interfaces/power/aidl/default/

以 setMode 这个HAL interface为例说明

> /hardware/interfaces/power/aidl/default/power-default.rc
>
> ```
> service vendor.power-default /vendor/bin/hw/android.hardware.power-service.example
>     class hal
>     user nobody
>     group system
> ```

> /hardware/interfaces/power/aidl/default/power-default.xml
>
> ```
> <manifest version="1.0" type="device">
>     <hal format="aidl">
>         <name>android.hardware.power</name>
>         <version>2</version>
>         <fqname>IPower/default</fqname>
>     </hal>
> </manifest>
> ```

> /hardware/interfaces/power/aidl/default/Android.bp
>
> ```
> cc_binary {
>     name: "android.hardware.power-service.example",
>     relative_install_path: "hw",
>     init_rc: ["power-default.rc"],
>     vintf_fragments: ["power-default.xml"],
>     vendor: true,
>     shared_libs: [
>         "libbase",
>         "libbinder_ndk",
>         "android.hardware.power-V2-ndk_platform",
>     ],
>     srcs: [
>         "main.cpp",
>         "Power.cpp",
>     ],
> }
> ```

> /hardware/interfaces/power/aidl/default/main.cpp
>
> ```
> int main() {
>     ABinderProcess_setThreadPoolMaxThreadCount(0);
>     std::shared_ptr<Power> vib = ndk::SharedRefBase::make<Power>();
> 
> 	const std::string instance = std::string() + Power::descriptor + "/default";
> 	binder_status_t status = AServiceManager_addService(vib->asBinder().get(), instance.c_str());
> 	CHECK(status == STATUS_OK);
> 
> 	ABinderProcess_joinThreadPool();
> 	return EXIT_FAILURE;  // should not reach
> 
> }
> ```

/hardware/interfaces/power/aidl/default/Power.cpp

```
ndk::ScopedAStatus Power::setBoost(Boost type, int32_t durationMs) {
    LOG(VERBOSE) << "Power setBoost: " << static_cast<int32_t>(type)
                 << ", duration: " << durationMs;
    return ndk::ScopedAStatus::ok();
}
```



mian 函数注册 hal service name为 ： **std::string() + Power::descriptor + "/default"**

其本质就是：**Power::descriptor + "/default"**

Power::descriptor的定义在哪？？

Power AIDL HAL在编译的时候会生成中间文件，在如下路径：**out/soong/.intermediates/hardware/interfaces/power/aidl/android.hardware.power-V2-ndk_platform-source/gen**

涉及文件：android  include  timestamp

其中，Power::descriptor的定义在如下路径：

./android/hardware/power/IPower.cpp

const char* IPower::descriptor = "android.hardware.power.IPower";

以上使Power AIDL HAL的实现。



**Power AIDL HAL 的使用**

使用端从 PowerManagerService 开始

```
    private void setPowerBoostInternal(int boost, int durationMs) {
        // Maybe filter the event.
        mNativeWrapper.nativeSetPowerBoost(boost, durationMs);
    }
```

调用到 JNI 中

/frameworks/base/services/core/jni/com_android_server_power_PowerManagerService.cpp

```
static void nativeSetPowerBoost(JNIEnv* /* env */, jclass /* clazz */, jint boost,
                                jint durationMs) {
    setPowerBoost(static_cast<Boost>(boost), durationMs);
}
static void setPowerBoost(Boost boost, int32_t durationMs) {
    gPowerHalController.setBoost(boost, durationMs);
    SurfaceComposerClient::notifyPowerBoost(static_cast<int32_t>(boost));
}
```

Power JNI 透过 libpowermanager 提供的通道和Power AIDL HAL交互

PowerHalController 进行 init 和 触发 HAL Connect ，并进行接口调用

HalConnector 进行HAL Connect ，先尝试connect AIDL HAL，如果AIDL HAL不存在，再connect HIDL HAL

```
std::unique_ptr<HalWrapper> HalConnector::connect() {
    sp<IPower> halAidl = PowerHalLoader::loadAidl();
    if (halAidl) {
        return std::make_unique<AidlHalWrapper>(halAidl);
    }
    sp<V1_0::IPower> halHidlV1_0 = PowerHalLoader::loadHidlV1_0();
    sp<V1_1::IPower> halHidlV1_1 = PowerHalLoader::loadHidlV1_1();
    if (halHidlV1_1) {
        return std::make_unique<HidlHalWrapperV1_1>(halHidlV1_0, halHidlV1_1);
    }
    if (halHidlV1_0) {
        return std::make_unique<HidlHalWrapperV1_0>(halHidlV1_0);
    }
    return nullptr;
}
```

这里仅关注AIDL HAL

PowerHalLoader loadAidl

```
sp<IPower> PowerHalLoader::loadAidl() {
    std::lock_guard<std::mutex> lock(gHalMutex);
    static bool gHalExists = true;
    static auto loadFn = []() { return waitForVintfService<IPower>(); };
    return loadHal<IPower>(gHalExists, gHalAidl, loadFn, "AIDL");
}
```

loadFn 指定 load/connect AIDL HAL的实际实现waitForVintfService<IPower>()

waitForVintfService 实现在： /frameworks/native/libs/binder/include/binder/IServiceManager.h

```
template<typename INTERFACE>
sp<INTERFACE> waitForVintfService(
        const String16& instance = String16("default")) {
    return waitForDeclaredService<INTERFACE>(
        INTERFACE::descriptor + String16("/") + instance);
}
```

逻辑很简单：laod name 为 **INTERFACE::descriptor + "/default"** 的AIDL HAL Service

load完成之后，即可以正常使用AIDL HAL 了



## ADB Shell Commands List

[ADB Shell Commands List and Detailed Cheat Sheet](https://technastic.com/adb-shell-commands-list/)



## StatLogger

StatLogger可以用来统计function执行时长

[举例说明LazyAlarmStore中的StateLogger使用](https://cs.android.com/android/platform/superproject/+/master:frameworks/base/apex/jobscheduler/service/java/com/android/server/alarm/LazyAlarmStore.java;l=107;drc=master;bpv=1;bpt=1)



## Google Pixel 运营商查询

[查询 Google Pixel 保修信息以及判断是否为 Verizon （运营商） 版](https://ericclose.github.io/Pixel-repairs-and-carriers.html)

[Check IMEI](https://www.imei.info/)



## Android Source Code 在线

[Android Code Search](https://cs.android.com/)

[AOSPXRef](http://aospxref.com/#538)



## Android Linker:namespace隔离机制

[Android Linker:namespace隔离机制](https://www.jianshu.com/p/1672b52548ce?utm_campaign=maleskine&utm_content=note&utm_medium=seo_notes&utm_source=recommendation)



## Android应用启动全流程分析（源码深度剖析）

[Android应用启动全流程分析（源码深度剖析）](https://www.jianshu.com/p/37370c1d17fc)



## Android 开机启动流程分析

[android 开机启动流程分析（01） init之前启动说明 原创](https://blog.51cto.com/u_14344871/3370053)

[android 开机启动流程分析（02）init的启动流程分析 原创](https://blog.51cto.com/u_14344871/3370052)

[android 开机启动流程分析（03）init启动中关键进程 uevent & watchdog 原创](https://blog.51cto.com/u_14344871/3370051)

[android 开机启动流程分析（04）init启动中关键服务-属性服务 原创](https://blog.51cto.com/u_14344871/3370050)

[android 开机启动流程分析（06）init.rc解析流程 原创](https://blog.51cto.com/u_14344871/3370049)



## Android uevent

[android-uevent 简记](https://blog.csdn.net/prike/article/details/78492613)
