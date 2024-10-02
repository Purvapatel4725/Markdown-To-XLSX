# Markdown to Excel Converter

This repository contains a Python script (`md-Xlsx.py`) that converts a Markdown table into an Excel file. The script uses the `openpyxl` library to create the Excel workbook and handles parsing of the Markdown table format. This tool is useful when you want to quickly generate an Excel file from a well-formatted Markdown table.

## Features

- Parses Markdown tables and extracts headers and rows.
- Automatically generates an Excel file with the table content.
- Easy to use and modify for different Markdown table structures.

## How to Use

1. **Install Dependencies**:  
   The script requires `openpyxl` for creating and modifying Excel files. You can install the necessary package using:

   ```bash
   pip install openpyxl
   ```

2. **Run the Script**:  
   The script reads a Markdown table string and converts it to an Excel file. Make sure to replace the sample Markdown table with your own data. To execute the script, simply run:

   ```bash
   python md-Xlsx.py
   ```

3. **Sample Input**:  
   The script currently includes a sample table:

   ```markdown
   | Protocol | Network                      | Metric | Next Hop                   | Interface |
   |----------|------------------------------|--------|----------------------------|-----------|
   | S        | ::/0                         | 1/0    | 2001:DB8:CAFE:99::D1       | -         |
   | C        | 2001:DB8:CAFE:99::/64        | 0/0    | -                          | Vlan99    |
   | L        | 2001:DB8:CAFE:99::A1/128     | 0/0    | -                          | Vlan99    |
   | C        | 2001:DB8:CAFE:110::/64       | 0/0    | -                          | Vlan110   |
   | L        | 2001:DB8:CAFE:110::A1/128    | 0/0    | -                          | Vlan110   |
   | C        | 2001:DB8:CAFE:120::/64       | 0/0    | -                          | Vlan120   |
   | L        | 2001:DB8:CAFE:120::A1/128    | 0/0    | -                          | Vlan120   |
   | C        | 2001:DB8:CAFE:200::/64       | 0/0    | -                          | Vlan200   |
   | L        | 2001:DB8:CAFE:200::A1/128    | 0/0    | -                          | Vlan200   |
   | L        | FF00::/8                     | 0/0    | -                          | Null0     |
   ```

   The output will be saved as `output_table.xlsx`.

4. **Modifying the Script**:  
   You can change the input Markdown table in the `markdown_table` variable or pass your own Markdown input by modifying the script.

## Author

This project was created by **Purva Patel**.
