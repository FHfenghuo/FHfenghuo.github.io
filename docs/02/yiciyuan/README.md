# 异次元发卡网

> 这一章学习怎么搭建异次元发卡网

---

## 添加站点解析

1. 先在cloudflare中添加新的域名解析，然后再到宝塔面板中添加网站解析
2. 开启Mysql数据库，保存好数据库名和数据库密码(数据库版本>=5.6)
3. 选择php版本>=8.0

---

## 下载解压源码

1. 前往Github下载异次元发卡网的源码 [点击前往](https://github.com/lizhipay/acg-faka) 
2. 下载成功后，转到宝塔面板，点击域名后面的网站文件夹即可跳转，也可以自行寻找路径 /www/wwwroot/ 目录下
3. 右键解压源码即可

---

## 配置数据库

1. 进入config目录，点击database.php文件，配置数据库
2. 把之前保存的数据库名填入 database和username中，把数据库密码填入password，不要删掉引号

---

## 配置网站

1. 转到面板的网站，点击域名，点击伪静态，把下面的伪静态代码输入进去保存
    1. 点击SSL申请免费的证书开启https，记得把域名勾上

2. 保存后访问域名，https://你的域名/admin

```
location / {
      if (!-e $request_filename){
              rewrite ^(.*)$ /index.php?s=$1 last; break;
      }
}
```
---

[>>Epusdt](01/Epusdt/)
