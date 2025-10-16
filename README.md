# Tailwind CSS Translator

一个优雅的双向转换工具，用于在 Tailwind CSS 类名和原生 CSS 样式之间进行转换。

## 🚀 在线访问

访问 [GitHub Pages](https://y1j2x34.github.io/tailwind-translater/) 查看在线版本

## 📦 本地运行

1. 克隆仓库:
```bash
git clone https://github.com/y1j2x34/tailwind-translater.git
cd tailwind-translater
```

2. 使用任意 HTTP 服务器运行:
```bash
# 使用 Python
python -m http.server 8000

# 使用 Node.js
npx http-server

```

3. 在浏览器中访问 `http://localhost:8000`

## 💡 使用示例

### 搜索模式

1. **搜索 Tailwind 类名**:
   - 输入: `bg-blue-500`
   - 结果: `background-color: rgb(59 130 246);`

2. **搜索 CSS 属性**:
   - 输入: `margin`
   - 结果: 显示所有包含 margin 的 Tailwind 类名

### CSS转换模式

1. **单行CSS转换**:
   - 输入: `background-color: blue;`
   - 结果: 推荐的 Tailwind 类名（如 `bg-blue-500`）

2. **多行CSS转换**:
   ```css
   background-color: rgb(59 130 246);
   padding: 1rem;
   margin: 0.5rem;
   display: flex;
   ```
   - 结果: `bg-blue-500 p-4 m-2 flex`（组合所有对应的 Tailwind 类名）

3. **智能匹配**:
   - 精确匹配：显示完全对应的 Tailwind 类名（绿色标签）
   - 相似匹配：显示最接近的 Tailwind 类名（黄色标签）
   - 无匹配：提示使用 Tailwind 任意值语法

## 📝 数据来源

`tailwind-classes-style-map.json` 文件包含了完整的 Tailwind CSS 类名到 CSS 样式的映射关系。

## 🤝 贡献

欢迎提交 Issue 和 Pull Request！

## 📄 许可证

MIT License

