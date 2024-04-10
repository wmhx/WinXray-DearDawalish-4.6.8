[winXray 入门小技巧](./sub/introduce.md)   
[winXray 相关视频列表](https://www.youtube.com/results?search_query=winXray)  

# WinXray 
WinXray[:loud_sound:](http://dict.youdao.com/dictvoice?audio=winxray&type=2) 是最简洁轻快的 V2Ray、XRay、Trojan、Trojan-go、Shadowsocks、SSR(ShadowsocksR)、SSRoT、NaïveProxy，SOCKS，HTTP,HTTPS 全能通用客户端（Windows系统），支持并发检测大量服务器并迅速找到当前最快的服务器，服务器连接异常时可自动寻找其他速度最快的服务器 - 切换速度快如闪电，自订阅源获取的服务器异常时可自动刷新订阅，并且自带一键自动部署服务端工具。

**本软件源码已放弃版权贡献到公共域** ，源码可使用 [aardio](http://www.aardio.com) 编译生成单文件绿色EXE

# WinXray 未注册任何域名，谨防钓鱼网站    
WinXray 分为原版、抄袭版。  
抄袭版没有贡献任何功能，仅添加了假冒官网推广链接，然后原版更新任何功能，抄袭版都会复制粘贴改成他自己的名字重新提交，并且乱改版本号

# 本项目说明
项目克隆自 [https://github.com/TheMRLL/WinXray](https://github.com/TheMRLL/WinXray)  
很显然，我克隆的这个项目就是上面所说的抄袭版，加了很多广告。   

### 为什么选择在这个“抄袭版”的基础上改进
这个版本是我接触`winxray`的第一个版本，用了很久，代理上没有什么问题，且这个版本较其他版本改进了些内容，比如  
- 将首选`core`由`v2ray`替换为更好的`xray`
- 添加二维码识别功能
- 其他优化（可能吧...）

### 改进计划
虽然这个版本较原版有些优化，但仍然值得改进。  
- [x] 删除所有广告
- [x] 优化系统托盘显示与交互
- [x] github直连下载改为github加速下载
- [x] 调整配置目录为和应用同级的config目录，方便打包拷走
- [x] 移除检查更新用的大文件
- [x] 节点测速方式更新
- [x] 默认pac规则更新

### 关于issues
我还是个`aardio`菜鸟，也只能做点边边角角上修修补补的事……  
我现在添加节点的方式主要是  
 1. 通过`订阅源`更新
 2. 复制`github`上的节点连接，右键粘贴到`winxray`

节点协议以`trojan`、`vmess`和`ssr`为主。  
<br>
我主要会关注我使用时的bug和功能更新，其他的功能更新和bug修复，等有机会再看吧。

<br>  
<br>  

---

# 原项目
## 原始库由`win2ray`更名为`winXray`网页快照留念
[https://web.archive.org/web/20201128074203/https://github.com/winXray/winXray](https://web.archive.org/web/20201128074203/https://github.com/winXray/winXray)
## 原始库删库前的`README`的部分内容截取


# 使用前必读    
最终都要删库跑路的原因大家都懂不用我多说了吧？！ 我删库特别快，是因为我写代码的速度快，我用了几小时就完成了 winXray 的主要代码，用了几天升级就迅速达到了一般其他软件写了几年的成熟度！因为我即将删库，但是我推上去的更新 - fork 的项目基本都没有那么迅速的主动拉更新，大家可以看一下 winXray 上线才短短几天就超过了 600 forks, 所以如果我推送更新之前不删库，那么我删库以后就没有人能找到最新版本的源代码。   
  
现在大多杀毒软件都是白名单查杀，所以新生的EXE都会乱报病毒，因为我更新的速度太快，所以不断的推新EXE上来，所以你可能遇到误报，但是你完全可以使用源代码自己编译出一模一样的EXE，还有人吹牛说其他翻墙软件不误报 - 你去 issues 里以及网上搜一下有多少误报好不好？！遇到误报可以提交给你的杀毒厂商核实，也可以自己编译源码生成EXE后使用，解决和核实问题很容易 - 其他套路都是多余的。
  
本来 winXray 源码已放弃版权贡献到公共域，但是有人（TheMRLL ）把源码拿去拖了个又大又丑的推广按钮上去，什么功能也不加就发布新版自称官方，而且还把源码搞得很乱出了问题的对本作者进行诋毁（ 错误信息都看不懂居然自称开源软件官方 ），对提及原版 winXray 的帖子进行封删和威胁，我真是惊到了世上居然有如此无耻之人，本来就是给你自由发挥的，吃相这么难看良心不会痛吗？！本来我想改一个许可证限制一下这种不好的行为，但是最后我还是决定继续放弃版权，继续将源码贡献到公共域，即然开放源码，就一定要开放得彻底，我们不能因为世上有个别的恶棍而放弃自己善良的初心。 

最近又发现 TheMRLL 有一些很奇怪的行为。每次我发布新版，他就在后面复制粘贴然后改版本号发布，<span style="color:red">更奇怪的是他的 commits 基本都是伪造的，我用文件比较工具查了一下，他的多个所谓的改进都只是添加了空函数</span>（ 而且还是在开发工具里双击控件生成的范例代码 ）。另外他不知道为什么复制粘贴时很多代码放错了位置，所以他提供的程序很多奇怪的 BUG - 这些我提供的原版是没有的。 虽然我并不反对大家自由使用 winXray 的源码，但这个 TheMRLL 实在是太不像话，他提供的 EXE 请大家注意安全谨慎下载。

---

# PAC 代理模式 / 全局代理 + 路由模式 对比

winXray 的 PAC 代理稳定、流畅、易用。  在 PAC 模式下，winXray 会优先启用高效安全的 SOCKS5 协议，并且可以自动兼容在 PAC 模式下仅支持 HTTP代理的应用。winXray 也可以在 PAC 模式下完美支持 Telegram IP 地址库 。

SOCKS5 支持对比：
- [ ] 全局路由模式: 不支持 SOCKS5
- [x] PAC模式: 支持 高效安全的SOCKS5   
  
UWP 应用支持对比：
- [ ] 全局路由模式: UWP 应用全部无法联网。
- [x] PAC模式: UWP 应用可以正常联网，使用 winXray 自带工具也可以为UWP应用开启本地代理。 

DNS 解析对比：
- [ ] 全局路由模式: 使用本机发起 DNS 解析，即使设为国外 DNS 服务器，仍然会返回适用于国内线路地址。
- [x] PAC模式: 使用服务器上的 DNS 解析，安全可靠。

根据客户端自动切换代理协议：
- [ ] 全局路由模式: 不支持
- [x] PAC模式: winXray 里的 PAC 代理可以让目标应用（例如浏览器）优先选择高效安全的 SOCKS5 代理协议，对于不支持 SOCKS 代理的应用（例如谷歌地球），winXray 在 PAC 模式下会自动为这些应用提供 HTTP 代理。

IP 段代理规则：
- [x] 全局路由模式: 比较好的支持 IP 段代理规则
- [x] PAC模式: winXray 里 PAC 可以支持IP 段代理规则（ 完美支持 Telegram ）。

独立性
- [ ] 全局路由模式: 不独立，代理规则集成在翻墙软件内核中
- [x] PAC模式: 完全独立，PAC 代理服务完全独立于翻墙软件，只有 PAC 指定的域名或IP才会与翻墙软件发生交互。

兼容性
- [ ] 全局路由模式: 不是由系统实现的规则，一旦设置全局代理，不管适不适合走代理的软件都被强制使用代理，所以兼容性不太好，会导致上述的 UWP 无法联网等问题。
- [x] PAC模式: 由系统提供的PAC有良好的兼容性，因为历史悠久，一般的软件都会对PAC有良好的兼容，PAC 主要为适合走代理的浏览器等软件而设计，所以其他软件可以较好的识别并判断是不是要使用 PAC 指定的代理还是直连。

简易度
- [ ] 全局路由模式: 配置复杂，有一定门槛。
- [x] PAC模式: 配置非常简单。


一般不建议普通用户去编辑路由规则 - 错误的配置可能会导致敏感的流量误走代理服务器。
专业的事请交给专业的人去做，使用 winXray 可以一键启用、更新 [v2ray-rules-dat](https://github.com/Loyalsoldier/v2ray-rules-dat) 提供的最新路由规则。

注意在 winXray 里无论使用 NaïveProxy 还是 SSR，SSRoT 都支持 V2Ray 路由规则。

# 设置系统代理失败怎么办
如果设置代理以后不能正常生效：请首先右键点击 winXray 任务栏的托盘图标，在弹出的右键菜单中点击【查看 Internet 代理设置】，并检查代理设置是否正常。如果 winXray 不能修改代理设置，但是可以手动修改成功，这一般是被安全软件错误地拦截了( 而且安全软件没有正常弹出确认对话框，或者误点了阻止设置 ）。这时候请到安全软件的相关设置中将 winXray 添加到信任列表即可。

如果不是上面的原因，请按下【Win + R】组合键打开系统运行对话框，输入 regedit 点击确定打开注册表路径 
<span style="color:green">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Internet Settings\Connections</span>
然后将“Connections”项删除，注销一下系统即可正常使用代理了。

如果上面的方法仍然不行，请在注册表中打开打开路径
<span style="color:green">Computer\HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services\WinHttpAutoProxySvc</span>
将 start 的值改为 2， 也就是将 WinHttpAutoProxySvc 服务改为自动启动，然后重启计算机即可。