RemoteDev Server
================

Bridge for connecting [remotedev monitor app](https://github.com/zalmoxisus/remotedev-app) with [Remote Redux DevTools](https://github.com/zalmoxisus/remote-redux-devtools) or [RemoteDev](https://github.com/zalmoxisus/remotedev) using a local server. Running a local server is optional, you may use [remotedev.io](remotedev.io) server instead, which is by default.

### Installation

```
npm install --save-dev remotedev-server
```

### Usage

```
remotedev --hostname=localhost --port=8000
```

Change `hostaname` and `port` to the values you want.

### Connect from Android device or emulator

If you're running an Android 5.0+ device connected via USB or an Android emulator, use [adb command line tool](http://developer.android.com/tools/help/adb.html) to setup port forwarding from the device to your computer:

```
adb reverse tcp:8000 tcp:8000
```

### License

MIT