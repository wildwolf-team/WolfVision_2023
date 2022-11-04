# WolfVision

WildWolf Team RoboMaster-2023 Visual &amp; Algorithm Group Code Framework.

## Enviroment

| name           | version                        |
|:--------------:|:------------------------------:|
| System         | [`Ubuntu 21.04`](https://discourse.ubuntu.com/t/hirsute-hippo-release-notes/19221) |
| OpenCV         | [`4.5.3`](https://github.com/opencv/opencv/releases/tag/4.5.3) |
| OpenCV_Contrib | [`4.5.3`](https://github.com/opencv/opencv_contrib/releases/tag/4.5.3) |
| CMake          | [`3.21.0`](https://cmake.org/) |
| GCC            | [`11.1.0`](https://ftp.gnu.org/gnu/gcc/gcc-11.1.0/) |
| GDB            | [`10.2`](https://www.gnu.org/software/gdb/download/) |
| MindVision-SDK | [`2.1.0`](http://mindvision.com.cn/rjxz/list_12.aspx) | 
| cpp-mjpeg-streamer |[html](https://github.com/nadjieb/cpp-mjpeg-streamer/tree/master)
## Contribute

Project created using [Visual Studio Code](https://code.visualstudio.com/), required plugins listed below:

- C/C++ `ms-vscode.cpptools`
- CMake `twxs.cmake`
- CMake Tools `ms-vscode.cmake-tools`
- Visual Studio IntelliCode `visualstudioexptteam.vscodeintellicode`

Our project is here [Projects](https://github.com/wildwolf-team/WolfVision/projects).

### Guide

Before start coding, please finish project configuration first:

```shell
sudo bash scripts/autoconfig.sh
```

After configuration, enjoy coding follow [Google C++ Style Guide](https://google.github.io/styleguide/cppguide.html), linting by command:

```shell
bash scripts/cpplint-pre-commit.sh
```

### Commit Lint

- feat: new feature
- fix: modify the issue
- refactor: code refactoring
- docs: documentation changes
- style: code formatting changes
- test: test case modifications
- chore: other changes, such as build process, dependency management

## License

`MIT, Copyright WildWolf Team 2023`

## 使用方法

### 克隆仓库

访问这个地址 [Projects](https://github.com/wildwolf-team/WolfVision_2023)

使用SSH的方式进行克隆

```shell
git clone git@github.com:wildwolf-team/WolfVision_2023.git
```

### 部署仓库

进入克隆好的仓库目录运行以下指令
```shell
mkdir build

cd build

cmake ..

make

./WolfVision
```
如果你的坏境是完好的，且编译通过，则本项目开始运行。

### 使用前请修改以下设定

（1）相机标定文件

（2）相机图像输入分辨率

（3）云台与相机的固定偏移量（数据由机械图纸上获得 单位为：m）

（4）Yaw轴与Pitch轴的固定补偿量

（5）检查是否与电控成功通信

### 如果自瞄无法使用

（1）检查曝光是否正常，图像亮度是否足够

（2）检查电控发送数据是否正常

（3）自瞄时场地上是否有强光对敌方装甲板造成干扰

（4）相机以及串口是否正常工作

如果还用不了，那就是你参数问题




