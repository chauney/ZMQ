# 编译
使用cmake，先进到该目录
cd libzmq-test
mkdir build
cd build
cmake ..
make
在build目录下则可以看到对应.c文件生成的对应的bin执行文件。

# 代码说明
1.REQ/REP模型
hwserver.c 		REP
hwclient.c 		REQ

2.PUB/SUB模型
wuserver.c	 	PUB
wuclient.c   	SUB

3.PUSH/PULL模型
taskwork.c		PUSH	
taskvent.c		PULL-PUSH
tasksink.c		PULL

4.ROUTER/DEALER 
rrclient.c		REQ
rrbroker.c		ROUTER/DEALER
rrworker.c		REP

文章见：https://blog.csdn.net/weixin_34764432/article/details/109130445
