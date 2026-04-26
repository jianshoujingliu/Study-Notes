# VSCode + MinGW + CMake（现代开发流）
## 准备工作（环境安装）
- MinGW-W64(编译器)
- CMake: 下载安装包并安装，同样建议添加到 PATH。
- Visual Studio Code: 安装 C/C++ 扩展插件 (C/C++ Extension Pack)。

## 创建项目结构
在你的电脑上创建一个文件夹（例如 gtest_demo），并在里面创建以下三个文件：
- hello.cc (你的业务代码)
- hello_test.cc (你的测试代码)
- CMakeLists.txt (构建脚本)
## 编译与运行
在 Windows 上，CMake 默认会尝试找 MSVC 编译器，我们需要强制它使用 MinGW。
1. 打开 VSCode，打开 gtest_demo 文件夹。
2. 打开终端（Terminal），在项目根目录下执行：
3. 运行测试
编译成功后，build 目录下会生成 run_tests.exe（或者是 Debug/Release 子目录下的 exe）。
-注意：在 VSCode 终端中直接运行 .exe 有时会因为 PowerShell 策略问题报错，建议切换到 CMD 终端运行，或者直接去文件夹里双击运行。
.\run_tests.exe
