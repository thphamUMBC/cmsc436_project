# **CMSC 436/636: Data Visualization**
## **Final Project**

### Memebers
**Thanh Pham, Rachit Shaha, Johnson Xie, and Rishabh Saxena**
### Project desscription
**This is The Affordability Identifier project that helps users to locate afforadable area according to their salary. There are three visualizations (Stacked bar chart, Heatmap, and Choropleth map) that allow users to interactively choose the states, counties, and occupations to aggregate the affordability percentage.**
### Contact:
**Email: [thanhp1@umbc.edu](mailto:thanhp1@umbc.edu)**

**GitHub: [thphamUMBC](https://github.com/thphamUMBC/cmsc436_project)**

----------

# User manual

## Depencies
* matplotlib
* pandas
* numpy
* mplcursors
* ipywidgets
* urllib
* plotly

__Note__: Those indepencies are downloaded and used for data processing and visualizing, but those independencies may need more supporting libraries. When you Jupyter Notebook, if you don't have a specific supporting library, just download it by `pip install library`.
## How to load the data set
* In order to load the datasets, just run the **Import Library** and **Import Datasets** sections.
## How to interact with the system
* There are threes visulizations in this product: _Stacked bar charts_, _Heatmap_, and _Choropleth map_. Among them, he Stacked bar chart and the Heatmap will have a very similar interactive user interface. Therefore, this will introduce them in two group:
1. Stacked bar charts and Heatmap: There are four common components between them. The first one is the combobox for choosing state. When the users choose a state, it will generate two multiple selection boxes for counties and occupation in that state, which are the second and third components. The visualizations are only generated and rendered only a state, at least one county, and at least one occupation are selected. Also, they have the text input for personal income as the fourth component. This only accepts a number as a input and will ignore the input if it is not a numeric format, such as 70000. When you enter a correct format for the personal income, the visulizations will be rerendered. The last component is the sorted by total feature which is only available for the Stacked bar chart. This also rerender the visualization everytime the users change it clicking it.
2. For the Choropleth map, there are only users' interaction with the map and no users' input. However, the users can hover over every county to check for the extra information in the tooltip. Also, the users can drag and zoom the map for better vision.

## How to restart
* There are two ways for users to restart the application. One of them is restart the whole Jupyter Notebook by clicking these two button in order: _Restart_ and _Run All_. The other and recommended one is to reset only the error visualization by recompiling the cell that renders that visualization.