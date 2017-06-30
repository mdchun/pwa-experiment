## pwa-experiment
一个PWA应用尝试

**[create-react-app](https://github.com/facebookincubator/create-react-app) 生成一个基本的React应用程序**

## start
```
npm install
```
## 启动应用
```
npm start
```

**Lighthouse是来自Google的一个免费工具，可基于他们的PWA清单来评估你的应用**

## 部署
**通过Firebase部署**
-- 在[Firebase控制台](!https://console.firebase.google.com/)中创建一个名为pwa-experiment的新项目
**根目录执行**
```
npm install -g firebase-tools
firebase login
firebase init
```
完成登录并启动初始化后, 回答以下问题：
当问你要为此目录设置什么Firebase CLI功能时，请使用空格键取消选择除托管之外的所有功能。

按回车，然后选择pwa-experiment作为项目。

当问你想用什么作为你的公开目录时，键入build，然后按回车键。

对于单页应用程序问题，回答no。


```
npm run build && firebase deploy
```
创建build文件夹，firebase部署,最后会返回一个[地址](https://pwa-experiment-fefd6.firebaseapp.com/)

## 测试
手机上打开该[地址](https://pwa-experiment-fefd6.firebaseapp.com/)并尝试将其保存到主屏幕,一旦从主屏幕打开，它应该就像一个原生应用。

[更多](https://engineering.musefind.com/build-your-first-progressive-web-app-with-react-8e1449c575cd)