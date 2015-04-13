title: "Converting Xcode iOS app to .ipa"
date: 2012-01-25 22:59:00
tags:
- work
- ios
---
The other day I was coding some apps for my iOS developing class and after I finished it, I found a [way](http://codigohispano.com/index.php?option=com_content&view=article&id=22:test-de-aplicaciones-en-el-iphone-sin-ser-desarrollador&catid=3:tutoriales) to transfer them to my iPhone via Xcode, however that process was a little boring and a little long because you need to make a self signed certificate and trick Xcode to use it, and still you will only be able to put it on the device you have at hand. I wanted to share my app with my friends without the need of App Store submitting and stuff ($99 anual developer fee).

So I found these great 4 steps to convert your Xcode project to a .ipa file that you can easily sincronize via iTunes to your device (you need to be jailbroken and have AppSync installed on your iDevice).

1 - Locate your application’s .app usually in

```
/Users/<youruser>/Library/Application Support/iPhone Simulator/5.0/Applications/<hexadecimal app identifier>/
```

or

```
/Users/<youruser>/Library/Developer/Xcode/DerivedData/<yourappname>/Build/Products/Debug-iphoneos
```

2 - Create a folder called Payload

3 - Place the .app folder inside of that

4 - Zip up the Payload folder using normal compression

5 - Then rename the file with a .ipa extension

6 - Double click so iTunes recognize it and add it to its app library

via [sinfuliphone](http://www.sinfuliphone.com/showthread.php?t=322)
