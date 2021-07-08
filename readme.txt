1.在计算机管理中新建管理员账号CN，密码:jkl890*()
2.运行LSencrypt.exe将密码:jkl890*()，进行加密
3.复制lsrunase.exe到 C:\Windows\System32\
4.新建批处理a.bat，指向需要绕过UAC的软件路径
5.新建run.bat,lsrunase运行参数如下：
6.运行run.bat

注：只需解压到C:\a\,按照步骤1和3操作，其余步骤仅供参考。

##########################################################################
lsrunase /user:administrator /password:41BngA== /domain: /command:notepad.exe /runpath:c:\
所有的参数必须齐全，其中：
user 为运行的账号
password 为密码加密后的字串
domain 为机器名或域名，也可留空代表本机
command 为要运行的程序名，如果携带参数需要在命令的首尾加引号
runpath 为程序启动的路径
###########################################################################