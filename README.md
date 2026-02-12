# Blog Test

使用 VitePress 构建的博客站点，用于存档 AI 翻译的长文。

> 示例文章：[《大事正在发生》](https://soar4ever.github.io/blog-test/blog/big-things-happening) - Matt Shumer 对 AI 发展的深度思考

---

## 本地开发

```bash
# 安装依赖
npm install

# 启动开发服务器
npm run docs:dev

# 构建
npm run docs:build

# 预览构建结果
npm run docs:preview
```

## 部署到 GitHub Pages

### 第一步：推送到 GitHub

```bash
# 在你的 GitHub 上创建一个名为 blog-test 的仓库（不要初始化）

# 然后执行：
git init
git add .
git commit -m "init vitepress blog"
git branch -M main
git remote add origin https://github.com/soar4ever/blog-test.git
git push -u origin main
```

### 第二步：开启 GitHub Pages

1. 进入仓库的 **Settings** → **Pages**
2. **Source** 选择 **GitHub Actions**
3. 返回仓库主页，点击 **Actions** 标签，确认 workflow 运行成功

### 第三步：访问站点

部署完成后，访问：
```
https://soar4ever.github.io/blog-test/
```

---

## 添加新文章

1. 在 `docs/blog/` 目录下创建新的 `.md` 文件
2. 在 `docs/.vitepress/config.mjs` 中更新 sidebar 配置
3. 提交并推送，GitHub Actions 会自动重新部署

## 技术栈

- [VitePress](https://vitepress.dev/) - 静态站点生成器
- GitHub Actions - 自动部署
- GitHub Pages - 免费托管

---

*由 AI 辅助生成*
