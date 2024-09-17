# 安装面板

> 这一章你将学习安装面板

---

## 如何安装面板

1. 根据上一章的学习你会学了如何连接到服务器，那么现在就需要安装面板了
    1. 这里我推荐宝塔国际版面板，虽然默认英文但是可以切换繁体中文，例如 **宝塔** **1panel** 面板，需要进行手机号登录和绑定，对于不想实名的你来说不会选择他们，而宝塔国际版不需要登录账号和绑定实名信息等任何操作即可使用
    2. 访问[宝塔国际版](https://www.aapanel.com)官网，点击**Install aaPanel for free**跳转页面复制命令
    3. 回到finalshell，ctrl+v，右键粘贴或者在输入栏中粘贴都可以，粘贴命令上去后回车，等待提示输入y，然后回车
    4. 等待脚本自动安装完成，完成后会输出面板地址 登录账号 密码这些信息，记得保存下来
    5. 浏览器访问安装好的面板地址进行登录，选择LNMP，根据自己的需求选择需要安装的东西
        1. 一般会安装Nginx，PHP，MySQL，phpMyAdmin这几个东西
        2. 面板安装完成后，如果出现访问不了的情况，记得在服务器或者服务器控制面板放行对应的端口
            1. 面板格式一般为 https://ip:端口/路径 根据:后面的端口前往服务器面板进行端口放行
    6. 面板安装目前到此为止，如有遗漏我会补充
    
---

[<<安装finalshell](01/finalshell/)

[>>安装面板](01/mianban/)