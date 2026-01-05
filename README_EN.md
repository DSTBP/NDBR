<p align="center">
  <a href="https://github.com/DSTBP/NDBR" title="点击访问">
    <img width="100" height="100" src="https://github.com/DSTBP/NDBR/blob/main/favicon.png?raw=true" alt="Notion 数据库批量替换助手">
  </a>
</p>


<h1 align="center">Notion Database Batch Replace</h1>

<p align="center">
  <img src="https://img.shields.io/badge/TamperMonkey-v5.0+-brightgreen.svg?style=flat-square" alt="tampermonkey">
  <a href="LICENSE">
    <img src="https://img.shields.io/badge/license-MIT-lightgrey.svg?style=flat-square" alt="LICENSE">
  </a>
  <img src="https://img.shields.io/badge/Notion-3.1.23-blue.svg?style=flat-square" alt="notion">
  <img src="https://img.shields.io/badge/Platform-Windows%20%7C%20Mac%20%7C%20Linux-blue.svg?style=flat-square" alt="platform">
</p>

<div align="center">
  <h3>
    <a href="#-usage-guide">
      Instructions
    </a>
    <span> | </span>
    <a href="#-installation">
      Install
    </a>
    <span> | </span>
    <a href="https://github.com/DSTBP/NDBR/issues">
      Report Bug
    </a>
  </h3>
</div>

<div align="center">
  <strong>👉 A powerful, intelligent tool for batch replacement in Notion databases 👈</strong><br>
  <sub>Automated Z-Scan traversing for Windows, macOS, and Linux</sub>
</div>
<br>

[中文文档](README.md) | [English Docs](README_EN.md)

【Notion Database Batch Replace】 is an open-source Tampermonkey script designed to fix the lack of native batch find-and-replace in Notion. It automates human-like interaction with a Z-pattern scanning logic across all columns and pages.



## 📖 Usage Guide

1. **Prerequisite**: Ensure Tampermonkey is installed.

2. **Open Panel**: Click the floating icon on your Notion page to expand.

3. **Configure**: Enter "Find" and "Replace with" values.

4. **Execute**: Click "Start Auto Replace". The script will sweep horizontally and scroll vertically.

5. **Abort**: Click the red "Stop" button or press **`ESC`**.

   

## 🔧 Features

- ✅ **Z-Scan Engine**: Sweeps columns horizontally and scrolls pages vertically.

- ✅ **Precision Targeting**: Penetrates deep cell editors to avoid row-selection bugs.

- ✅ **Anti-Hijack UI**: Supports `Ctrl+A` / `Ctrl+V` inside UI inputs.

- ✅ **Draggable UI**: Header-based dragging for panel positioning.

- ✅ **Collapsible**: Shrinks into a draggable, custom SVG icon.

  

## 💽 Installation

Ensure [Tampermonkey](https://www.tampermonkey.net/) is installed.

### 1. Direct Install (Recommended)
- **[Click here to install the latest version](https://greasyfork.org/zh-CN/scripts/561380-notion-database-batch-replace)**

### 2. Manual Installation
1. Open Tampermonkey **Dashboard**.

2. Click the **"+" (Add New Script)** button.

3. Clear the default code in the editor.

4. Copy and paste the entire content from `Notion Database Batch Replace.user.js`.

5. Press `Ctrl + S` or click **"File" -> "Save"**.

   

## 🎨 Interface

![](https://github.com/DSTBP/NDBR/blob/main/asserts/UI.png?raw=true)

**Demonstration animation**

  ![](https://github.com/DSTBP/NDBR/blob/main/asserts/Demonstration.gif?raw=true)

## ⚠️ Notes

- **Data Backup**: Always **backup your database page** before running the script.

- **Property Support**: Supports **Text, Number, URL, Email, Phone**. Complex properties like Relations or Dates are currently unsupported.

- **Loading Speed**: For large databases, consider increasing the `sleep` timer in the source code.

- **Keep Focused**: Keep the browser window in the foreground during the process.

  

## ⚖️ Disclaimer

This tool is for educational and personal productivity use only. Users assume full responsibility for any data changes (including errors or losses) resulting from the use of this script. The developer is not liable for any losses incurred.



## 📝 Changelog

- **v1.0.0**: Optimized UI anchoring, and introduced the Z-Scan automated scrolling engine.
- **v1.0.1**：Fixed input shortcut hijacking.