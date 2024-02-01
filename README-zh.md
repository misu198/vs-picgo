# vs-picgo

> VSCode的扩展 [PicGo](https://github.com/PicGo).

[![version](https://img.shields.io/vscode-marketplace/v/Spades.vs-picgo.svg?style=flat-square&label=vscode%20marketplace)](https://marketplace.visualstudio.com/items?itemName=Spades.vs-picgo)
![Visual Studio Marketplace Rating](https://img.shields.io/visual-studio-marketplace/r/Spades.vs-picgo?style=flat-square)
[![installs](https://img.shields.io/vscode-marketplace/d/Spades.vs-picgo.svg?style=flat-square)](https://marketplace.visualstudio.com/items?itemName=Spades.vs-picgo)
[![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2FPicGo%2Fvs-picgo%2Fbadge%3Fref%3Ddev&style=flat-square)](https://actions-badge.atrox.dev/PicGo/vs-picgo/goto?ref=dev)
[![Coveralls github branch](https://img.shields.io/coveralls/github/PicGo/vs-picgo/refs/heads/dev.svg?style=flat-square)](https://coveralls.io/github/PicGo/vs-picgo?branch=refs/heads/dev)
[![GitHub stars](https://img.shields.io/github/stars/PicGo/vs-picgo.svg?style=flat-square&label=github%20stars)](https://github.com/PicGo/vs-picgo)
[![PicGo Convention](https://img.shields.io/badge/picgo-convention-blue.svg?style=flat-square)](https://github.com/PicGo/bump-version)
[![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg?style=flat-square)](https://standardjs.com)

## 描述

`vs-picgo` 是一个VSCode扩展，用于上传图像到远程图像托管服务，并将url插入当前编辑文件。它比其他工具更有效。它可以给我们更好的上传图片的体验。“vs-picgo”支持8种图像托管服务: [weibo](https://picgo.github.io/PicGo-Doc/zh/guide/config.html#%E5%BE%AE%E5%8D%9A%E5%9B%BE%E5%BA%8A), [qiniu](https://picgo.github.io/PicGo-Doc/zh/guide/config.html#%E4%B8%83%E7%89%9B%E5%9B%BE%E5%BA%8A), [tcyun](https://picgo.github.io/PicGo-Doc/zh/guide/config.html#%E8%85%BE%E8%AE%AF%E4%BA%91cos), [upyun](https://picgo.github.io/PicGo-Doc/zh/guide/config.html#%E5%8F%88%E6%8B%8D%E4%BA%91), [github](https://picgo.github.io/PicGo-Doc/zh/guide/config.html#github%E5%9B%BE%E5%BA%8A), [aliyun](https://picgo.github.io/PicGo-Doc/zh/guide/config.html#%E9%98%BF%E9%87%8C%E4%BA%91oss), [imgur](https://picgo.github.io/PicGo-Doc/zh/guide/config.html#imgur%E5%9B%BE%E5%BA%8A) and [SM.MS](https://sm.ms/), 都是由 [PicGo-Core](https://github.com/PicGo/PicGo-Core).PicGo-Core 的插件功能正在开发中。.

## 功能

<details>
<summary>从剪贴板上传图片</summary>
<img src="https://i.loli.net/2019/04/09/5cac17d2d2265.gif" alt="clipboard.gif">
</details>

<details>
<summary>从资源管理器上传图片</summary>
<img src="https://i.loli.net/2019/04/09/5cac17eea0d65.gif" alt="explorer.gif">
</details>

<details>
<summary>从输入框上传图片</summary>
<img src="https://i.loli.net/2019/04/09/5cac17fe52a86.gif" alt="input box.gif">
</details>

<details>
<summary>使用选中文本作为上传的图片<code>fileName</code></summary>
<img src="https://i.loli.net/2019/04/09/5cac180fb1dc7.gif" alt="selection.gif">
<b>注意：这些字符： <code>\$</code>, <code>:</code>, <code>/</code>, <code>?</code> 和换行符将在图片名称中被忽略. </b>(因为它们对于文件名来说是无效的.)
</details>

## 键盘快捷键

**您可以随意更改下面的所有快捷键。**

| OS           | 从剪贴板上传图像               | 从浏览器上传图片                  | 从输入框上传图片               |
| ------------ | ----------------------------------------------- | ----------------------------------------------- | ----------------------------------------------- |
| Windows/Unix | <kbd>Ctrl</kbd> + <kbd>Alt</kbd> + <kbd>U</kbd> | <kbd>Ctrl</kbd> + <kbd>Alt</kbd> + <kbd>E</kbd> | <kbd>Ctrl</kbd> + <kbd>Alt</kbd> + <kbd>O</kbd> |
| OsX          | <kbd>Cmd</kbd> + <kbd>Opt</kbd> + <kbd>U</kbd>  | <kbd>Cmd</kbd> + <kbd>Opt</kbd> + <kbd>E</kbd>  | <kbd>Cmd</kbd> + <kbd>Opt</kbd> + <kbd>O</kbd>  |

## 设置

- 默认的
  - 默认的图片托管是 [SM.MS](https://sm.ms/).

- 自定义

    <details>
    <summary><b>重大新闻:从2.0.0开始，我们可以在VSCode设置中自定义设置</b></summary>
    <img src="https://i.loli.net/2019/04/09/5cac1821b6621.png" alt="vscode-setting.png">
    </details>

  - 使用外部配置文件

    <details>
    <summary>输入配置文件的路径</summary>
    <img src="https://i.loli.net/2019/04/09/5cac1836598a8.png" alt="external-config.png">
    </details>

  - 使用VSCode设置

    <details>
    <summary>首先，选择当前的PicBed</summary>
    <img src="https://i.loli.net/2019/04/09/5cac1847b5907.png" alt="current-picbed.png">
    </details>

    <details>
    <summary>然后，输入当前PicBed所需的所有信息</summary>
    <img src="https://i.loli.net/2019/04/09/5cac4950d176b.png" alt="picbed-info.png">
    </details>

    <details>
    <summary>自定义要上传的图像的名称</summary>
    <b>注意：如果您在上传之前选择了某些文本，该选择将变成要上传的图像的名称 <code>fileName</code> 上传的图像的名称.</b>
    <img src="https://i.loli.net/2019/04/09/5cac189446749.png" alt="image-name.png">
    </details>

    <details>
    <summary>自定义上传的图像的输出格式</summary>
    <img src="https://i.loli.net/2019/04/09/5cac18a5c9def.png" alt="output-format.png">
    </details>

    <details>
    <summary>
       建议的设置对于  <a href='https://github.com/Molunerfinn/PicGo'>PicGo-electron</a> users (看 <a href='https://picgo.github.io/PicGo-Doc/zh/guide/config.html#%E9%85%8D%E7%BD%AE%E6%89%8B%E5%86%8C'> PicGo配置路径</a> 了解更多信息):
    </summary>
    </details>

    **注意: `YOUR_HOME_DIR` 应替换为您当前用户路径的路径.**

    ```json
    // Windows
    {
        "picgo.configPath":"YOUR_HOME_DIR\\AppData\\Roaming\\PicGo\\data.json",
        "picgo.dataPath": "YOUR_HOME_DIR\\AppData\\Roaming\\PicGo\\data.json"
    }

    // macOS
    {
        "picgo.configPath": "YOUR_HOME_DIR/Library/Application Support/picgo/data.json",
        "picgo.dataPath": "YOUR_HOME_DIR/Library/Application Support/picgo/data.json"
    }

    // Linux
    {
        "picgo.configPath": "YOUR_HOME_DIR/.config/picgo/data.json",
        "picgo.dataPath": "YOUR_HOME_DIR/.config/picgo/data.json"
    }
    ```

    <details>
    <summary><code>picgo.configPath</code> 和 <code>picgo.dataInfoPath</code> 可以在VSCode设置中设置</summary>
    <img src="https://i.loli.net/2019/04/09/5cac19421ddf5.png" alt="for-picgo-user.png">
    </details>

    通过这种方式:

    1. `vs-picgo` 将使用与 `PicGo-electron`.
    2. `PicGo-electron` 将显示所有通过上传的图像 `vs-picgo` 在其相册中.

    </details>

## 迁移

- 从 ^1.0.0 to ^2.x
  - 外部配置文件属性已更改，从 `picgo.path` 到 `picgo.configPath`.

## 版本控制

对于可用的版本，请参阅 [tags on PicGo/vs-picgo](https://github.com/PicGo/vs-picgo/tags). 可以在ChangeLogs中找到 [CHANGELOG.md](CHANGELOG.md).所有开发构建可以在 [GitHub Actions](https://github.com/PicGo/vs-picgo/actions/), 您可以打开特定提交的构建，转到摘要选项卡以下载工件.

## 贡献

请阅读 [CONTRIBUTING.md](./CONTRIBUTING.md) 有关我们的行为准则的详细信息，以及向我们提交拉取请求的流程.

## 贡献者

- [Spades-S](https://github.com/Spades-S)
- [Molunerfinn](https://github.com/Molunerfinn)
- [upupming](https://github.com/upupming)

## 谢谢

- [PicGo-Core](https://github.com/PicGo/PicGo-Core)

**Enjoy!**
