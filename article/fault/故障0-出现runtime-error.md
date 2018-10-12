<!-- TITLE: 故障 0 出现 "Runtime Error!" -->
<!-- SUBTITLE: 本错误属于天翼校园客户端错误-->

<!-- overview: 请将代码放于 SUBTITLE 下 -->
<div class="overview" style="float:right;width:280px;padding:10px;margin:10px;border: 1px solid #4054b2;background-color: #f9f9fb;">
<div class="overview-header" style="width:100%;margin: 5px 0;text-align: center;">
<h3 style="margin:0 0 10px;">出现 "Runtime Error!"</h3>

<img style="display:block;width:100%;max-width:100%;margin-left:-10px;" src="/uploads/0-runtime-error.png" />
</div>

<div class="overview-main" style="display: flex; flex-direction: column;padding:10px 5px 0 5px;">
<div class="overview-item" style="display: flex;margin: 5px 0;">
<p style="flex:0 0 100px;padding:0;font-weight: 600;">故障名称</p>
<p style="padding:0;">出现 "Runtime Error!"</p>
</div>

<div class="overview-item" style="display: flex;margin: 5px 0;">
<p style="flex:0 0 100px;padding:0;font-weight: 600;">故障代码</p>
<p style="padding:0;">0</p>
</div>

<div class="overview-item" style="display: flex;margin: 5px 0;">
<p style="flex:0 0 100px;padding:0;font-weight: 600;">所属运营商</p>
<p style="padding:0;">电信</p>
</div>
</div>
</div>

# 解决方法

步骤一：以 “管理员身份” 运行 cmd，然后输入 `netsh winsock reset catalog`，重启电脑。  
步骤二：如果还不行，重置 TCP/IP 协议，或者直接跑神器吧。  