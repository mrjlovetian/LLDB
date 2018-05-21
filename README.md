#007--LLDB(Low Lever Debug)


### 断点
* 设置断点
$breakpoint set -n XXX
set 是子命令
-n 是选项 是--name 的缩写!

* 查看断点列表
$breakpoint list 

* 删除
$breakpoint delete 组号

* 禁用/启用
$breakpoint disable 禁用
$breakpoint enable  启用

* 遍历整个项目中满足Game:这个字符的所有方法
$breakpoint set -r Game:
### 流程控制
* 继续执行
$continue c 
* 单步运行,将子函数当做整体一步执行
$n next
* 单步运行,遇到子函数会进去
$s 

### stop-hook
让你在每次stop的时候去执行一些命令,只对breadpoint,watchpoint

### 常用命令
* image list 调用栈列表信息
* p 操作对象
* b -[xxx xxx] 打断点
* x 内存读取
* register read 寄存器读取
* po 打印对象描述


