# Git Commit Search

🔍 Search keywords in all Git commits and branches with enhanced user experience and smart caching.

在Git提交和分支中搜索关键词，具有增强的用户体验和智能缓存功能。

![Usage](https://raw.githubusercontent.com/purpleroc/pics/main/vsext/usage.png)

## ✨ What's New in v1.7.0 / v1.7.0 新功能

### 🎯 Enhanced Search Input / 增强的搜索输入
- **Real Input Field**: Direct HTML input box in the SEARCH area - no more popup dialogs
- **Instant Search**: Type keyword and press Enter or click "Search" button
- **Smooth Experience**: Seamless workflow without interruptions

- **真正的输入框**: 在SEARCH区域直接显示HTML输入框，无需弹框
- **即时搜索**: 输入关键词后按Enter键或点击"Search"按钮
- **流畅体验**: 无缝的工作流程，无中断

### 📚 Smart Search History / 智能搜索历史
- **Instant Feedback**: Keywords appear immediately in KEYWORD area when search starts
- **Real-time Status**: Shows "searching..." while processing, then updates with commit count
- **Automatic History**: All searches are automatically saved in the KEYWORD area  
- **Quick Access**: Click any completed history item to instantly re-run that search
- **Smart Caching**: Previously searched results are cached for instant access
- **Auto Deduplication**: No duplicate entries, keeps history clean
- **Capacity Management**: Maintains up to 10 recent searches

- **即时反馈**: 搜索开始时关键词立即出现在KEYWORD区域
- **实时状态**: 处理时显示"searching..."，完成后更新提交数量
- **自动历史**: 所有搜索自动保存在KEYWORD区域
- **快速访问**: 点击任意已完成的历史项目立即重新搜索
- **智能缓存**: 之前搜索的结果被缓存以便即时访问
- **自动去重**: 无重复条目，保持历史清洁
- **容量管理**: 维护最多10个最近的搜索

### ⚡ Performance Optimizations / 性能优化
- **Result Caching**: Search results are cached to avoid redundant Git operations
- **Instant History Loading**: Cached results load immediately when accessing history
- **Improved Response Time**: Faster searches for previously queried keywords
- **Complete Case Insensitive Search**: Both file content and commit message searches ignore case differences (e.g., "Test" finds "test", "TEST")
- **Smart History Management**: Clicking existing keywords doesn't reorder the history list

- **结果缓存**: 搜索结果被缓存以避免冗余的Git操作
- **即时历史加载**: 访问历史时缓存结果立即加载
- **改进响应时间**: 对之前查询的关键词进行更快的搜索
- **完整的大小写不敏感搜索**: 文件内容和提交消息搜索都忽略大小写差异（例如，"Test"找到"test"、"TEST"）
- **智能历史管理**: 点击现有关键词不会重新排序历史列表

## 🚀 How to Use / 使用方法

### 1. Launch the Extension / 启动插件
Click the 'CommitSearch' icon in the Activity Bar

点击活动栏中的 'CommitSearch' 图标

### 2. Perform Searches 🔍 / 执行搜索
1. **Type directly** in the input field in the SEARCH area
2. **Press Enter** or **click "Search"** to execute
3. **View results** instantly in the COMMITS area below

1. **直接在SEARCH区域的输入框中输入**
2. **按Enter键或点击"Search"执行**
3. **在下方COMMITS区域立即查看结果**

### 3. Use Search History 🔄 / 使用搜索历史
- **Recent Searches**: All search history displayed in KEYWORD area
- **History Entries**: Listed as "keyword (X commits)" in chronological order (most recent first)
- **Quick Reload**: Click any history entry for instant re-search
- **Stable Order**: Clicking existing entries doesn't change the list order
- **Case Insensitive**: Searches for "Test" and "test" are treated as the same

- **最近搜索**: 所有搜索历史显示在KEYWORD区域
- **历史条目**: 按时间顺序列出为"keyword (X commits)"（最新的在前）
- **快速重载**: 点击任意历史条目立即重新搜索
- **稳定顺序**: 点击现有条目不会改变列表顺序
- **大小写不敏感**: "Test"和"test"的搜索被视为相同

### 4. Explore Results 📂 / 探索结果
- **COMMITS Area**: Browse all matching Git commits
- **File Changes**: Click any commit to view modified files
- **FILES Area**: Examine the list of changed files
- **Diff View**: Click files to see detailed changes

- **COMMITS区域**: 浏览所有匹配的Git提交
- **文件变更**: 点击任意提交查看修改的文件
- **FILES区域**: 检查更改的文件列表
- **差异视图**: 点击文件查看详细更改

## 🛠️ Core Features / 核心功能

- **Repository-wide Search**: Search across all commits and branches
- **Detailed Commit Info**: Author, timestamp, signature status, and more
- **File Diff Visualization**: Side-by-side comparison of file changes
- **Keyboard Shortcuts**: `Ctrl+Shift+L` / `Cmd+Shift+L` for quick access
- **Cross-platform**: Works on Windows, macOS, and Linux

- **全仓库搜索**: 在所有提交和分支中搜索
- **详细提交信息**: 作者、时间戳、签名状态等
- **文件差异可视化**: 文件变更的并排比较
- **键盘快捷键**: `Ctrl+Shift+L` / `Cmd+Shift+L` 快速访问
- **跨平台**: 支持 Windows、macOS 和 Linux

## 📋 Requirements / 系统要求

- VS Code 1.0.0 or higher
- Git repository (local or remote)
- Git installed and accessible in PATH

- VS Code 1.0.0 或更高版本
- Git 仓库（本地或远程）
- Git 已安装并可在 PATH 中访问

## 🎨 Interface Layout / 界面布局

```
CommitSearch (Activity Bar) / CommitSearch (活动栏)
├── Search (Input Interface) / Search (输入界面)
│   ├── [Input Field] Enter search keyword... / [输入框] 输入搜索关键词...
│   └── [Search Button] / [搜索按钮]
├── Keyword (Search History) / Keyword (搜索历史)
│   ├── Recent Search 1 (X commits) / 最近搜索 1 (X 个提交)
│   ├── Recent Search 2 (Y commits) / 最近搜索 2 (Y 个提交)
│   └── Recent Search 3 (Z commits) / 最近搜索 3 (Z 个提交)
├── Commits (Search Results) / Commits (搜索结果)
│   └── List of matching Git commits / 匹配的 Git 提交列表
└── Files (File Changes) / Files (文件变更)
    └── Modified files in selected commit / 选中提交中修改的文件
```
