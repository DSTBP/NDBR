- 

- <p align="center">
    <a href="https://github.com/DSTBP/NDBR" title="点击访问">
      <img width="100" height="100" src="https://github.com/DSTBP/NDBR/blob/main/favicon.png?raw=true" alt="Notion 数据库批量替换助手">
    </a>
  </p>


  <h1 align="center">Notion 数据库批量替换助手</h1>

  <p align="center">
    <img src="https://img.shields.io/badge/TamperMonkey-v5.0+-brightgreen.svg?style=flat-square" alt="tampermonkey">
    <a href="LICENSE">
      <img src="https://img.shields.io/badge/license-MIT-lightgrey.svg?style=flat-square" alt="LICENSE">
    </a>
    <img src="https://img.shields.io/badge/Notion-2026-blue.svg?style=flat-square" alt="notion">
    <img src="https://img.shields.io/badge/Platform-Windows%20%7C%20Mac%20%7C%20Linux-blue.svg?style=flat-square" alt="platform">
  </p>

  <div align="center">
    <h3>
      <a href="#-使用教程">
        使用说明
      </a>
      <span> | </span>
      <a href="#-安装助手">
        安装地址
      </a>
      <span> | </span>
      <a href="https://github.com/你的用户名/仓库名/issues">
        提交Bug
      </a>
    </h3>
  </div>

  <div align="center">
    <strong>👉 一个强力、智能的 Notion 数据库内容批量替换工具 👈</strong><br>
    <sub>支持自动 Z 字形全库扫描，适用于 Linux，macOS，Windows 平台</sub>
  </div>
  <br>

  [中文文档](README.md) | [English Docs](README_EN.md)

  【Notion 数据库批量替换助手】是一款免费开源的油猴脚本，专为解决 Notion 数据库无法批量查找替换的痛点而生。它能够模拟人工操作进行全库 Z 字形扫描，支持跨列、跨页面的深度替换，并解决了输入框被 Notion 快捷键劫持的问题。

  

  ## 📖 使用教程

  1. **准备工作**：确保浏览器已安装 Tampermonkey 插件。

  2. **启动面板**：进入 Notion 数据库页面，点击右上角自定义图标展开面板。

  3. **配置参数**：在输入框内填入“查找内容”与“替换为”内容。

  4. **自动扫描**：点击“开始自动替换”，脚本将自动横向遍历所有列并纵向翻页。

  5. **中途停止**：如需停止，请点击红色的“停止扫描”按钮或直接按下键盘 **`ESC`** 键。

     

  ## 🔧 插件功能

  - ✅ **Z 字形深度扫描**：自动横向遍历列，纵向翻页滚动，确保覆盖全库。

  - ✅ **精准单元格定位**：直接穿透至底层编辑器，避免误选整行。

  - ✅ **防焦点劫持**：支持 UI 输入框内正常使用 `Ctrl+A` / `Ctrl+V` 等快捷键。

  - ✅ **交互式 UI**：支持面板标题栏拖拽移动，位置灵活。

  - ✅ **收缩隐藏**：一键收缩为美观的自定义图标，图标亦可自由拖拽。

    

  ## 💽 安装助手

  请确保已先安装 [Tampermonkey](https://www.tampermonkey.net/) 脚本管理器。

  ### 1. 直接安装（推荐）
  - **[点击此处安装最新版本脚本](你的安装地址.user.js)**

  ### 2. 手动安装步骤
  1. 打开 Tampermonkey **管理面板**。

  2. 点击右上角的 **“+” (添加新脚本)**。

  3. 清空编辑器内的默认代码。

  4. 将本仓库中 `Notion Database Batch Replace-1.0.0.user.js` 的**全部代码**复制并粘贴进去。

  5. 按下 `Ctrl + S` 或点击编辑器左上角的 **“文件” -> “保存”**。

     

  ## 🎨 助手界面

  ![](https://github.com/DSTBP/NDBR/blob/main/asserts/UI.png?raw=true)

  

  ## ⚠️ 注意事项

  - **数据备份**：执行大规模替换前，**请务必先复制或备份数据库页面**。

  - **属性支持**：目前完美支持 **Text, Number, URL, Email, Phone**。对于 Relation、Date 等弹窗类属性，脚本暂不支持自动录入。

  - **网络延迟**：若数据库极大且加载缓慢，请在代码中适当调大 `sleep` 延迟时间。

  - **窗口置顶**：运行期间请保持浏览器窗口处于前台，不要最小化，以免影响模拟滚动。

    

  ## ⚖️ 免责声明

  本工具仅供学习和个人工作效率提升使用。使用本脚本所产生的所有数据变更后果（如数据误替换、丢失等）均由使用者自行承担。开发者不对因使用本工具导致的任何形式的损失负责。请在正式操作前于测试数据上充分验证。

  

  ## 📝 更新日志

  - **v1.0.0**：优化 UI 锚定逻辑，修复输入框快捷键被 Notion 劫持的问题，引入 Z 字形自动滚动扫描引擎。