<!-- TITLE: 故障0-Windows通信端口初始化失败 -->
<!-- SUBTITLE: 本错误属于天翼校园客户端错误 -->

![windows通信端口初始化失败](/uploads/0-windows-port-init-fail.png)

# 原因

Windows通信端口初始化失败

# 解决办法

1. 以管理员权限打开CMD，输入`netsh winsock reset`，回车（重置LSP）
2. 禁用再启用网卡，或者重启电脑
