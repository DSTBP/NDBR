# Notion Database Batch Replace

A powerful Tampermonkey script designed to perform deep "Find and Replace" operations across entire Notion databases. It overcomes Notion's **Virtual List** rendering limitations by automating a Z-pattern scroll (horizontal then vertical) to ensure every cell is processed.

## 🌟 Key Features

- **Z-Scan Engine**: Automatically executes a "Scan Columns $\rightarrow$ Scroll Down $\rightarrow$ Repeat" logic to reach every hidden cell in large databases.
- **Precision Targeting**: Bypass Notion's default "Row Selection" behavior. The script penetrates deep into the DOM to activate the specific cell editor.
- **Anti-Hijacking Inputs**: Special event-handling allows you to use standard shortcuts (`Ctrl+A`, `Ctrl+C`, `Ctrl+V`) inside the script UI without triggering Notion's global commands.
- **Interactive UI**:
  - **Draggable**: Move the panel anywhere by dragging the header.
  - **Collapsible**: Shrink the panel into a sleek, custom SVG icon to save space.
  - **Smart Anchoring**: The panel expands to the left from the icon's position, staying perfectly aligned with the screen edge.
- **Safety First**: Press **`ESC`** at any time to immediately abort the scanning and replacement process.

## 🛠️ Installation

1. **Install a Manager**: Install the [Tampermonkey](https://www.tampermonkey.net/) extension for your browser (Chrome, Edge, Safari, or Firefox).
2. **Create Script**:
   - Click the Tampermonkey icon and select "Create a new script".
   - Delete the template code and paste the content of `Notion Database Batch Replace-1.0.0.user.js`.
3. **Save**: Press `Ctrl + S` (or `Cmd + S` on Mac) to save.
4. **Activate**: Navigate to any Notion database page; the custom blue icon will appear in the top-right area.

## 🚀 How to Use

1. **Open Database**: Go to the Notion Table view you wish to modify.
2. **Expand UI**: Click the floating SVG icon to open the control panel.
3. **Configure**:
   - **Find**: Enter the text you want to replace.
   - **Replace with**: Enter the new text.
4. **Execute**: Click **"Start Auto Replace"**.
   - The script will begin auto-scrolling. **Do not click the page** during this process to avoid interrupting the simulated clicks.
   - To stop, click the red **"Stop"** button or hit the **`ESC`** key.
5. **Done**: A summary will appear in the status log once the scan is complete.

## ⚠️ Important Notes

- **Backup Your Data**: Always **duplicate or back up your database** before running a batch replacement. Notion's "Page History" is a lifesaver, but prevention is better than cure.
- **Supported Property Types**: This script works best with **Text**, **Number**, **URL**, **Email**, and **Phone** properties. It may not support "Relation," "Person," or "Date" properties as they use complex menu popups instead of standard text inputs.
- **Performance**: For extremely large databases or slow internet connections, you may need to increase the `sleep` values in the code to allow Notion more time to render cells.

## 📜 Changelog

- **v1.0.0**: Optimize the UI anchoring logic, fix the problem that the shortcut keys of the input box are hijacked by Notion, and introduce the Z-shaped automatic scrolling scanning engine.