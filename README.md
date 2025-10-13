项目结构：
HelloCV


├── src/          存放项目源代码（如ROS2节点、OpenCV处理脚本）

├── docs/         存放项目文档（如语雀导出的Markdown文件、技术说明）

├── scripts/      存放可执行脚本（如环境配置脚本、测试脚本）

└── README.md     项目整体说明（结构、配置、使用方法）

2.环境配置
（1）安装 ROS2 Humble
bash
sudo apt update
sudo apt install ros-humble-desktop
（2）安装 OpenCV 4.5.x
sudo apt install libopencv-dev python3-opencv
（3）配置 VS Code 开发环境

安装扩展：C/C++、Python、ROS

配置 tasks.json（编译 ROS2 工作空间）和 launch.json（调试节点）

3. 语雀文档汇总

• ROS2 安装配置

• OpenCV 环境搭建
