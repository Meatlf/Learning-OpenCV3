# 安装OpenCV4

## 依赖项

```shell
sudo apt-get install libvtk7-dev libjpeg-dev libtiff5-dev libopenexr-dev libtbb-dev
```

## 下载源码

从[OpenCV官方](https://opencv.org/releases/)下载源码到本地,解压,进入目录,然后执行以下操作:
```
mkdir build
cd build

```

## 编译源码

```shell
cmake -D CMAKE_BUILD_TYPE=RELEASE -D WITH_TBB=ON  -D WITH_V4L=ON -D CMAKE_INSTALL_PREFIX=/usr/local/opencv430 ..  

make  -j8

sudo make install
```

## 构建项目

使用CMake构建项目,具体参考'code/code-official/chapter14-轮廓'项目.