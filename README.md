# 六级精读实验室 · CET-6 Review Hub

一个长期维护的英语六级精读和复习仓库。当前版本整理了 **2025 年 12 月六级第二套的两篇文章**，学习记录始于 **2026-10-19**。

## 在线访问

启用 GitHub Pages 后访问：`https://immkernel.github.io/cet6-review-hub/`

目前首页 `index.html` 是完整的离线可运行网页，无需安装依赖。将 `index.html` 下载到电脑双击也可以使用。

## 现有内容

- 文章精读：AI 与人类工作、给出不请自来的建议，两篇文章中英对照及段落重点
- 词汇积累：核心单词、搭配、词卡与掌握标记
- 语法整理：同位语从句、分词后置定语、让步结构等
- 真题训练：26–35、51–55，共 15 题（其中部分题目为依据考点设计的改写练习，请见网页说明）
- 错题回顾与进度记录
- **进度备份**：在「错题与复习」中点击「导出进度」，需要迁移设备时点击「导入进度」

## 文件结构

```text
cet6-review-hub/
├── index.html                  # 首页：六级复习网页，直接部署到 GitHub Pages
├── archive/
│   └── 2026-10-19.html        # 最初上传的网页快照（未改动）
├── records/
│   ├── README.md              # 学习日期索引
│   └── 2026-10-19.md          # 2026-10-19 学习记录
├── .nojekyll                  # 不经过 Jekyll 处理
└── README.md                  # 仓库使用和维护说明
```

## 如何长期维护

1. **每次学完新真题**，在 `records/` 新建 `YYYY-MM-DD.md`，记录试卷来源、文章内容、重点词汇、长难句和错误原因。
2. **需要新增网站中的题目或单词**，编辑 `index.html` 中 `articles`、`wordbank`、`grammar`、`cloze`、`readingQs` 等数据数组。先本地打开测试，再提交。
3. **每次大幅更新网页前**，把当时的 `index.html` 复制到 `archive/YYYY-MM-DD.html`，保存可回看的历史快照。
4. 在 GitHub 网页的 `Add file → Create new file` 中直接添加笔记，或使用 Git 本地提交。提交后 GitHub Pages 会在构建部署完成后更新网页。
5. 复习进度保存在当前域名/浏览器的 `localStorage` 中，不在 GitHub 仓库中，**不跨设备自动同步**。请定期导出 JSON 文件备份，不要把含个人学习习惯的备份随意提交到公开仓库。

> 注意：不要随意改变 `storageKey`（当前 `cet6_reading_lab_v1`），否则旧的浏览器进度可能读取不到。

## 第一次部署到 GitHub Pages

1. 新建 **Public** 仓库 `cet6-review-hub`，不要初始化 README（直接导入本项目文件）。
2. 将本项目解压后的 **文件和文件夹** 上传到仓库根目录并提交到 `main` 分支。
3. 打开 `Settings → Pages`，在 `Build and deployment` 下选择 **Deploy from a branch**，将 Branch 设为 `main`，目录设为 `/(root)`，然后保存。
4. 等待 GitHub Pages 完成部署，再访问上方的在线地址。网址在仓库的 `Settings → Pages` 中也会显示。

## 版权与用途

本站以个人学习与复习为目的，真题文章及相关材料的版权属于各自权利人。请在公开传播前自行确认使用权限。此仓库不预设开源许可证。
