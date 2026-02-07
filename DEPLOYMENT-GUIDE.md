# GitHub Pages 部署教程

## 📋 前期准备

1. **注册GitHub账号**
   - 访问：https://github.com
   - 点击 "Sign up" 注册免费账号
   - 验证邮箱

## 🚀 部署步骤

### 步骤 1: 创建仓库

1. 登录GitHub后，点击右上角的 "+" 按钮
2. 选择 "New repository"
3. 填写仓库信息：
   - **Repository name**: `clothing-rack-product` (或任何你喜欢的名字)
   - **Description**: `Heavy Duty Clothes Rack Product Page`
   - 选择 **Public** (必须是公开仓库才能使用免费的GitHub Pages)
   - ✅ 勾选 "Add a README file"
4. 点击 "Create repository"

### 步骤 2: 上传HTML文件

#### 方法A: 通过网页界面上传（推荐新手）

1. 在仓库页面，点击 "Add file" → "Upload files"
2. 将 `index.html` 文件拖入上传区域
3. 在底部填写提交信息：
   - Commit message: `Add product page`
4. 点击 "Commit changes"

#### 方法B: 使用Git命令行（推荐熟悉Git的用户）

```bash
# 1. 克隆仓库到本地
git clone https://github.com/你的用户名/clothing-rack-product.git
cd clothing-rack-product

# 2. 复制HTML文件到仓库目录，并重命名为index.html
cp /path/to/clothing-rack-product-page.html index.html

# 3. 提交并推送
git add index.html
git commit -m "Add product page"
git push origin main
```

### 步骤 3: 启用GitHub Pages

1. 在仓库页面，点击顶部的 "Settings" (设置)
2. 在左侧菜单找到 "Pages"
3. 在 "Source" 部分：
   - Branch: 选择 `main`
   - Folder: 选择 `/ (root)`
4. 点击 "Save"
5. 等待几分钟，页面会显示：
   ```
   Your site is live at https://你的用户名.github.io/clothing-rack-product/
   ```

### 步骤 4: 访问你的网站

- 你的网站地址：`https://你的用户名.github.io/仓库名/`
- 例如：`https://johnsmith.github.io/clothing-rack-product/`

## 📝 重要提示

### 文件命名规则
- **主页必须命名为 `index.html`** （小写）
- GitHub Pages会自动识别这个文件作为网站首页

### 网站地址
- 默认地址：`https://用户名.github.io/仓库名/`
- 如果想要更短的地址，可以：
  1. 创建一个特殊仓库：`用户名.github.io`
  2. 上传index.html到这个仓库
  3. 你的网站地址就会变成：`https://用户名.github.io/`

### 更新网站内容
每次修改HTML文件后：
1. 重新上传到GitHub（覆盖旧文件）
2. 或使用Git推送更新
3. 等待1-2分钟，网站会自动更新

## 🎯 提交到Google Search Console

网站上线后，将网址提交到Google：

1. 访问：https://search.google.com/search-console
2. 添加资源 → 输入你的网站URL
3. 验证所有权（推荐使用HTML文件验证）
4. 提交Sitemap（可选）
5. 等待Google索引（通常1-7天）

## ✅ 检查清单

部署前确认：
- [ ] GitHub账号已注册
- [ ] 仓库已创建（Public）
- [ ] HTML文件已重命名为 `index.html`
- [ ] 文件已上传到仓库
- [ ] GitHub Pages已启用
- [ ] 网站可以访问
- [ ] 已提交到Google Search Console

## 🆓 费用说明

- GitHub Pages: **完全免费**
- 流量限制: 每月100GB（对个人网站足够）
- 存储限制: 1GB
- 无需信用卡

## 🔧 常见问题

**Q: 网站显示404错误？**
A: 确认文件名是 `index.html` (小写)，并且GitHub Pages已启用

**Q: 更新后网站没变化？**
A: 清除浏览器缓存，或等待2-5分钟

**Q: 想使用自己的域名？**
A: 在Settings → Pages中，可以添加Custom domain

**Q: 网站访问速度慢？**
A: GitHub Pages使用CDN，全球访问速度都很快

## 📞 需要帮助？

如果遇到问题：
1. 查看GitHub Pages文档：https://docs.github.com/pages
2. 检查仓库的 Actions 标签页查看部署状态
3. 确保仓库是Public（公开）状态

---

🎉 部署成功后，你的产品页面就可以被全世界访问了！
