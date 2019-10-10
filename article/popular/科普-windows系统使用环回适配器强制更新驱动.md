<!-- TITLE: windows系统使用环回适配器更新网卡(适配器)驱动 -->
<!-- SUBTITLE: 本文章旨在科普遇网卡设备一直处于黄色感叹号异常状态解决思路 -->

# 简介

本方法原引用自[PPPoE 720 处理方法之 猎豹WIFI 章节](/article/fault/%E6%95%85%E9%9A%9C720-%E6%8B%A8%E5%8F%B7%E7%BD%91%E7%BB%9C%E6%97%A0%E6%B3%95%E5%8D%8F%E8%B0%83%E7%BD%91%E7%BB%9C%E4%B8%AD%E6%9C%8D%E5%8A%A1%E5%99%A8%E7%9A%84%E5%8D%8F%E8%AE%AE%E8%AE%BE%E7%BD%AE#由卸载旧版本猎豹wifi导致解决方法)

鉴于该章节对本方法描述较为精简且没有配图，因此抽出来重新配图科普。

注意本方法对于网卡(适配器)设备一直处于黄色感叹号异常状态同样适用


# 故障现象

网卡(适配器)设备一直处于黄色感叹号异常状态，卸载驱动重启电脑无效

![网卡(适配器)设备一直处于黄色感叹号异常状态](/uploads/kp-hhspq_demo.jpg "网卡(适配器)设备一直处于黄色感叹号异常状态")

# 解决流程
1. 打开设备管理器[可以使用命令`devmgmt.msc`快速打开]
2. 选择 **有叹号** 的设备-右键-更新驱动程序软件

   <img src="/uploads/kp-hhspq_screenshot1.jpg" alt="右键-更新驱动程序软件" height="400" width="600" >
   
   
3. 选择 **浏览我的计算机以查找驱动程序软件**

   <img src="/uploads/kp-hhspq_screenshot2.jpg" alt="浏览计算机以查找驱动程序软件" height="350" width="500" >
   
   
4. 选择  **让我从计算机上的可用驱动列表中选取**

   <img src="/uploads/kp-hhspq_screenshot3.jpg" alt="让我从计算机上的可用驱动列表中选取" height="350" width="500" >
   
5. **去掉** 显示兼容硬件的勾-厂商:Microsoft--网络适配器:Microsoft KM-TEST 环回适配器
   
   <img src="/uploads/kp-hhspq_screenshot4.jpg" alt="去掉显示兼容硬件的勾选择驱动" height="350" width="500" >

6. 下一步。如果有警告提示，就选择 **是**

    <img src="/uploads/kp-hhspq_screenshot5.jpg" alt="警告提示" >

7. 等待安装结束后，回到设备管理器页面，找到“Microsoft KM-TEST 环回适配器”，然后右键卸载，**点击上方的硬件变动扫描按钮** 查看网卡状态是否恢复(有可能需要重新安装一下驱动)
   (如果没有这个按钮的话，随便点击一个设备条目，就会出来这个图标了。或者点最上方菜单栏: 操作-扫描检测硬件变动)
   
   <img src="/uploads/kp-hhspq_screenshot6.png" alt="重新扫描硬件变动" >

## PS
1. 如果在安装驱动的过程中一直在等待中或者安装失败，请尝试到服务中重启 `Device Install Service` 及 `Device Setup Manager` 服务，再重新操作

   【同时按下键盘上的 `win + r` 键，输入 `services.msc` 回车即可进入服务管理页面】
