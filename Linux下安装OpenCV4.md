# 安装OpenCV4

## 依赖项

```shell
sudo apt-get install libvtk7-dev libjpeg-dev libtiff5-dev libopenexr-dev libtbb-dev
```

## 编译源码

```shell
cmake -D CMAKE_BUILD_TYPE=RELEASE -D WITH_TBB=ON  -D WITH_V4L=ON -D CMAKE_INSTALL_PREFIX=/usr/local/opencv430 ..  

make  -j8

sudo make install
```

## 构建项目

使用CMake构建项目