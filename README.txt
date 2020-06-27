配合Shadowrocket观看（适用于最新版）
打开Shadowrocket
生成证书文件（先查看版本）
Shadowrocket 2.1.24（717）之前版本：设置 – 证书 – 生成新的 CA证书 – 安装证书
Shadowrocket 2.1.24（717）之后版本：配置 – 点击一个配置文件HJ_Sword.conf – 编辑配置 – 开启 HTTPS 解密 – 生成新的 CA证书 – 安装证书
如果在这个步骤卡在“强制安装证书”页面，点击“强制安装”也无效的情况下，点右下角Safari浏览器图标，使用Safari打开就可以正常安装了
点右上角 – 安装 – 输入手机锁屏密码 – 再次点右上角 – 安装 – 安装 – 右上角 – 完成
打开手机 – 设置 – 通用 – 关于本机 – 证书信任设置 – 找到 – Shadowrocket开头的选项 – 打开右侧开关 – 弹出警告框 – 继续
再次打开Shadowrocket – 配置 – 找到[本地文件]内的配置文件，HJ_Sword.conf – 点击 – HJ_Sword.conf – 编辑纯文本
翻到底部，在最后粘贴以下代码：
[URL Rewrite]
CN $1KR 302
(?<=\?version_code=)16.. $11 302

[MITM]
hostname = *.tiktokv.com,*.musical.ly

然后点击右上角 – 保存

最后返回首页添加节点，此步骤不可跳过；
然后全局路由选择配置，然后开启连接（首次开启需要验证 – Allow – 指纹/密码）
开启美区TikTok（强调，不是国内版抖音），愉快~



