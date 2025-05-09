# xiaozhi-python
虾哥的小智 AI 聊天机器人（XiaoZhi AI Chatbot）- python客户端

# 鸣谢
首先感谢虾哥提供的服务端

https://github.com/78/xiaozhi-esp32

以上是虾哥的github地址，大家可以去学习，动手能力强的可以制作esp32硬件版本的机器人

# 实现功能
基于python语言，实现在windows系统中访问虾哥小智AI聊天机器人服务器，与大模型机器人进行对话。

所使用的协议为websocket，参考虾哥提供的通信协议，欢迎大家补充功能。

https://ccnphfhqs21z.feishu.cn/wiki/M0XiwldO9iJwHikpXD5cEx71nKh

https://github.com/78/xiaozhi-esp32/blob/main/docs/websocket.md

# 部署脚本
所使用python版本为3.8

需要安装的依赖参考requirements.txt文件

# 配置及使用

一、设置对话模式，自动模式为自动识别语音，手动模式为长按空格键识别语音

is_manualmode = False  #True 手动模式，False自动模式

1、自动模式下，如果连接已经建立，空格键按下为打断当前对话，如果连接已经失效，则重建连接

2、手动模式下，如果连接已经建立，长按空格键进行对话，如果连接已经失效，则重建连接

二、设置设备的MAC地址，确保唯一性,令牌、UUID随意

access_token = "test-token"

device_uuid = "test-uuid"

device_mac = "12:22:33:34:66:89"

三、访问虾哥控制台，进行硬件绑定及设置

1、控制台地址：https://xiaozhi.me/

2、具体操作参见虾哥的手册：https://ccnphfhqs21z.feishu.cn/wiki/F5krwD16viZoF0kKkvDcrZNYnhb

# ESP32S3 硬件版本

https://item.taobao.com/item.htm?ft=t&id=921351525703

# python客户端-udp协议版本

参考zhh827网友的代码

https://github.com/zhh827/py-xiaozhi

玩的开心！！！




