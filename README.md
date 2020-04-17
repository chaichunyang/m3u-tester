# m3u-tester
此脚本主要用来测试m3u视频资源的连接速度，每个人的网络环境不同，测试结果也会不一样
此脚本基于python 3.8.2编写，其他版本并未测试，本人也不是很熟悉python，有写的不好的地方，欢迎指正
# 使用
脚本会检查当前目录下的`.m3u`文件，并测试所有检测到的视频流资源的网络连接速度
```
python3 m3u-tester.py
```
每个连接测试大约需要5秒左右的时间，如果资源较多，可能需要花费较长时间才能完成

测试完成后，会在当前目录生成以下文件：
1. result.json，所有测试的结果，包括extinf，url，speed
2. useful.m3u，速度大于200KB/sec
3. good.m3u，速度大于500KB/sec
4. wonderful.m3u，速度大于700KB/sec
5. excellent.m3u，速度大于1MB/sec
