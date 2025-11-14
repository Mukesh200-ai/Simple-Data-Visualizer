# 🔒 Local CSV Data Visualizer

A simple, 100% private, browser-based tool to instantly chart your CSV data. No sign-ups, no uploads, no tracking.
<img width="1863" height="1015" alt="image" src="https://github.com/user-attachments/assets/41995f3d-e687-4197-92cf-17d64e906719" />

---

## 🤔 Why Use This Tool?

Have you ever wanted to quickly create a chart from a CSV file, but...

* You don't know how to use **complex tools** like Power BI, Tableau, or Qlik?
* You don't want to go through a **long sign-up or installation** process just for a simple graph?
* You are **worried about the privacy of your data** and don't want to upload your sensitive CSV file to a random website?

**This tool is the solution.**

It's a single HTML file that runs **100% in your local web browser.** Your data is never sent to a server, never uploaded, and never seen by anyone but you. It's the perfect tool for quick, simple, and secure data visualization.

---

## ✨ Features

* **100% Private:** Your data never leaves your computer.
* **No Installation:** Just download the `index.html` file and open it in your browser.
* **Two Ways to Load Data:** Paste your CSV data directly or upload a `.csv` file.
* **Dynamic Column Selection:** Automatically reads your CSV headers and lets you choose your X and Y axes.
* **Multi-Chart Support:** Generate **Bar Charts**, **Line Graphs**, and **Pie Charts**.
* **Advanced Comparison:** Toggle a "Compare Multiple Y-Axes" option to plot multiple datasets on a single chart.
    * **Side-by-side** bars for direct comparison.
    * **Overlapping** lines to see trends.
* **Save Your Work:** Download any chart you create as a high-quality PNG file.
* **Error Handling:** C-friendly messages tell you if your data format is incorrect.

---

## 🚀 How to Use

1.  **Download:** Download the `index.html` file from this repository.
2.  **Open:** Double-click the `index.html` file to open it in any modern web browser (like Chrome, Firefox, or Edge).
3.  **Load Data:**
    * **Option A:** Paste your CSV data into the large text box.
    * **Option B:** Click "Choose File" to upload a `.csv` file from your computer.
4.  **Select Columns:** The "Select X-Axis" and "Select Y-Axis" dropdowns will automatically fill with your column headers.
5.  **Configure:**
    * For a simple chart, select one X-axis and one Y-axis.
    * For a comparison chart, check the "Compare Multiple Y-Axes" box and select multiple Y-axes.
6.  **Generate:** Click "Generate Bar Chart," "Generate Line Graph," or "Generate Pie Chart" to see your data!
7.  **Save:** Click "Download Chart" to save the result as a PNG.

---

## ⚙️ How It Works

This tool is intentionally simple. It's a single `index.html` file containing three parts:
1.  **HTML:** Creates the buttons, dropdowns, and text areas.
2.  **CSS:** Provides basic styling to make the tool clean and usable.
3.  **JavaScript:** This is the "brain."
    * It uses `FileReader` to read your uploaded file.
    * It parses the CSV text into arrays.
    * It uses the amazing [Chart.js](https://www.chartjs.org/) library (loaded from a CDN) to draw the charts on an HTML `<canvas>` element.

Since all the logic is in JavaScript that runs in *your* browser, no data ever needs to be sent to a server, guaranteeing your privacy.
