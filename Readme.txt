DXF Text Extractor Tool

Overview
-This project is a Python-based tool designed to streamline the extraction and aggregation of text data from DXF files, commonly used in CAD software. The tool leverages tkinter for a simple GUI, ezdxf for reading DXF file content, and pandas for data handling. Processed data is exported to an Excel file for easy analysis and reporting.

Features
-User-friendly Interface: Built with tkinter to make file selection intuitive.
-Text Parsing and Aggregation: Extracts text that includes = symbols and sums values associated with duplicate keys.
-Data Cleanup: Automatically removes trailing feet (') characters from values before processing.
-Excel Export: Outputs processed data to an Excel file for further use.
-Standalone Executable: Packaged with PyInstaller to create a .exe for easy distribution without Python dependencies.

How It Works
-Select a DXF File: Use the GUI to choose a DXF file.
-Data Processing: The tool reads and processes the file, identifying and summing up values after = symbols, and handles duplicate entries efficiently.
-Result Display: The tool displays a success message indicating where the Excel file has been saved.
-Error Handling: Gracefully manages non-numeric data and invalid inputs.

Usage
-Run the script with Python or use the standalone executable created with PyInstaller.
-Ideal for engineers, CAD specialists, or data analysts needing quick text extraction and processing from DXF files.

Technologies Used
-Python: Core language.
-tkinter: GUI framework.
-ezdxf: DXF file parsing.
-pandas: Data processing and Excel export.
-PyInstaller: Converts the script into an executable.

How to Run
Clone the repository and execute the script or download the executable from the dist folder. To package your own executable, run:

pyinstaller --onefile --windowed dxf_extractor.py

Future Enhancements
-Add support for more complex DXF entities.
-Integrate with cloud services for direct data upload.
-Improve the UI for better user experience.