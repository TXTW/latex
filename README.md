# LaTeX 公式编辑器

在线 LaTeX 公式编辑器，支持实时预览、符号面板、工具栏下拉菜单、导出功能。

**在线访问**：https://txtw.github.io/latex_edit/

## 功能

- 实时 KaTeX 渲染预览
- 符号面板（希腊字母、关系运算、箭头、函数等）
- 工具栏下拉菜单（分数、角标、积分、矩阵等，支持占位符跳转）
- 光标同步（输入光标位置同步显示在预览区）
- 点击预览跳转到对应输入位置
- 模板库（常用公式一键插入）
- 矩阵/分段函数对话框（可设置行列数）
- 浅色/深色主题切换
- 导出为 SVG / PNG / LaTeX / MathML
- 历史记录（自动保存到 localStorage）

## 部署

纯静态项目，无需构建。直接将 `index.html` 部署到任意静态托管服务即可。

### GitHub Pages

项目已配置 GitHub Pages，从 `master` 分支的根目录自动部署。

### 本地预览

```bash
# 使用 Python
python -m http.server 8080

# 使用 Node.js
npx serve .
```

然后访问 http://localhost:8080

## 技术栈

- [KaTeX](https://katex.org/) - LaTeX 数学公式渲染
- [html2canvas](https://html2canvas.hertzen.com/) - PNG 导出
- 纯 HTML/CSS/JavaScript，无框架依赖
