# Daily Papers 论文分享平台

## 📖 介绍

这是一个用于分享和管理 Daily Papers（每日论文）的网站。支持论文搜索、分类浏览和标签管理。

## 🚀 快速开始

### 访问网站
- **主页面**：`https://davidwisdom.github.io/papers.html`
- **功能**：
  - 🔍 **搜索**：按标题、作者搜索论文
  - 🏷️ **分类**：AI、NLP、CV、ML、其他
  - 📅 **日期**：查看论文发布时间

## 📝 如何添加论文

### 方式一：直接编辑 HTML（推荐初期使用）

编辑 `papers.html` 中的 `papersGrid` 部分，添加新的论文卡片：

```html
<div class="paper-card" data-category="ai">
    <div class="paper-date">2024-07-06</div>
    <div class="paper-title">论文标题</div>
    <div class="paper-authors">作者: 作者名字</div>
    <div class="paper-abstract">论文摘要...</div>
    <div class="paper-tags">
        <span class="tag">标签1</span>
        <span class="tag">标签2</span>
    </div>
    <a href="论文链接" class="paper-link">查看详情 →</a>
</div>
```

### 分类说明
- `ai` - 人工智能综合
- `nlp` - 自然语言处理
- `cv` - 计算机视觉
- `ml` - 机器学习
- `other` - 其他

## 📊 建议的数据格式

每篇论文需要包含：
- **日期**：发布日期（YYYY-MM-DD）
- **标题**：论文标题
- **作者**：主要作者及机构
- **摘要**：简短的摘要（100-150字）
- **标签**：2-3个相关标签
- **链接**：ArXiv、论文库或其他来源的链接

## 🔧 自定义

### 修改主题色
编辑 CSS 中的 `background` 渐变色：
```css
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
```

### 添加新分类
1. 在 HTML 中添加新按钮：
```html
<button class="filter-btn" data-category="新分类">新分类</button>
```

2. 在论文卡片中使用该分类：
```html
<div class="paper-card" data-category="新分类">
```

## 💡 后续优化建议

- [ ] 建立数据库存储论文信息（JSON 或数据库）
- [ ] 实现论文详情页面
- [ ] 添加论文评分/收藏功能
- [ ] 集成 ArXiv API 自动获取最新论文
- [ ] 实现用户评论和讨论功能
- [ ] 添加论文分享到社交媒体功能

## 📱 响应式设计

网站已针对不同设备进行优化：
- 🖥️ 桌面版：3列网格布局
- 📱 移动版：单列布局

## 🤝 贡献

欢迎提交 Issue 和 Pull Request！

---

**最后更新**：2024-07-06
