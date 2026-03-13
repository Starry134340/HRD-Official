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
├── CNAME               # 自定义域名配置（如使用自定义域名）
├── README.md           # 说明文档
└── .gitignore          # Git忽略文件
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

2. **自定义域名（去掉GitHub账号名）**
   
   如果您想使用自定义域名（如 `https://hrd.com`），需要以下步骤：
   
   **步骤1：购买域名**
   - 在域名注册商（如阿里云、腾讯云、GoDaddy等）购买域名
   - 常见域名：`.com`、`.cn`、`.net` 等
   
   **步骤2：配置CNAME文件**
   - 编辑项目根目录的 `CNAME` 文件
   - 将 `yourdomain.com` 替换为您的实际域名（如 `hrd.com`）
   - 提交并推送到GitHub
   
   **步骤3：在GitHub设置自定义域名**
   - 访问：https://github.com/Starry134340/HRD-Official/settings/pages
   - 在 "Custom domain" 部分输入您的域名（如 `hrd.com`）
   - 勾选 "Enforce HTTPS"（强制HTTPS）
   - 点击 "Save" 保存
   
   **步骤4：配置DNS记录**
   - 登录您的域名注册商管理后台
   - 添加DNS记录：
     - **方式A（推荐）**：添加CNAME记录
       - 类型：CNAME
       - 主机记录：@（或留空，表示主域名）
       - 记录值：`starry134340.github.io`
     - **方式B**：添加A记录（如果域名不支持CNAME）
       - 类型：A
       - 主机记录：@
       - 记录值：`185.199.108.153`、`185.199.109.153`、`185.199.110.153`、`185.199.111.153`
       - （需要添加4条A记录，分别指向这4个IP）
   
   **步骤5：等待DNS生效**
   - DNS配置通常需要几分钟到几小时生效
   - 配置完成后，访问您的自定义域名即可
   - GitHub会自动为您的域名配置SSL证书（HTTPS）
   
   **注意事项：**
   - 如果使用 `www` 子域名（如 `www.hrd.com`），需要额外配置
   - 确保CNAME文件中的域名与DNS配置一致
   - 自定义域名配置后，原GitHub Pages URL仍然可以访问

3. **HTTPS**
   - GitHub Pages自动提供HTTPS支持
   - 无需额外配置SSL证书

## 📞 技术支持

如有问题，请查看GitHub Pages官方文档：https://docs.github.com/en/pages

