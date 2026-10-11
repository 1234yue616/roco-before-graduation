# 毕业之前

一册关于相遇、成长与心动的魔法学院手札。

[开始游玩](https://1234yue616.github.io/roco-before-graduation/) · [ChatGPT 游玩页](https://roco-before-graduation.peppytitan4.chatgpt.site/)

《洛克王国》非官方同人恋爱文字游戏，免费体验。打开游玩链接即可开始，无需登录 GitHub。

本仓库用于发布游戏的编译版。`game-release.zip` 包含静态网页、人物素材与 CG，不包含开发环境或服务器。

## 更新方式

使用 `/roco-before-graduation/` 作为资源基础路径构建游戏，将生成的静态文件打包为 `game-release.zip`。压缩包根目录应直接包含 `index.html`、`.nojekyll`、`assets` 等文件和目录。

在同一次提交中替换仓库根目录的 `game-release.zip` 和对应的 `game-release.zip.sha256`，提交到 `main` 分支。Pages 自动发布流程会先校验文件，再解压并部署新版。发布结果以仓库 Actions 和 Pages 页面为准。

可在发布包所在目录生成校验文件：

```bash
sha256sum game-release.zip > game-release.zip.sha256
```

## 存档说明

进度保存在玩家当前浏览器的本地存储中。GitHub Pages 与 ChatGPT Site 使用不同域名，两边的存档相互独立，不会自动同步。
