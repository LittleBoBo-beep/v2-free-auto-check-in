## 定时任务脚本

v2free自动签到 签到后可以获得流量。
执行结束发送邮件通知签到结果。

使用方法：fork 本仓库

打开浏览器，登陆v2free网站，F12 查看 Network 面板，复制 cookie

打开 github 仓库的 Setting，选择 Secrets，新建下列 4 个仓库 Secret
| key | value |
| --- | ---|
| COOKIE | 值为上面复制v2free的 cookie |
| USER | 发送邮件的邮箱地址，该邮箱需要开启 SMTP |
| PASS | 该邮箱的 SMTP 密码 |
| TO | 接收邮件的邮箱 |