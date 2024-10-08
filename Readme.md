# Radar Chart Plotting Script

This script generates a radar chart from an Excel file and supports features such as dynamic scaling, customizable plot properties, interactive annotations, and selective emphasis of series in an exported image. The script also has support for both linear and logarithmic scaling on indiviual axes.


**Prerequisites**

Ensure you have the following libraries installed:

- pandas
- numpy
- matplotlib
- mplcursors

You can install these libraries using pip: pip install pandas numpy matplotlib mplcursors


**Excel File Format**

The Excel file DataToPlot.xlsx provides the expected structure of the spreadsheet, with the properties section in the first 12 rows and the data section starting from row 13


**Usage**

Ensure your Excel file DataToPlot.xlsx is properly formatted as described above.

Adjust "Save Image" and "Legend" flags to indicate preference. Specify if your axes are "linear" or "log".

Run the script: python radargraphmaker.py


The script will:

Read the data and properties from the Excel file.
Generate a radar chart based on the data.
Annotate data points as specified in the Excel file.
Provide an interactive chart with hover functionality.
Save the chart as an image if specified in the Excel file.


**Features**

Interactive Annotations: Hover over data points to see annotations.
Customizable Appearance: Define colors, line types, markers, presence of legend, and more in the Excel file.
Save Chart: Optionally save the generated chart as an image. Additionally, specify traces to be emphasized in the saved image.

**Logarithmic Axes**

Logarithmic scaling is applied to axes where the data spans several orders of magnitude. The logarithmic scale converts data into its logarithmic value (log10), and the tick marks on logarithmic axes are spaced according to powers of 10, rather than linearly. 


**Notes**

Ensure the Excel file path is correctly specified in the script (file_path variable).
Customize the chart appearance by adjusting the properties in the Excel file.


For further customization, refer to the matplotlib and mplcursors documentation.
