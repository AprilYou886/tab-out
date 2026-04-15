# Tab Out

**Keep tabs on your tabs.**

Tab Out is a Chrome extension that replaces the new tab page with a cleaner workspace for browsing. It keeps your search experience front and center, shows frequently used shortcuts, adds a left bookmarks sidebar, and turns open tabs into a grouped dashboard you can actually clean up.

No server. No account. No external API calls. Just a Chrome extension.

---

## English

### Install With A Coding Agent

Send your coding agent (Codex, Claude Code, etc.) this repo and say **"install this"**:

```text
https://github.com/AprilYou886/tab-out
```

---

### Features

- **Google-style new tab layout** with centered search and frequent shortcuts
- **Frequent shortcuts row** with support for add, edit, and remove
- **Left bookmarks sidebar** for quick access without taking over the main content area
- **Open tabs grouped by domain** so cleanup is much easier
- **Homepage grouping** for Gmail, GitHub, YouTube, X, LinkedIn, and similar landing pages
- **Duplicate detection** with one-click dedupe
- **Jump to any open tab** across Chrome windows
- **Close tabs with style** using synthesized swoosh audio and confetti
- **Save for later** checklist stored locally in `chrome.storage.local`
- **Expandable groups** for larger tab sets
- **100% local** with no backend, login, or sync service required

---

### Manual Setup

**1. Clone the repo**

```bash
git clone https://github.com/AprilYou886/tab-out.git
cd tab-out
```

**2. Load the extension in Chrome**

1. Open `chrome://extensions`
2. Turn on **Developer mode**
3. Click **Load unpacked**
4. Select the `extension/` folder inside this repo

**3. Open a new tab**

You should now see Tab Out.

---

### What The Product Looks Like Now

When you open a new tab, Tab Out gives you:

- A centered search box
- A row of frequent shortcuts
- A left bookmarks sidebar
- Your currently open tabs grouped into cleanup-friendly cards
- A saved-for-later column when you use the bookmark-for-later flow

---

### How It Works

```text
Open a new tab
  -> Search or type a URL
  -> Use frequent shortcuts or bookmarks from the left sidebar
  -> Review open tabs grouped by domain
  -> Jump to a tab, close duplicates, or close a whole group
  -> Save tabs for later before closing them
```

Everything runs inside the extension. Data is stored locally in Chrome storage.

---

### Tech Stack

| What | How |
|------|-----|
| Extension | Chrome Manifest V3 |
| Storage | `chrome.storage.local` |
| Tabs data | `chrome.tabs` |
| Bookmarks | `chrome.bookmarks` |
| Frequent shortcuts | `chrome.topSites` + local shortcut preferences |
| Sound | Web Audio API |
| Effects | CSS transitions + JS confetti |

---

## 中文

### 让 Coding Agent 帮你安装

把下面这个仓库地址发给你的 Coding Agent（比如 Codex、Claude Code 等），然后说一句 **“install this”**：

```text
https://github.com/AprilYou886/tab-out
```

---

### 当前版本功能

- **接近 Google 原生的新标签页布局**，中间是搜索框和常用网址
- **常用网址快捷入口**，支持新增、编辑、删除
- **左侧书签侧边栏**，方便快速访问书签，不占用中间主区域
- **按域名分组展示当前打开的标签页**
- **首页标签自动归组**，例如 Gmail、GitHub、YouTube、X、LinkedIn 等
- **重复标签检测**，支持一键清理重复页
- **点击标题直接跳转到对应标签页**，支持跨窗口切换
- **带音效和撒花的关闭动效**
- **稍后阅读清单**，数据保存在本地 `chrome.storage.local`
- **大分组支持展开查看更多标签**
- **100% 本地运行**，没有服务端、没有账号、没有外部 API

---

### 手动安装

**1. 克隆仓库**

```bash
git clone https://github.com/AprilYou886/tab-out.git
cd tab-out
```

**2. 在 Chrome 中加载扩展**

1. 打开 `chrome://extensions`
2. 打开右上角 **Developer mode**
3. 点击 **Load unpacked**
4. 选择仓库里的 `extension/` 文件夹

**3. 打开一个新标签页**

你就会看到 Tab Out。

---

### 当前产品形态

现在的新标签页会同时提供：

- 中间搜索框
- 一排常用网址
- 左侧书签侧边栏
- 按域名整理的标签页看板
- “稍后阅读”侧栏（当你使用该功能时出现）

---

### 工作方式

```text
打开一个新标签页
  -> 在中间搜索或输入网址
  -> 使用常用网址，或从左侧书签栏进入目标页面
  -> 查看按域名分组的已打开标签页
  -> 快速跳转、关闭重复页、关闭整组标签
  -> 关闭前可先保存到稍后阅读
```

整个产品都运行在 Chrome 扩展内部，数据只保存在本地。

---

### 技术实现

| 模块 | 方案 |
|------|------|
| 扩展 | Chrome Manifest V3 |
| 本地存储 | `chrome.storage.local` |
| 标签读取 | `chrome.tabs` |
| 书签读取 | `chrome.bookmarks` |
| 常用网址 | `chrome.topSites` + 本地快捷方式配置 |
| 音效 | Web Audio API |
| 动效 | CSS transitions + JS confetti |

---

## License

MIT

---

Built by [Zara](https://x.com/zarazhangrui)
