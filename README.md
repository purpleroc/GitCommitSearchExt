# Git Commit Search

🔍 Search keywords in all Git commits and branches with enhanced user experience and smart caching.

![Usage](https://raw.githubusercontent.com/purpleroc/pics/main/vsext/usage.png)

## ✨ What's New in v1.6.0

### 🎯 Enhanced Search Input
- **Real Input Field**: Direct HTML input box in the SEARCH area - no more popup dialogs
- **Instant Search**: Type keyword and press Enter or click "Search" button
- **Smooth Experience**: Seamless workflow without interruptions

### 📚 Smart Search History
- **Instant Feedback**: Keywords appear immediately in KEYWORD area when search starts
- **Real-time Status**: Shows "searching..." while processing, then updates with commit count
- **Automatic History**: All searches are automatically saved in the KEYWORD area  
- **Quick Access**: Click any completed history item to instantly re-run that search
- **Smart Caching**: Previously searched results are cached for instant access
- **Auto Deduplication**: No duplicate entries, keeps history clean
- **Capacity Management**: Maintains up to 10 recent searches

### ⚡ Performance Optimizations
- **Result Caching**: Search results are cached to avoid redundant Git operations
- **Instant History Loading**: Cached results load immediately when accessing history
- **Improved Response Time**: Faster searches for previously queried keywords

## 🚀 How to Use

### 1. Launch the Extension
Click the 'CommitSearch' icon in the Activity Bar

### 2. Perform Searches 🔍
1. **Type directly** in the input field in the SEARCH area
2. **Press Enter** or **click "Search"** to execute
3. **View results** instantly in the COMMITS area below

### 3. Use Search History 🔄
- **Recent Searches**: All search history displayed in KEYWORD area
- **History Entries**: Listed as "keyword (X commits)" in chronological order (most recent first)
- **Quick Reload**: Click any history entry for instant re-search

### 4. Explore Results 📂
- **COMMITS Area**: Browse all matching Git commits
- **File Changes**: Click any commit to view modified files
- **FILES Area**: Examine the list of changed files
- **Diff View**: Click files to see detailed changes

## 🛠️ Core Features

- **Repository-wide Search**: Search across all commits and branches
- **Detailed Commit Info**: Author, timestamp, signature status, and more
- **File Diff Visualization**: Side-by-side comparison of file changes
- **Keyboard Shortcuts**: `Ctrl+Shift+L` / `Cmd+Shift+L` for quick access
- **Cross-platform**: Works on Windows, macOS, and Linux

## 📋 Requirements

- VS Code 1.0.0 or higher
- Git repository (local or remote)
- Git installed and accessible in PATH

## 🎨 Interface Layout

```
CommitSearch (Activity Bar)
├── Search (Input Interface)
│   ├── [Input Field] Enter search keyword...
│   └── [Search Button]
├── Keyword (Search History)
│   ├── Recent Search 1 (X commits)
│   ├── Recent Search 2 (Y commits)
│   └── Recent Search 3 (Z commits)
├── Commits (Search Results)
│   └── List of matching Git commits
└── Files (File Changes)
    └── Modified files in selected commit
```
