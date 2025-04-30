🧮 Excel Clone


A web-based Excel clone built using Vanilla JavaScript, HTML, and CSS, mimicking core spreadsheet functionalities such as cell formatting, formula evaluation, and multi-sheet support.

✨ Features
2D grid of rows and columns (A-Z, 1–100)

Formula bar with dependency handling

Text styling: bold, italic, font size/type, alignment

Multiple sheets with independent data

Formula parsing using DFS for dependencies and infix stack evaluation

🧠 Core Concepts
Grid & Addressing
Grid: 100 rows × 26 columns

Address format: Column + Row (e.g., A1, B2)

Each cell assigned a rowId and colId during grid construction

Data Storage
Each sheet is a 2D array of cell objects:

js
Copy
Edit
{ name: "A1", value: "", formula: "", parents: [], childrens: [], isBold: false }
All sheets stored in a 3D array: db = [sheet1, sheet2, ...]

Cell Formatting
Button click → get active cell → update DOM + database

➗ Formula Handling
Formulas like =A1+B2 are parsed and evaluated

Dependency tree built using DFS

On input change, all dependent formulas auto-update

📂 Project Structure
bash
Copy
Edit
/excel-clone
├── index.html
├── style.css
├── script.js
✅ TODO
CSV/Excel import-export

Formula function support (SUM, AVG, etc.)

Undo/redo, autosave

📄 License
MIT License

************************************************************

Here’s a simple setup and run guide you can add to your README.md under a section like ## 🚀 Getting Started:

🚀 Getting Started
📥 Clone the Repository
bash
Copy
Edit
git clone https://github.com/yourusername/excel-clone.git
cd excel-clone
🧾 Run the Project
Since this is a pure HTML/CSS/JS project (no backend or build tools), you can run it by simply opening the index.html file:

Option 1: Open in Browser
Double-click index.html
OR

Right-click and choose “Open with” → your browser

 Option 2: Use a Live Server (Recommended for Development)
If you have VS Code:

Install the “Live Server” extension

Right-click index.html → “Open with Live Server”

**Screenshot*
![2025-04-30](https://github.com/user-attachments/assets/6218ebd9-ef97-4334-ac19-515bfbf7a609)
