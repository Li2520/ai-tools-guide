# AI工具使用指南

一个无需构建的中文静态网站，包含10类、28款精选AI工具，9类用户场景，以及5套Skill / 工作流 / Agent搭建方案。

## 功能

- 工具分类与关键词搜索
- 使用详情、上手步骤和官网跳转
- 场景方案与关联工具导航
- Dify、n8n、LangGraph搭建指南
- 可复制、下载的论文精读SKILL.md模板

## 文件

- `dist/index.html`：页面结构
- `dist/style.css`：样式和响应式布局
- `dist/app.js`：工具数据、交互和方案内容
- `.github/workflows/pages.yml`：GitHub Pages自动部署

## 本地查看

安装Node.js后，在仓库目录运行：

```sh
node preview.cjs
```

浏览器打开 `http://127.0.0.1:4175/`。

## GitHub Pages

在仓库的 **Settings → Pages → Build and deployment** 中，将 **Source** 设为 **GitHub Actions**。

推送到 `main` 或手动运行 `Deploy AI Tools Guide` 工作流即可部署。实际网站地址见工作流部署环境中的链接。

本网站采用相对资源路径，兼容GitHub Pages仓库子路径。无需模型API密钥，也不需要服务器或数据库。

## 更新内容

工具信息、场景和教程位于 `dist/app.js`。修改并推送到 `main` 后，GitHub Actions自动更新网站。

此版本提供教程与模板，不直接调用模型或执行Agent。收费、模型版本、产品开放范围和素材使用许可以官方说明为准。

## 资料来源

基于《AI工具的用户场景需求匹配》和提供的参考截图整理；框架教程参考Dify、n8n、LangGraph和Claude Code官方文档。28款工具为精选目录，并非原资料的完整200+清单。
