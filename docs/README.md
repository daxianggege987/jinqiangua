# 易经八卦通 — 公开页面（隐私政策 / 技术支持）

本目录包含供 **App Store Connect** 填写的：

- `privacy-policy.html` — 隐私政策  
- `support.html` — 技术支持  

## 发布到 GitHub Pages 后的访问地址

在 GitHub 仓库中启用 **Settings → Pages**，Source 选择 **Deploy from a branch**，Branch 选 **main**（或 **master**），文件夹选 **`/docs`**。

假设您的用户名为 **`YOUR_USERNAME`**，仓库名为 **`YOUR_REPO`**，则公开链接一般为：

| 页面     | URL |
|----------|-----|
| 隐私政策 | `https://YOUR_USERNAME.github.io/YOUR_REPO/privacy-policy.html` |
| 技术支持 | `https://YOUR_USERNAME.github.io/YOUR_REPO/support.html` |

将上述 URL 填入 App Store Connect 的 **隐私政策 URL** 与 **支持 URL**。

## 发布前请修改

1. 两个 HTML 文件中的 **`support@yijingbagua.app`** 改为您真实可用的邮箱。  
2. 若应用名称或功能有变更，请同步更新正文。

## 推送到 GitHub（示例）

```bash
cd /path/to/jinqiangua
git init
git add docs/
git commit -m "Add privacy policy and support pages for App Store"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
git push -u origin main
```

然后在仓库 **Settings → Pages** 中按上文启用 `/docs`。
