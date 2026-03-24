# 🚀 营销导航网 - 部署指南

## ✅ 已完成

- ✅ `index.html` - 网页主文件
- ✅ `sites.json` - 网址数据（已填充 40+ 个常用营销工具）

---

## 📦 部署到 GitHub Pages（5 分钟）

### 步骤 1：创建 GitHub 仓库

1. 打开 https://github.com/new
2. 仓库名：`marketing-nav`（或你喜欢的名字）
3. 设为 **Public**（公开）
4. 点击 **Create repository**

---

### 步骤 2：上传文件

**方法 A：网页上传（最简单）**

1. 在仓库页面点击 **uploading an existing file**
2. 把这两个文件拖进去：
   - `index.html`
   - `sites.json`
3. 点击 **Commit changes**

**方法 B：命令行上传**

```bash
cd /Users/huangwubing/.openclaw/workspace/projects/marketing-nav
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/你的用户名/marketing-nav.git
git push -u origin main
```

---

### 步骤 3：开启 GitHub Pages

1. 进入仓库 **Settings** → **Pages**
2. **Source** 选择：`Deploy from a branch`
3. **Branch** 选择：`main` / `root`
4. 点击 **Save**
5. 等待 1-2 分钟

---

### 步骤 4：访问你的导航站

部署完成后，访问：
```
https://你的用户名.github.io/marketing-nav/
```

---

## 🎨 功能特性

- ✅ **搜索功能** - 快速查找工具
- ✅ **分类筛选** - 点击分类按钮
- ✅ **响应式设计** - 手机电脑都能用
- ✅ **自动图标** - 抓取网站 favicon
- ✅ **点击跳转** - 新标签页打开

---

## 📝 添加/修改网址

编辑 `sites.json` 文件，格式：

```json
{
  "name": "网站名称",
  "url": "https://example.com",
  "desc": "网站描述",
  "tags": ["标签 1", "标签 2"]
}
```

修改后：
1. 保存文件
2. `git add . && git commit -m "添加新网址"`
3. `git push`
4. 等待 1 分钟自动更新

---

## 🎯 下一步优化（可选）

- [ ] 添加更多网址（你平时用的）
- [ ] 自定义配色主题
- [ ] 添加访问统计
- [ ] 绑定自定义域名
- [ ] 添加用户登录（需要后端）

---

## 💡 分享给团队

把 GitHub Pages 链接发给同事：
- 微信/飞书/钉钉直接发链接
- 手机扫码也能访问
- 可以加入书签/收藏夹

---

## 🆘 遇到问题？

**问题 1：页面显示 404**
- 等 2 分钟，GitHub 需要时间构建
- 检查 Settings → Pages 是否开启

**问题 2：图片不显示**
- 网站图标从 Google 抓取，国内可能慢
- 不影响使用，点击卡片正常跳转

**问题 3：JSON 格式错误**
- 用 https://jsonlint.com/ 检查格式
- 确保逗号、引号成对

---

**需要我帮你部署吗？** 

告诉我你的 GitHub 用户名，我可以：
1. 帮你创建仓库
2. 上传文件
3. 配置 GitHub Pages
4. 给你最终链接

---

*最后更新：2026-03-24*
