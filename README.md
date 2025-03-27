# AWS Deployment Sanity & Regression Report Viewer

## Overview
This project is a web-based report viewer that displays AWS deployment sanity and regression reports using **Tabulator.js**. It allows users to view, filter, and analyze reports based on different test environments.

## Features
- 📊 **Dynamic Table with Tabulator.js** for interactive data visualization.
- 📅 **Date Range Filter** to filter reports between specific dates.
- 🎨 **Color-Coded Status** for quick identification (Green, Amber, Red).
- 🔄 **Pagination & Sorting** for efficient browsing.
- ⏩ **Clear Filters Button** for resetting applied filters.

## Setup & Installation
### Prerequisites
- Install Python (for local hosting) or use a static server.

### Steps
1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-repo/aws-report-viewer.git
   cd aws-report-viewer
   ```
2. **Run a Local Server**
   - Using Python:
     ```bash
     python -m http.server 8000
     ```
   - Open `http://localhost:8000/` in your browser.

## Project Structure
```
📂 aws-report-viewer/
 ├── 📄 index.html          # Main UI
 ├── 📄 script.js           # JavaScript logic (filters, table rendering)
 ├── 📄 styles.css          # Styling for the UI
 ├── 📂 static/
 │   ├── 📄 data.json       # JSON file containing report data
```

## Usage
1. **Load Reports:** Automatically loads reports from `data.json`.
2. **Filter by Date Range:**
   - Select **From Date** and **To Date**, then click **Apply**.
3. **Reset Filters:** Click **Clear Filters** to remove all filters.

## JSON Data Format
Example JSON:
```json
{
  "reports": [
    {
      "date": "27/03/2025",
      "checks": [
        {
          "activity": "Sanity",
          "domains": [
            { "name": "BUY", "INT-Done": "Amber", "TEST-Done": "Green" }
          ]
        }
      ]
    }
  ]
}
```

## Contribution
1. Fork the repository.
2. Create a feature branch.
3. Submit a pull request.

## License
MIT License

