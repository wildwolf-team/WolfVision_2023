# WolfVsion 2023

## 环境部署

### 1.1 OpenVINO

配置教程 [Click](https://www.yuque.com/ajiong-hwcyf/geap87/uw0vkg)

在首次运行此项目时，由于OpenVINO需要生成文件，需要大概一分钟才能运行起来

### 1.2 OpenCV

配置教程 [Click](https://www.yuque.com/ajiong-hwcyf/geap87/gxogq1)

推荐使用 4.5.3 版本并配置 Opencv_contrib

### 1.3 fmt文字格式库

下载地址 [Download](https://fmt.dev/latest/index.html)

配置教程 [CLick](https://fmt.dev/latest/usage.html)

在运行 Cmake 进行编译配置时要将 BUILD_SHARED_LIBS 设为 TRUE

```shell
    cmake -DBUILD_SHARED_LIBS=TRUE ..
```
### 1.4 mindvision相机驱动

下载地址 [Download](https://www.mindvision.com.cn/rjxz/list_12.aspx?lcid=138)

进入下载目录

```shell
    mkdir build 

    cd build

    ./run.sh
```

## 使用方法

### 2.1 克隆仓库

访问这个地址 [Projects](https://github.com/wildwolf-team/WolfVision_2023)

使用SSH的方式进行克隆

```shell
git clone git@github.com:wildwolf-team/WolfVision_2023.git
```

### 2.2 部署仓库

进入克隆好的仓库目录运行以下指令
```shell
mkdir build

cd build

cmake ..

make

./WolfVision
```
如果你的坏境是完好的，且编译通过，则本项目开始运行。

### 2.3 使用前请修改以下设定

（1）相机标定文件

（2）相机图像输入分辨率

（3）云台与相机的固定偏移量（数据由机械图纸上获得 单位为：m）

（4）Yaw轴与Pitch轴的固定补偿量

（5）检查是否与电控成功通信

（6）修改 Yaw Power 补偿量

### 2.4 如果本项目无法使用

（1）检查曝光是否正常，图像亮度是否足够

（2）检查电控发送数据是否正常

（3）自瞄时场地上是否有强光对敌方装甲板造成干扰

（4）相机以及串口是否正常工作

（5）检查敌方装甲板上是否贴有数字，数字是否完整

如果还用不了，那就是你参数问题

### 2.5 如需部署在RM机器人上

（1）在自己的笔记本电脑上进行编译部署后放到小电脑上进行运行

（2）注意串口波特率为921600

（3）剩下步骤如 2.3 继续进行




