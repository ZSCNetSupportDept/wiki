<!-- TITLE: 故障 0 PPPoE错误通用解决方法 -->
<!-- SUBTITLE: 本错误属于移动、联通故障 -->

# 原因

- PPPoE拨号故障

# 通用解决方法

1. 确认网络连通性正确：插紧网线、端口、交换机端口线路
2. 计算机-管理-设备管理器-网络适配器，依次禁用再启用各个网络适配器
3. 网络和共享中心-更改适配器设置，依次禁用再启用各个本地连接/以太网，删除所有宽带 连接并尝试重建
4. 确认本地连接/以太网-属性-Internet协议版本4(TCP/IPv4)-属性，选中自动获取IP地址，自动，获得DNS服务器地址
5. 运行神器Cintrep
6. 运行驱动人生类软件重装驱动
7. 开启相关网络连接所需服务（见下）
8. 重启计算机重置/重装系统

# 开启相关网络连接所需服务

1. Device Install Sevise
2. DHCP Client
3. DNS Client
4. Device Setup Manager
5. DCOM Server Process Launcher
6. Windows Event Log
7. Secure Socket Tunneling Protocol Service
8. Remote Access Auto Connection Manager
9. Remote Access Connection Manager
10. Remote Procedure Call (RPC)
11. Telephony
12. Network Setup Service
13. Network List Service
14. Network Connections
15. Network Store Interface Service
16. System Events Broker
