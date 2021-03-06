# StarEngine
An experimental rendering engine

知乎专栏：
https://zhuanlan.zhihu.com/starengine

# 系统要求
良好的网络环境，能顺利连接github与microsoft。

## Visual Studio 2019 16.8, 需要安装以下模块。

1.Desktop development with C++

2.Game development with C++

3.Universal Windows Platform development

4.Windows10 SDK 18362

5.dotNet desktop development (可选，为了支持Unity)

6.Game development with Unity (可选，为了支持Unity）

## Visual Studio安装完成后，需要安装以下插件

1.C++/WinRT

# 编译步骤
1. 确保网络环境良好，否则可能花费较长时间在文件下载上。

2. 按照上述系统要求安装完Visual Studio 2019

3. git clone vcpkg到本地。 https://github.com/Microsoft/vcpkg 

4. 打开cmd或者powershell，跳转至{vcpkg文件夹}，键入.\bootstrap-vcpkg.bat，编译vcpkg。

5. cmd或者powershell跳转到{StarEngine文件夹}下，键入{vcpkg文件夹}\vcpkg.exe install --triplet x64-windows --feature-flags manifests

6. vcpkg会自动安装boost、eigen3等依赖。安装时间视网络环境与机器配置而定。顺利的话，30分钟左右完成安装。

7. 打开StarEngine目录下的Star.sln，选择x64-Development即可开始编译。

8. 输出文件在build/v142/x64/Development目录下。
