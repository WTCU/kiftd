# kiftd私有云二次开发
### 此项目为对于基于Java的kiftd进行二次开发的项目
### 此项目为[庞玺桐](https://pangxitong.github.io)和[袁浚皓](https://steveandkrepa.github.io)对[青阳龙野](https://github.com/KOHGYLW/kiftd)的[kiftd](https://github.com/KOHGYLW/kiftd)进行二次开发
#### 此项目主要是对服务的网页进行视图优化，此储存库仅包含网页文件，查找全部可执行文件可以去[青阳龙野](https://github.com/KOHGYLW/kiftd)的[kiftd](https://github.com/KOHGYLW/kiftd)或[此项目的0.0.1版本](https://github.com/WTCU/kiftd/releases/tag/0.0.1)

# 此项目可以进行继续修改的位置:

#上线运行时间
##### ./webContext/JavaScript.js 第16行 
```Javascript
var start_timestamp = 1672992840*1000; 
```
##### 可以更改为服务器建立时的时间代码

# Artalk评论
##### ./webContext/home.html
```html
<center><br><br><div style="font-size:40px;">WTCU留言</div><br><div style="font-size:20px;">支持Markdown语法、Latex语法、OwO表情语法和纯文本</div><br>
<!-- CSS -->
<link href="https://cdn.bootcdn.net/ajax/libs/artalk/2.4.4/Artalk.css" rel="stylesheet">
<!-- JS -->
<script src="https://cdn.bootcdn.net/ajax/libs/artalk/2.4.4/Artalk.js"></script>
<center><div id="Comments"style="width:900px"></div></center>
<br><br><div style="font-size:16px;">评论服务由庞玺桐的个人iMac上构建的自建Artalk服务器提供</div></center><br><br>
<script>
new Artalk({
  el:        '#Comments',// 绑定元素的 Selector
  pageKey:   'http://192.168.31.203',// 固定链接 (留空自动获取)
  pageTitle: '',  // 页面标题 (留空自动获取)
  server:    'https://3jxkfrdkfhha.ngrok.xiaomiqiu123.top',  // 后端地址
  site:      'WTCU',             // 你的站点名
})
</script>
```
##### 可以更改为自己的Artalk服务器参数

# 页面底部参数
##### ./webContext/home.html
```html
<div class="bottom"style="background-color:#F7F8FA">
  <big>
  <p>
    <div style="display:inline-block;" class="uptime"></div>
    &nbsp;&nbsp;&nbsp;开发者：WTCU团队
    &nbsp;&nbsp;&nbsp;网站版本：0.1.0
    <br>
    <a target="_blank" href="https://pangxitong.github.io/open.html"><span9>Copyright</span9></a>
    &nbsp;©&nbsp;2023&nbsp;<a target="_blank" href="https://wtcu.github.io">UTCU.</a>&nbsp;&nbsp;All rights reserved. 
    Based on&nbsp;<a target="_blank" href="https://github.com/KOHGYLW/kiftd">Kiftd.</a>
    &nbsp;Project by <a target="_blank" href="https://wtcu.github.io">UTCU.</a>
  </p>
  </big>
</div>
```
##### 可以根据自己的情况进行更改

# 页面顶部<head>参数
##### ./webContext/prv/error.html 第9行和第35行
##### ./webContext/prv/forbidden.html 第9行和第36行
##### ./webContext/prv/login.html 第11行和第46行
##### ./webContext/prv/login.html 第11行和第27行
##### 有内容需要改成自己的项目名称、组织名称或品牌名

# 公告
#####./notice.md 全部
##### 是显示在登陆后弹窗的信息，支持Markdown语法

# 说明
##### ./来自原开发者青阳龙野的信息
##### 文件夹内包含整个服务端的使用说明，在目前的二次开发进度，完全适用

# 初始信息
#### 管理员账户
##### 用户名：admin
##### 密码：123456
#### ./logs
##### 此文件夹内信息为二次开发测试时产生的日志
