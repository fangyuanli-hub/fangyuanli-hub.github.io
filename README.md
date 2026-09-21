# 我的个人主页：使用说明

这个文件不会出现在网站上，只给你自己看。

## 一、第一次上线（约 15 分钟）

1. 登录 GitHub（账号 `fangyuanli-hub`）。
2. 右上角 **+** → **New repository**。
   - 名字必须是：`fangyuanli-hub.github.io`
   - 选 **Public**，点 **Create repository**。
3. 在新仓库页面点 **uploading an existing file**。
   - 把这个文件夹里的**所有文件，连同 `_posts` 文件夹**一起拖进去。
   - 点 **Commit changes**。
4. （可选）上传 CV：
   - 用新版 CV（SimpleOne），另存一份，**先删掉电话号码和地址**。
   - 命名为 `cv.pdf`，同样拖进仓库。
   - 不传的话，页面上的 "CV (PDF)" 链接会打不开。
5. **Settings** → **Pages**：确认 Source 是 "Deploy from a branch"，Branch 是 `main` / `(root)`。
6. 等 1–2 分钟，打开 <https://fangyuanli-hub.github.io>。

## 二、发一篇新文章（约 1 分钟）

1. 打开仓库 → 进入 `_posts` 文件夹 → **Add file** → **Create new file**。
2. 文件名格式：`年-月-日-英文短名.md`
   - 例如：`2026-10-05-astrocyte-idea.md`
3. 内容照这个格式写：

   ```
   ---
   title: "Your title here"
   ---

   Your text here...
   ```

4. 点 **Commit changes**。1–2 分钟后首页就会出现。

注意：

- 文件名里的日期就是发布日期。**日期写成未来的，文章不会显示。**
- 改文章：点开文件 → 铅笔图标 → 修改 → Commit。
- 删文章：点开文件 → **⋯** → Delete file。
- 先存草稿不发布：在开头 `---` 之间加一行 `published: false`。

## 三、Markdown 速查

| 写法 | 效果 |
|---|---|
| `**粗体**` | **粗体** |
| `*斜体*` | *斜体* |
| `## 小标题` | 小标题 |
| `- 项目` | 列表 |
| `[文字](https://链接)` | 链接 |
| `![图注](/images/fig1.png)` | 图片（先把图片上传到 `images` 文件夹） |
| 空一行 | 新段落 |

## 四、常改的地方

- 首页自我介绍：`index.md`
- 论文列表：`publications.md`
  - 未发表的那篇（Noradrenaline）藏在 `{% comment %}` 里，和合作者确认后再放出来。
- 网站名、邮箱、简介：`_config.yml`
- 换照片：用新照片替换 `photo.jpg`，文件名保持不变。

## 五、出问题了？

网站没更新 → 仓库顶部 **Actions** 标签 → 看有没有红叉，点进去看报错。

最常见的错误是开头 `---` 那段格式写错：

- 冒号后面要有空格。
- 标题里有冒号时，整个标题要加引号。
