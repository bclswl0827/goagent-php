# GoAgent PHP 翻墙

## 这是个什么翻墙法

> 这是基于 PHP_curl 的一种的翻墙方式。将一个 PHP 脚本上传至 PHP 空间，配合即可翻墙。

## Wiki 页

Wiki 页有更详细的介绍。

[https://github.com/bclswl0827/goagent-php-bclswl/wiki](https://github.com/bclswl0827/goagent-php-bclswl/wiki)

## 基本的使用

 - 将这个项目 clone 下来。

```
git clone https://github.com/bclswl0827/goagent-php-bclswl.git
```

 - 然后将 `index.php` 上传至你的 PHP 空间。

 - 浏览器访问对应的地址，如果页面出现跳转，即为部署成功。

 - 在 GoAgent 的本地配置文件 `proxy.ini` 中的 `[php]` 一项的 `enable = 0` 改为 `1`， `fetchserver = ` 填入该脚本地址。需要注意， `=` 后有一个空格号。

 - 以管理员身份运行 GoAgent ，记住程序所给出的本地代理地址，并将该地址配置在所需翻墙的软件上，即可翻墙。速度稳定在 1~2 Mbps 左右，可以轻松观看 YouTube 480P 视频。

### 注意

 - GoAgent 在访问 `HTTPS` 网站时，所使用的证书是自签证书，但 Chrome 浏览器从 58 版开始不再支持自签证书，所以使用最新版 Chrome 浏览时会出现隐私错误的字样。解决方案是使用支持自签证书的 Firefox 最新版本。

 - 首次运行 GoAgent 时，程序会向系统导入证书，所以请务必关闭电脑上的杀毒软件。

 - 首次运行 GoAgent，请使用管理员身份运行。

 - 因为 PHP 版的 GoAgent 不再使用 Google 的 IP ，所以您不用再花时间扫描可用的 Google IP。

 - 如果您使用的是免费 PHP 空间，那么请仔细阅读该空间的使用条款中防止滥用的部分。因为一些 PHP 空间并不允许代理脚本，这样做可能会使您的帐户被锁定。比如 Byethost。同时也请注意流量。

## 进阶的使用

### 设置密码

为了防止盗用，可以设置密码。

默认的密码是 `123456`

### 禁止访问的网站

还可以设置禁止访问的网站。参照脚本中给出的范例设置。

## 备注

 - [Fire-Browser](https://github.com/bclswl0827/Fire-Browser)，翻墙浏览器已经完成～欢迎使用。
