---
title: "Can't input Chinese in Mendeley by using fcitx at Ubuntu 18.04"
date: 2019/06/15
permalink: /posts/2019/06/mendeleyfcitx/
tags:
  - UBUNTU
  - Mendeley
  - Fcitx
---

# Locate qt fcitx lib
```shell
locate libfcitxplatforminputcontextplugin.so
```
Typically, the system default one is:
```
/usr/lib/x86_64-linux-gnu/qt5/plugins/platforminputcontexts/libfcitxplatforminputcontextplugin.so
```

# Copy it to Mendeley folder
```shell
cd /opt/mendeleydesktop/plugins/qt/plugins/platforminputcontexts
sudo cp /usr/lib/x86_64-linux-gnu/qt5/plugins/platforminputcontexts/libfcitxplatforminputcontextplugin.so ./
```

# Restart Mendeley and try to input Chinese

# Reference & Useful materials

- [https://www.findhao.net/easycoding/2287](https://www.findhao.net/easycoding/2287)
- [https://github.com/JackieMium/my_blog/issues/12)](https://github.com/JackieMium/my_blog/issues/12)
- [http://yinflying.top/2017/09/727#comment-31](http://yinflying.top/2017/09/727#comment-31)
