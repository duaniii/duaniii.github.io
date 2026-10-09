# 段现时的个人主页

适用于 GitHub Pages 的静态个人主页。包含已提供的姓名、硕士生身份、山东大学网络空间安全学院、对称密码实验室、邮箱和 GitHub 链接；后续可添加论文与项目。

## 本地预览

直接用浏览器打开 `index.html`。也可以在本目录运行：

```bash
python3 -m http.server 8000 --bind 127.0.0.1
```

然后访问 `http://127.0.0.1:8000`。不需要安装依赖或构建。

## 发布到 GitHub Pages

1. 登录 **duaniii** 账号，创建名为 **duaniii.github.io** 的 Public 仓库。如果已有同名仓库，先检查原有内容再上传。
2. 将 `index.html`、`styles.css`、`favicon.svg` 和 `.nojekyll` 放到仓库根目录。`README.md` 可一并上传。使用 ZIP 包时，先解压，再上传里面的文件，不能只上传 ZIP，也不要在根目录外再套一层目录。
3. 进入 **Settings → Pages**，Source 选择 **Deploy from a branch**，Branch 选择实际上传文件的分支（通常为 `main`），目录选 **/(root)**，点击 **Save**。
4. 等待 Pages 部署完成后，从 Settings → Pages 的 **Visit site** 打开网站。预期网址为 `https://duaniii.github.io/`。

这是待发布源码；上述网址是否上线，以 GitHub Pages 的实际部署结果为准。

官方文档：[创建 Pages 网站](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site)、[配置发布来源](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)。

## 后续修改

- **个人信息、栏目、链接**：修改 `index.html`。邮箱同时出现在邮件按钮和联系区域。
- **颜色、字体、排版**：修改 `styles.css`，主题色在顶部 `--accent`。
- **网站图标**：替换 `favicon.svg`。

页面以中文为主，适配窄屏，支持键盘导航。使用系统字体，不依赖外部脚本、字体服务或图片服务。
