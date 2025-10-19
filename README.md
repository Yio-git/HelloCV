文本加解密工具（CryptoTool）

一个基于 C++ 和 CMake 的简易文本加解密工具，支持凯撒密码和XOR 加密算法，提供文本加密/解密、文件加密/解密功能，并通过交互式命令行菜单操作。

项目结构
CryptoTool/


├── include/        # 头文件目录

│   ├── Crypto.h    # 加密解密逻辑类

│   ├── FileHandler.h  # 文件操作类

│   └── Menu.h      # 命令行菜单类

├── src/            # 源文件目录

│   ├── Crypto.cpp

│   ├── FileHandler.cpp

│   ├── Menu.cpp

│   └── main.cpp    # 主程序入口

└── CMakeLists.txt  # CMake 构建配置文件
技术栈

• 编程语言：C++11

• 构建工具：CMake

• 加密算法：凯撒密码（Caesar Cipher）、XOR 加密

构建与运行

步骤 1：使用 CMake 构建
# 创建并进入构建目录
mkdir build && cd build

# 生成 Makefile 并编译
cmake ..
make
步骤 2：运行程序
./CryptoTool
功能说明

1. 文本加密/解密

• 凯撒密码：通过字母偏移量（密钥）对文本进行加密/解密。

• XOR 加密：通过字节异或运算对文本进行加密/解密（加密和解密逻辑一致）。

2. 文件加密/解密

• 支持从文件读取文本并加密，结果保存到新文件；

• 支持从加密文件读取文本并解密，结果保存到新文件。

3. 交互式菜单

通过命令行菜单选择功能，输入对应数字即可执行加密/解密操作。

示例输入输出

示例 1：凯撒密码-文本加密
请输入要加密的文本: Hello, World!
请输入密钥: 3
加密结果: Khoor, Zruog!
示例 2：凯撒密码-文本解密
请输入要解密的文本: Khoor, Zruog!
请输入密钥: 3
解密结果: Hello, World!
示例 3：文件加密（凯撒密码）
请输入要加密的文件路径: input.txt
请输入密钥: 5
加密结果已保存到: encrypted_caesar.txt
