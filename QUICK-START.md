# 快速部署命令

## 如果你已经安装了Git，可以使用以下命令：

### 1. 首次部署

```bash
# 创建新文件夹
mkdir clothing-rack-product
cd clothing-rack-product

# 初始化Git仓库
git init

# 复制所有文件到这个文件夹，然后：
git add .
git commit -m "Initial commit: Add product page"

# 关联远程仓库（替换YOUR-USERNAME和YOUR-REPO-NAME）
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git

# 推送到GitHub
git branch -M main
git push -u origin main
```

### 2. 更新网站内容

```bash
# 修改文件后
git add .
git commit -m "Update product page"
git push
```

## 没有安装Git？

直接使用GitHub网页界面上传文件即可！
参考 DEPLOYMENT-GUIDE.md 中的"方法A"。

---

**重要提示：**
1. 主页文件必须命名为 `index.html`
2. 确保仓库设置为Public（公开）
3. 在Settings → Pages中启用GitHub Pages
4. 记得修改 sitemap.xml 和 robots.txt 中的URL
