# NoDevFee
程序永久更新地址：https://github.com/nofeeeth/NoDevFee

Email：nofeeeth@gmail.com

下载地址：https://wws.lanzous.com/s/nofee

V2.0已发布：
1.修复CPU占用过高问题
2.增加en_us语言选择
3.增加NBMiner&T-rex核心拦截


端口定义：如矿池地址cn.sparkpool.com:3333 矿池端口即为3333
监控矿池：添加矿池地址到该窗口则意味着所有连接到该矿池的地址都会被进行拦截
端口：需和监控矿池配合使用
挖矿配置-矿池：你所使用的挖矿矿池地址
挖矿配置-端口：你所使用的挖矿矿池端口
挖矿配置-钱包：你本人的矿池子账号或ETH钱包地址
挖矿配置-矿工名：你本人算力提交到矿池的机器名
挖矿配置-拦截名：拦截到的算力提交到你矿池的机器名

####小白操作步骤（以轻松矿工举例）：
1. 停止轻松矿工挖矿
2. 将矿池配置为蜜蜂（只是为了将流量劫持到拦截软件，并非真实挖矿地址）
3. 打开本软件，填入你真实的矿池地址和端口
4. 配置矿工名和钱包，需和轻松矿工上配置保持一致
5. 点击开始拦截
6. 轻松矿工点击开始挖矿
7. 在1-2H内监控是否有成功拦截日志，及挖矿数据是否正常

####进阶配置：
1. 如果你明确知道抽水的矿池和端口则可以将其加入矿池列表，软件会自动对该地址的eth提交进行拦截
2. 挖矿软件上(如轻松矿工)的矿池可以任意配置为（127.0.0.1:端口） 端口为监控端口中的任何一个端口

监控矿池和端口说明：
配置了监控矿池和对应端口，在其他程序连接到配置中的矿池进行抽水时会进行拦截。如不了解该配置，请勿更改！

！！!注意：拦截3333端口会影响轻松矿工读取数据，导致显示异常，实际算力不受影响。

[========]

F&Q

F：如果软件被核心拦截怎么办？ 如（软件命名NoDevFee.exe时，点击开始挖矿核心会强制关闭该进程）
Q：修改文件名并勾选上随机窗口名选项

F：打开了开机自启和自动拦截后如何修改配置？(考虑后期优化)
Q：先关掉该选项，然后退出程序重新打开即可修改

F：我不用该软件了，但是矿池连不上了怎么办？
Q：打开软件，然后点击退出程序即可恢复初始HOSTS

F：为什么我本地日志打印出来了拦截日志但是矿池却没看到呢？
Q：拦截到那段时间如果没有算出hash提交则矿池不会记录

F：为什么开启后再点击开始挖矿报错Unknown CMD request：eth_submitLogin?
Q：因为挖矿软件用的3333端口被转发到127.0.0.1，但是本地未监听本端口，具体解决看小白操作步骤按步骤操作或自己在挖矿软件中新建矿池127.0.0.1+监听列表中端口

拦截方式：
1.劫持抽水地址改为自己钱包地址 
2.拦截所有抽水请求，禁止其链接矿池
