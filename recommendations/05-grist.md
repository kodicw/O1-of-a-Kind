# Recommendation 05: Grist vs. Excel

A comparison of relational data management vs. traditional cell-based spreadsheets.

**TL;DR:** Grist is a **relational database** disguised as a spreadsheet, whereas Excel is a **cell-based grid** for ad-hoc calculation.

## Data Structure: Database vs. Grid
*   **Excel:** Operates on a free-form grid. To connect data across tabs, you must rely on fragile `VLOOKUP` chains that easily break.
*   **Grist:** Operates as a relational SQLite database. Columns hold specific data types (text, dates, references), preventing data corruption. Records update globally without broken links.

## Logic & Formulas: Python vs. Proprietary
*   **Excel:** Uses proprietary formulas and requires complex VBA macros or DAX (Power Pivot) for advanced logic.
*   **Grist:** Natively supports full **Python** syntax and standard libraries for formulas, which is vastly superior for engineering workflows.

## Infrastructure & Control: The Open Source Advantage
*   **Excel:** Locked into the Microsoft 365 cloud or local `.xlsx` files that become corrupted when shared via SharePoint/OneDrive.
*   **Grist:** 100% open-source. You can self-host it via Docker/NixOS, giving you sovereign control over the data without paying per-user license fees.

## Security & Collaboration
*   **Excel:** File-level locking or clunky co-authoring. "Sharing" often means giving full access to the entire workbook.
*   **Grist:** Granular access controls. You can set permissions down to the specific row or column based on the user's login.

## Scale & Efficiency
Grist is specifically designed for building internal tools or managing interconnected lists (like server IPs, hardware MAC addresses, or car audio fitments). It provides the strict data integrity of a database while keeping the drag-and-drop ease of a spreadsheet. 

**Summary Recommendation:**
*   Use **Excel** strictly for financial modeling or when integrating heavily with other Microsoft products.
*   Use **Grist** for everything else, especially in DevOps and developer workflows where data integrity and infrastructure-as-code (self-hosting) are priorities.
