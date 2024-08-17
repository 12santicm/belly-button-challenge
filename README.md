# belly-button-challenge

OVERVIEW:

The main goal of this project is to develop an interactive dashboard that allows users to explore information on the microbes that colonize human navels, based on data from various test subjects.

FILES:

In this repository, you'll find an HTML file containing the code for the webpage, a JSON file with the project data, and a JavaScript file for the data analysis.

DATA ANALYSIS:

To create the interactive dashboard, I filtered the data, created functions, and used the D3 library. My first step was to create a function to retrieve the data using d3.json() and then filter it to obtain relevant information for the project. I then worked with the HTML to specify where the first graphic would be displayed.

DATA VISUALIZATION:

Bubble Chart:

The Bubble Chart visualizes the operational taxonomic units (OTUs) found in each sample. It uses OTU IDs for the x-axis, sample values for the y-axis, and OTU labels as hover text. The marker size is based on the sample values, and the color is determined by the OTU IDs.

Bar Chart:

The Bar Chart displays the top 10 OTUs found in the selected sample. The x-axis represents the sample values, and the y-axis represents the OTU IDs, which are sliced to include only the top 10 and reversed for display.

Dropdown Menu and Event Listener:

I populated the dropdown menu with sample names using D3, allowing users to select a specific sample to explore. When a new sample is selected from the dropdown, the optionChanged() function is triggered. This function calls buildCharts() and buildMetadata() to update the visualizations and metadata with the new sample.
