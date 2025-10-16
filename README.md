# Tailwind CSS Translator

一个优雅的双向转换工具，用于在 Tailwind CSS 类名和原生 CSS 样式之间进行转换。

## ✨ 特性

- 🔄 **双向搜索**: 支持通过 Tailwind 类名查找 CSS，或通过 CSS 属性查找 Tailwind 类名
- ⚡ **实时搜索**: 输入即搜索，快速响应
- 🎨 **美观界面**: 使用 Tailwind CSS 设计的现代化 UI
- 📋 **一键复制**: 点击即可复制类名或样式
- 📱 **响应式设计**: 完美支持移动端和桌面端

## 🚀 在线访问

访问 [GitHub Pages](https://你的用户名.github.io/tailwind-translater/) 查看在线版本

## 📦 本地运行

1. 克隆仓库:
```bash
git clone https://github.com/你的用户名/tailwind-translater.git
cd tailwind-translater
```

2. 使用任意 HTTP 服务器运行:
```bash
# 使用 Python
python -m http.server 8000

# 使用 Node.js
npx http-server

# 或直接在浏览器中打开 index.html
```

3. 在浏览器中访问 `http://localhost:8000`

## 🔧 部署到 GitHub Pages

### 自动部署（推荐）

本项目已配置 GitHub Actions 自动部署。按照以下步骤操作：

1. **推送代码到 GitHub**:
```bash
git add .
git commit -m "Initial commit"
git push origin main
```

2. **启用 GitHub Pages**:
   - 进入仓库的 Settings → Pages
   - 在 "Source" 下选择 "GitHub Actions"
   - 保存设置

3. **触发部署**:
   - 每次推送到 `main` 分支时会自动触发部署
   - 也可以在 Actions 标签页手动触发工作流

4. **访问网站**:
   - 部署完成后，访问 `https://你的用户名.github.io/tailwind-translater/`

### 手动部署

如果你想手动部署，可以直接将以下文件上传到 `gh-pages` 分支：
- index.html
- tailwind-classes-style-map.json

## 📁 项目结构

```
tailwind-translater/
├── index.html                          # 主页面
├── tailwind-classes-style-map.json    # Tailwind 类名映射数据
├── .github/
│   └── workflows/
│       └── deploy.yml                 # GitHub Actions 部署配置
└── README.md                          # 项目说明
```

## 🛠️ 技术栈

- **HTML5**: 页面结构
- **Tailwind CSS**: 样式框架（通过 CDN）
- **原生 JavaScript**: 搜索和交互逻辑
- **GitHub Actions**: 自动化部署

## 💡 使用示例

1. **搜索 Tailwind 类名**:
   - 输入: `bg-blue-500`
   - 结果: `background-color: rgb(59 130 246);`

2. **搜索 CSS 属性**:
   - 输入: `margin`
   - 结果: 显示所有包含 margin 的 Tailwind 类名

3. **一键复制**:
   - 悬停在结果上时，点击复制按钮即可复制到剪贴板

## 📝 数据来源

`tailwind-classes-style-map.json` 文件包含了完整的 Tailwind CSS 类名到 CSS 样式的映射关系。

## 🤝 贡献

欢迎提交 Issue 和 Pull Request！

## 📄 许可证

MIT License

## 👨‍💻 作者

Created with ❤️ using Tailwind CSS

