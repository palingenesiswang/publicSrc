- 查看设备：
```
adb devices
```
- 安装apk至手机：
```
adb install -r [path.apk]
```
- 查看顶层activity：
```
adb shell dumpsys activity top
```

- 启动/杀死adb服务

```
adb start-server
adb kill-server
```

- 连接指定设备

```
adb connect 127.0.0.1:7555  //	Mumu模拟器示例
```

