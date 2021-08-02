# 配置VSCODE和交叉编译环境用于开发STM32

众所周知，ARM收购`KEIL`后`KEIL`仍旧没啥长进，唯一好的一点是集成的ARMCC编译器对Cortex-M内核编译效率很高，但这和`KEIL`本身没啥关系。

上面是我的观点，有的就要问了（下面其实是我的内心戏）：

- `KEIL`用中间件、第三方代码之类的很方便？下`KEIL`的Software Pack的时间都能去东京奥运会拿个金牌了。

- `KEIL`安装上就能用，不像`Vscode`要配这配那的？`KEIL`是商业软件，它不配拿来比较。有人要开始反驳了，商业软件促进行业发展。。。。建议您关掉别看，因为作者我从不听取别人意见，不管说的对不对。

- `KEIL`用着挺舒服、它还有逻辑分析仪、软件仿真之类的功能。用着舒服不用看这个，逻辑分析仪、软件仿真我不会也不想用。
- `KEIL`好、`PlatformIO`好。。。。献上一句话和一幅图给任何善意和恶意的抬杠者：我不听，滚。

<img src="readme.assets\b64da6adly1g810dup3qsj20j60khmzq.jpg" style="zoom: 33%;" />

不要质疑用Vscode写STM32的动机，有问题欢迎提issue

## 本体

1. [搭建VSCODE下STM34F4标准库开发环境](readme-stm32f4-mwlib)

2. 搭建VSCODE下STM34F1标准库开发环境

3. 搭建VSCODE下STM34F7标准库开发环境

4. 搭建VSCODE下STM34F4HAL库开发环境

5. 搭建VSCODE下STM34F1HAL库开发环境

6. 搭建VSCODE下STM34F7HAL库开发环境

## 仓库目录说明

- make-from-mingw64

  包含mingw64里的make.exe文件

- stm32-ld

  包含stm32用到的GNU链接脚本

- stm32-startup

  包含stm32用到的启动文件，使用的是GUN的ARM汇编语法

- stm32-svd

  包含stm32的系统视图文件

