# house-clean-site

Mac House Clean 官网（静态站，托管于 GitHub Pages）。

- 站点：https://house-clean.zpad.app
- 归属仓库：pekaboo/house-clean-site（public，仅静态文件；App 源码在私有仓库 pekaboo/mac-house-clean）

## 部署

推送到 `main` 即自动发布（GitHub Pages，来源 = main 分支根目录）。

## 自定义域名（一次性）

DNS 在 `zpad.app` 的解析商处添加：

```
类型   主机名            值
CNAME  house-clean      pekaboo.github.io
```

GitHub 仓库 Settings → Pages → Custom domain 已由 `CNAME` 文件声明为
`house-clean.zpad.app`；DNS 生效后勾选 **Enforce HTTPS**。

## 截图更新

`assets/*.jpg` 来自 App 仓库的 `marketing/zh-Hans/light/`，由
`scripts/capture-marketing.sh` 生成后压缩拷贝（sips, 1440px, q82）。

## 待办（上架后）

- [ ] `index.html` 两处 `https://apps.apple.com/app/machouseclean` 占位换成真实 App Store 链接（App ID）
- [ ] 页脚 `support@zpad.app` 换成真实支持邮箱（若不同）
- [ ] App Store Connect 的「隐私政策 URL」填 `https://house-clean.zpad.app/privacy.html`，「支持 URL」填 `https://house-clean.zpad.app`
