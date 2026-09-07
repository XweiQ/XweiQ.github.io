# Xiaowei Qian 的个人学术主页

线上地址：[xweiq.github.io](https://xweiq.github.io/)。

本站使用 Jekyll 构建、GitHub Pages 发布。当前布局基于 [Arvid Academic Homepage Template](https://github.com/Arvid-pku/Academic-Homepage-Template)，配合定制的 Palatino 排版、酒红标题与墨蓝链接。

## 修改内容

- `_pages/about.md`：个人介绍、Biography、精选论文、Education、Service。
- `_data/publications.yml`：完整论文数据；`selected: true` 的论文出现在首页。
- `_includes/arvid-paper.html`：统一渲染论文标题、作者、会议年份及链接。
- `_pages/publications.html`：完整论文页，分为 Preprints 和 Conference。
- `_config.yml`：姓名、邮箱、社交链接及站点信息。
- Projects 与 CV 暂时留空；Blogs、Photography 保留入口与占位内容。

## 调整外观

在 `assets/css/arvid/typography.css` 顶部修改：

- `--nav-color`、`--nav-active-color`：导航、姓名、各级标题、完整列表入口、论文荣誉标注。
- `--primary-color`、`--secondary-color`：论文标题及其他正文链接。
- `--font-heading`、`--font-body`、`--font-ui`：标题、正文、界面字体。
- `--title-size`、`--section-size`、`--body-size`：各级字号。

页面宽度和页边距在 `shared-styles.css` 中；照片、个人介绍和 Education 的布局在 `homepage.css` 中。

深色模式的按钮与初始化调用已注释，代码未删除。恢复时需同时取消 `site-shell.js` 中按钮的注释，以及两个 Arvid 布局中 `initializeDarkMode()` 的注释，并重新检查深色配色。

## 本地预览与发布

安装依赖后运行 `bundle exec jekyll serve --host 127.0.0.1 --port 4000`。当前电脑可使用以下已有环境：

```sh
JEKYLL_NO_BUNDLER_REQUIRE=true jekyll serve \
  --destination /Users/silver/.cache/blog-preview/manual-site \
  --host 127.0.0.1 --port 4001
```

提交并推送到 `main` 后，在 GitHub Actions 检查 `pages build and deployment`。样式与脚本使用构建时间作为版本参数，避免新页面继续引用旧缓存；已打开的页面需要刷新。

## 模板来源

当前模板和修改范围见 [UPSTREAM.md](../assets/css/arvid/UPSTREAM.md)。早期网站基于 AcadHomepage，部分 Jekyll 基础设施仍然保留，因此原有许可证和版权声明继续保留；它不再是当前页面的设计模板。
