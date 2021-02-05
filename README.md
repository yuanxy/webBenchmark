# webBenchmark
http benchmark tool to ran out your server bandwidth.
- random User-Agent on every Request
- customizable Referer Url
- cocurrent thread as you wish, depends on you server performance.

# Usage: 
    webBenchmark -c [COUNT] -s [URL] -r [REFERER]
    -c int
          cocurrent thread for download (default 8)
    -r string
          referer url
    -s string
          target url (default "https://baidu.com")

# LINUX:
    wget https://github.com/maintell/webBenchmark/releases/download/0.1/webBenchmark_linux_x64
    chmod +x webBenchmark_linux_x64
    ./webBenchmark_linux_x64 -c 32 -s https://target.url
    
    
    
    这是一个HTTP基准测试工具，可以用来耗尽服务器带宽或流量限额。
特点：

每个请求都有随机的 User-Agent
可自定义请求参数中的 Referer
并发线程取决于您的服务器性能。
项目地址：GayHub

起源
这个起源于MJJ论坛刷“剑皇”的运动。
简单的说就是有一天有人用阿里云OSS存放黄色视频（质量极差，不想瞎眼的就别看），被mjj发现，发了一贴。标题大概是“阿里云oss没有鉴黄？”，附带一个txt文件，包括大约350条链接。闲的没事干的就用吃灰鸡配上aria2/wget刷起来，大概刷了一两天所有链接失效。
有大佬发了一个脚本：
《网络测压小工具webBenchmark》
这是剑皇史上重要的转折点，从个人剑皇变成了集体剑皇，从wget、axel、aria2到专用的golang版本（本文脚本）。

剑皇操作（刷流量）（鉴黄）本质就是 CC 攻击按流量计费的网站，是以恶制恶的行为。

使用说明
参数说明
1
2
3
4
5
webBenchmark -c [COUNT] -s [URL] -r [REFERER]
 
-c 整数，当前的下载线程数（默认 8）；
-r 字符串，HTTP请求的 referer 参数；
-s 字符串，目标链接（默认"https://baidu.com"）；
LINUX:
一条一条复制执行以下命令即可（注意替换参数）。

1
2
3
wget https://github.com/maintell/webBenchmark/releases/download/0.1/webBenchmark_linux_x64
chmod +x webBenchmark_linux_x64
./webBenchmark_linux_x64 -c 32 -s https://target.url
Windows:
打开releases页面
《网络测压小工具webBenchmark》
下载合适的EXE文件
《网络测压小工具webBenchmark》

启动CMD命令窗口，进入程序所在目录，如下运行命令。

《网络测压小工具webBenchmark》
工具的重点在于下载远程文件的过程中不会读写本地硬盘，无需担心本地存储介质问题，工具备份地址：蓝奏 | 微云 密码：m2v9gq

