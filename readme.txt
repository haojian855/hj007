方案（一）VerifyS.exe 作为服务运行 每日开机无需登陆即可运行认证程序 方法：

 NTService.exe 程序可以帮助VerifyS.exe作为后台服务运行
 NTService.ini 设置文件 修改CommandLine 和 WorkingDir 项
 /*CommandLine 设置为认证程序的绝对路径*/
 /*WorkingDir  设置为认证程序的工作目录*/

 在CMD下 运行NTService.exe -i 注册服务 重启机器 即可

方案（二）登陆操作系统后 手工启动VerifyS.exe 开机后必须手动再次启动