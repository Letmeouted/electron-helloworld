**# electron-helloworld**

helloworld-Electron



如果有需要，请git本项目（仅是为了测试）

<h1>1.在window下打开cmd命令框</h1>

cd xxx //cd到该项目目录下

# 2.安装依赖

cnpm install //等待安装完成所有依赖

# 3.运行

electron .

![image-20201120095433384](C:\Users\Cubicise\AppData\Roaming\Typora\typora-user-images\image-20201120095433384.png)

# 4.打包

//本人已全局安装electron-builder,如需详细打包过程，请看下面的[electron的打包步骤]()

npm run dist // 最后便可完成打包

# 注：electron的打包步骤

在本项目下运行

1.cnpm install electron --save-dev 

2.cnpm install electron-builder --save-dev

3.npm run dist //打包完成后会在你的项目目录下生成一个dist文件夹（如下图所示）

![image-20201120095200218](C:\Users\Cubicise\AppData\Roaming\Typora\typora-user-images\image-20201120095200218.png)

# 注：package.json当中的配置如下

```
 "scripts": {

  "dist": "electron-builder --win --x64"

 },

 "build": {

  "appId": "com.NewElectron.app",

  "mac": {

   "target": [

​    "zip",

​    "dmg"

   ]

  },

  "win": {

   "target": [

​    "zip",

​    "nsis"

   ]

  }

 }


```

