# HRD公司官网

这是一个使用HTML、CSS和JavaScript构建的静态公司官网，可以通过GitHub Pages在公网访问。

## 🚀 快速开始

### 方式一：使用GitHub Pages（推荐）

1. **创建GitHub仓库**
   - 登录GitHub
   - 点击右上角 "+" 号，选择 "New repository"
   - 仓库名称填写：`HRD-Official`（或您喜欢的名称）
   - 选择 Public（公开仓库）
   - 点击 "Create repository"

2. **上传代码到GitHub**
   ```bash
   # 初始化git仓库
   git init
   
   # 添加所有文件
   git add .
   
   # 提交代码
   git commit -m "Initial commit: 公司官网"
   
   # 添加远程仓库（将YOUR_USERNAME替换为您的GitHub用户名）
   git remote add origin https://github.com/YOUR_USERNAME/HRD-Official.git
   
   # 推送到GitHub（将main改为master如果您的默认分支是master）
   git branch -M main
   git push -u origin main
   ```

3. **启用GitHub Pages**
   - 进入您的GitHub仓库页面：https://github.com/Starry134340/HRD-Official
   - 点击 "Settings"（设置）
   - 在左侧菜单找到 "Pages"
   - 在 "Source" 部分，选择 "Deploy from a branch"
   - Branch选择 "main"，文件夹选择 "/ (root)"
   - 点击 "Save" 保存设置

4. **访问网站**
   - 等待1-2分钟让GitHub Pages完成部署
   - 访问地址：`https://starry134340.github.io/HRD-Official/`
   - 您也可以在仓库的Settings > Pages页面查看部署状态和URL
   - 注意：如果显示404，可能需要等待几分钟让DNS生效

### 方式二：本地预览

1. **使用Python简单服务器**
   ```bash
   # Python 3
   python -m http.server 8000
   
   # Python 2
   python -m SimpleHTTPServer 8000
   ```

2. **使用Node.js服务器**
   ```bash
   # 安装http-server
   npm install -g http-server
   
   # 运行服务器
   http-server -p 8000
   ```

3. **访问**
   - 打开浏览器访问：`http://localhost:8000`

## 📁 项目结构

```
HRD-Official/
├── index.html          # 主页面
├── styles.css          # 样式文件
├── script.js           # JavaScript交互
├── README.md           # 说明文档
└── .github/
    └── workflows/
        └── deploy.yml  # GitHub Actions部署配置
```

## ✨ 功能特性

- ✅ 响应式设计，支持移动端和桌面端
- ✅ 现代化UI设计
- ✅ 平滑滚动导航
- ✅ 联系表单
- ✅ GitHub Pages自动部署

## 🔧 自定义配置

### 修改网站信息

编辑 `index.html` 文件，修改以下内容：
- 公司名称
- 联系方式
- 服务项目
- 产品信息

### 修改样式

编辑 `styles.css` 文件，可以修改：
- 颜色主题（CSS变量在文件顶部）
- 字体大小
- 布局样式

## 📝 注意事项

1. **GitHub Pages限制**
   - 仓库必须是公开的（Public）才能免费使用GitHub Pages
   - 私有仓库需要GitHub Pro账户

2. **自定义域名**
   - 在仓库Settings > Pages中可以设置自定义域名
   - 需要配置DNS记录指向GitHub Pages

3. **HTTPS**
   - GitHub Pages自动提供HTTPS支持
   - 无需额外配置SSL证书

## 📞 技术支持

如有问题，请查看GitHub Pages官方文档：https://docs.github.com/en/pages

