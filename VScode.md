
## VScode 安装配置教程

##### 这里提到的所有安装包和配置文件需要大家到我网盘下载一下啦，链接：

### 1、下载VScode安装
点击VScode安装包运行安装即可

### 2、基本环境配置
1、将setting.json文件内容全部拷到VScode的setting文件中
VScode里ctrl+shift+p里输入 setting 首选项打开设置，将setting.json文件内容粘贴过来这个配置了之后VScode里基本的环境就有了



2、在桌面（或者任务栏）的快捷方式加上  --extensions-dir "目的位置"
这一步目的：默认VScode扩展都安装在C盘，以后每次加载扩展都会在C盘，但是在扩展安装多了后C盘宝贵空间会越占越多。加上这个后以后每次安装扩展都会在你写的目的位置，每次加载也会到该位置加载。例目的位置：“F:/VScodeExtensions”



3、打开VScode，安装系统提示你的扩展，一般在右下角，点击install即可

### 3、C环境配置
1、安装C编译环境：LLVM 直接运行 LLVM-7.0.0-win64.exe 文件


2、解压 MinGW-w64 文件，解压后将其名字改为LLVM，然后复制粘贴到第一步中的LLVM合并两个文件，有相同的则跳过即可


3、增加环境变量。右键桌面此电脑->属性->高级系统设置->环境变量->双击用户变量中的path->新建->添加LLVM下bin目录的路径，如“F:/LLVM/bin”


4、将下载.vscode 文件 并将其粘贴到C工程目录下，并将.vscode文件中c_cpp_properties.json文件中的路径LLVM之前的更改为你自己的目录

![image](.\image\VScode.png)
