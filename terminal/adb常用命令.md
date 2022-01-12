# adb常用命令

**配置adb环境变量 ~/.bash_profile**
```bash
export ANDROID_HOME=/Users/xxx/Library/Android/sdk
export PATH=$PATH:$ANDROID_HOME/platform-tools
```

|功能|命令|
| --- | --- |
|查看手机设备|```adb devices```|
|安装包|```adb install x.apk```|
|卸载包|```adb uninstall x.apk```|
|关闭adb服务|```adb kill-server```|
|启动adb服务|```adb start-server```|
|查看日志|```adb logcat```|
|查看包含时间的日志|```adb logcat -v time```|
|查看级别为Error的日志|```adb logcat *:E```|
|查看包含时间且级别为Error的日志|```adb logcat -v time *:E```|
|保存日志到电脑固定位置|```adb logcat -v time >D:\log.txt```|
|手机文件推送到电脑|```adb pull /sdcard/xx.png D:/xx.png```|
|电脑文件推送到手机|```adb push D:/xx.text /sdcard/xx.text```|
|查看手机里面所有包名|```adb shell pm list packages```|
|查看手机里面所有第三方包名|```adb shell pm list packages -3```|
|截屏并保存文件在手机上为xx.Png|```adb shell /system/bin/screencap -p /sdcard/xx.png```|
|清除应用缓存数据|```adb shell pm clear com.xx.xx```|
|启动程序|```adb shell am start -n com.xx.xx/com.xx.xx.SplashActivity```|
|强制停止应用程序|```adb shell am force-stop com.xx.xx```|
|获取手机设备型号|```adb -d shell getprop ro.product.model```|
|获取手机系统版本|```adb shell getprop ro.build.version.release```|
|获取手机系统api版本|```adb shell getprop ro.build.version.sdk```|
|获取手机厂商名称|```adb -d shell getprop ro.product.brand```|
|获取手机的序列号|```adb get-serialno 或 adb shell getprop ro.serialno```|
|获取手机内存信息|```adb shell cat /proc/meminfo```|
|获取手机物理密度|```adb shell wm density```|




