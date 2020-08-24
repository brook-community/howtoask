# 如何提问的Brook版本

关于提问的智慧网上有很多版本, 本版本是关于Brook的又简化版本

### 前提说明

Brook无论是命令行使用还是图形客户端使用都很简单, 所以建议清空下思维后阅读下[Brook文档](https://txthinking.github.io/brook/)以理解Brook的理念, 同时能解决大部分基础问题.

### 提问之前

- 先阅读[Brook文档](https://txthinking.github.io/brook/)
- 先搜索下[issues](https://github.com/txthinking/brook/issues)看看有没有别人已经遇到了你的问题

### 提供完整的环境信息和遇到问题的步骤

#### 坏的提问

- 为什么我的Android手机连接了不能用?

#### 好的提问

1. 我的服务端使用以下命令部署
    0. 我的服务器操作系统是Ubuntu 20.04, 64位
    1. `curl -L https://git.io/getnami | bash && sleep 6 && exec -l $SHELL`
    2. `nami install github.com/txthinking/joker`
    3. `nami install github.com/txthinking/brook`
    4. `joker brook server -l :9999 -p hello` # (备注: 注意隐藏你的密码在公开提问时)
    5. 我通过 `joker list` 查看确保brook已经在运行了
    6. 我确保防火墙已经开放了TCP和UDP的9999端口
2. 我的客户端情况
    0. 我在macOS 10.15.5系统下
    1. 安装了Brook macOS图形客户端v20200901版本
    2. 设置里面的内容我均保持了安装后的默认设置
    3. 选择`server`, 输入`1.2.3.4:9999`(1.2.3.4是我服务端IP), 和密码, 点击Connect后, 页面按钮出现了`Disconnect`
    4. Brook macOS客户端, 从设置页面里我知道在IPv4环境下默认会创建一个socks5://127.0.0.1:1080代理
    5. 我使用[一键测试socks5的TCP和UDP](https://denorun.app/?url=https%3A%2F%2Fgit.io%2Fsocks5.js%20127.0.0.1%3A1080)来测试`127.0.0.1:1080`, 输出了`OK: TCP response is OK`和`OK: UDP response is OK`. 证明我当前网络到服务器的TCP和UDP是畅通的.
3. 当我...时发生了, 却..., 步骤如下
    0. ...
    1. ...

### 我就提个问题需要那么啰嗦吗

- 因为如果信息太少, 回答者可能需要反问你很多问题, 而如果回答者也觉得啰嗦的话, 便可能没人来愿意回答你的问题
- 如果信息足够多, 让回答者一眼便看出可能的问题所在, 直接给你答案, 那么你的问题获得答案的概率便会更大

### Brook是免费开源的软件, 有些问题需要理解下:

- 开发团队可能没有足够多的时间来回答你的问题
- 保持礼貌和风度能让社群里成员更愿意回答你的问题
- 不要带有情绪进行交流, 原本两个陌生人之间谁也不欠谁, 礼貌和风度的交流可能会让你们成为朋友

