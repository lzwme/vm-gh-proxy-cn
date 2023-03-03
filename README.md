# vm-gh-proxy-cn

GitHub 访问代理助手。一个适合中国大陆用户使用的浏览器油猴脚本。

## 注意：请不要在镜像网站登录账号，若因此造成任何损失本人概不负责

## 主要功能

- 为`源码文件、release附件`添加加速代理链接浮动按钮
- 为仓库生成加速 `clone` 地址的可选项
- 为 `raw`、`release` 附件生成加速下载的链接可选项
- more...

## 安装

首先，你应确保浏览器已安装油猴扩展 [violentmonkey](https://violentmonkey.github.io/get-it/)。

然后在浏览器地址栏输入如下地址，应当会被油猴插件检测到并跳转到安装确认界面（若未检测到，可手动复制其内容，在油猴插件中新建脚本并填入）：

```txt
https://ghproxy.com/https://raw.githubusercontent.com/lzwme/vm-gh-proxy-cn/main/gh-proxy.js
```

## 关于 Github 代理访问体验提升的几种策略

当前主要有以下几种策略，其核心是基于开源免费的 CDN 网站或代理网站地址，对要访问的 GitHub 资源地址支持代理、重定向、或镜像服务，以实现加速访问或下载。

低频率简单使用：

- `host绑定`：DNS 测速获取 host、host 绑定软件定时更新
  - `host 切换管理软件 SwitchHosts`: <brew|scoop> install switchhosts
  - `host定时更新`：https://gitlab.cn/ineo6/hosts/-/raw/master/next-hosts
  - `host定时更新`：https://ghproxy.com/https://raw.githubusercontent.com/521xueweihan/GitHub520/main/hosts
- `浏览器插件网页助手`
  - [violentmonkey(油猴插件)](https://violentmonkey.github.io/get-it/)
  - [Git Master 插件](https://github.com/ineo6/git-master)
- `免费的代理资源站（raw/archive/release 下载、git clone）、mirror镜像`
  - [https://ghproxy.com](https://ghproxy.com)
  - [https://fastgit.org](https://fastgit.org)
  - [CF workers 免费代理站（域名污染，已基本失效）](https://dash.cloudflare.com)
  - [https://cdn.jsdelivr.net/gh](https://cdn.jsdelivr.net/gh) 50MB 限制
  - [https://cdn.staticaly.com/gh](https://cdn.staticaly.com/gh) 图片与源码文件，30MB 限制
  - more...
- `代理软件：`拦截请求，重定向、代理、SNI
  - 本地起 nginx 等 webserver 服务，设置为本地代理，配置代理、重定向、SNI 配置等规则
  - [https://github.com/docmirror/dev-sidecar](https://github.com/docmirror/dev-sidecar)
  - more...
- `仓库镜像`：使用国内开源站查找或自行建立定时同步镜像
  - [gitee mirrors](https://gitee.com/organizations/mirrors/projects)
  - [gitlab.cn](https://gitlab.cn)
  - [gitcode.net/mirrors](https://gitcode.net/mirrors)

高频逛 `GitHub` 的重度用户：

- 买 VPN 服务
- 买外网 VPS 服务器自建代理
- More...

**提示：请注意风险，应仅以为学习研究提供便利为唯一目的，切勿触及道德与法律底线。**

## 相关参考

感谢以下开源仓库的工作。本脚本参考了其中部分仓库的相关逻辑。

- [https://github.com/du33169/gh-proxy-buttons](https://github.com/du33169/gh-proxy-buttons)
- [https://github.com/RC1844/FastGithub](https://github.com/RC1844/FastGithub)
