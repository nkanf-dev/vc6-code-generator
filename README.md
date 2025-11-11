# VC6 代码截图生成器

一个用于生成 Visual C++ 6.0 风格代码截图和运行结果截图的在线工具。

## 功能特性

- VC6 风格代码语法高亮
- CMD 风格运行结果展示
- 支持多个代码和运行结果
- 可自定义字体大小和字体类型
- 可控制语法高亮类型（关键字、字符串、注释、预处理指令）
- 自动保存内容到本地存储

## 部署到 Cloudflare Pages

### 方法 1：通过 Git 仓库部署（推荐）

1. 创建 GitHub 仓库并上传以下文件：
   - `index.html`
   - `vc6code.html`
   - `FSEX.ttf`

2. 登录 [Cloudflare Dashboard](https://dash.cloudflare.com/)

3. 进入 **Pages** → 点击 **Create a project**

4. 选择 **Connect to Git**

5. 授权并选择你的 GitHub 仓库

6. 配置构建设置：
   - **Framework preset**: None
   - **Build command**: （留空）
   - **Build output directory**: `/`

7. 点击 **Save and Deploy**

### 方法 2：直接上传部署

1. 登录 [Cloudflare Dashboard](https://dash.cloudflare.com/)

2. 进入 **Pages** → 点击 **Create a project**

3. 选择 **Direct Upload**

4. 将以下文件拖拽上传：
   - `index.html`
   - `vc6code.html`
   - `FSEX.ttf`

5. 点击 **Deploy site**

### 部署后访问

- 部署完成后，Cloudflare 会提供一个 `*.pages.dev` 域名
- 也可以在项目设置中添加自定义域名

## 本地使用

直接在浏览器中打开 `index.html` 或 `vc6code.html` 即可使用。

## 技术栈

- 纯 HTML + CSS + JavaScript
- 无需构建工具
- 无外部依赖（除了字体文件）
