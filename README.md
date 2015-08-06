# RobotDemo说明

** 纯绿色 无污染 **
----------


##功能
实现向聊天窗口自动重复发送指定内容，即刷屏。

##实现方式
复制指定文本内容到剪切板后，通过Robot模拟重复按Ctrl+V和软件设置的发送消息快捷键(如QQ默认Alt+S)动作实现自动刷屏，
引用了JIntellitype库简化全局热键注册所需的JNI调用过程。

##使用方式
* 运行环境:

1. 必须为32位jre环境，64位环境无法加载32位dll动态链接库文件
2. 注意机器安装多个jre环境时，运行jar文件选择的jre环境

* 运行方式:

1. 将libs库中JIntellitype.dll文件放置到非管理员权限的Path环境变量目录中

2. docs目录下有编译好的Jar包和运行批处理文件runRobot.bat,更改批处理文件中jre路径

3. 双击批处理文件执行程序,将光标置于需要刷屏聊天窗口

4. 默认刷屏内容为‘小娜抱抱’,如需其它默认刷屏内容请在程序内自行更改或在开始刷屏前自行复制

5. 按Ctrl+Alt+R开始刷屏，Ctrl+Alt+S停止刷屏，Ctrl+Alt+X退出程序

6. 程序默认Enter回车键为发送消息快捷键，如果为其它快捷键,请在程序内自行更改

7. 注意快捷键绑定冲突，比如有程序占用了上述快捷键，请先退出占用程序

8. 默认完成一次发送动作为100毫秒,特殊需要请在程序内自行更改

##为什么没有图形界面
一个字---**懒**