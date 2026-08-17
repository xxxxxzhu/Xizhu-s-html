# 韩熙竹个人网站

纯静态网站（一个 index.html + 一张照片），中英双语切换

## 部署到 GitHub Pages

1. 去 github.com 新建一个仓库，名字随便取，比如 `my-resume`（建议选 Public，
   GitHub Pages 免费版需要公开仓库；如果不想让搜索引擎收录，可以在页面加
   `<meta name="robots" content="noindex">`，我也可以帮你加）

2. 把这个文件夹里的 `index.html` 和 `assets/` 文件夹整个上传到仓库根目录
   （拖拽上传或用 git push 都行，保持目录结构不变）

3. 仓库页面 → **Settings** → 左侧 **Pages** → Source 选择 `Deploy from a
   branch` → Branch 选择 `main` / `master`，文件夹选 `/ (root)` → Save

4. 等 1-2 分钟，页面顶部会出现一个网址，形如：
   ```
   https://你的用户名.github.io/仓库名/
   ```
   打开就是你的网站了

## 之后想改内容

直接在 GitHub 网页上点开 `index.html`，点右上角铅笔图标编辑，或者告诉我想
改什么，我帮你改好新版本发你。

内容分英文（`data-en` 标签包裹）和中文（`data-zh` 标签包裹）两份，改的时候
两边都要对应更新。

## 想绑定自己的域名（可选）

如果以后想用类似 `xizhuhan.com` 这样的自定义域名，买好域名后在仓库根目录
加一个 `CNAME` 文件（内容就是域名），再去域名服务商那边把 DNS 指向 GitHub
Pages，我可以到时候再帮你走一遍这个流程。
