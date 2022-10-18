[<<< Previous](https://github.com/jacobmswisher/ArcGIS-Online/blob/main/Sections/Part%205%20-%20Inquiry%20with%20Spatial%20Data.md) | [Next >>>](https://github.com/jacobmswisher/ArcGIS-Online/blob/main/Sections/Part%207%20-%20Resources.md)  

## Part 6: Data Visualization in ArcGIS Online

Alongside filters, ArcGIS Online users also utilize the styles tool to create data visualizations with the Map Viewer.

Most often, creating a data visualization in ArcGIS Online involves manipulating the basemap and feature layer symbology in the Map Viewer. In ArcGIS Online, you can manage the symbology of your feature layers using the styles tool.

*Tip: The styles tool can also be deployed in the inquiry process. Sometimes, looking at variations in symbology can be just useful as making selections, especially early on in a research project when you often generate new research questions in the course of implementing a workflow.*

### Step 1: Adjust Feature Layer Symbology

For this part of the workshop, we'll continue working with Administrative Forest Boundaries. Make sure that Administrative Forest Boundaries is still added to your Map Viewer. Then, click the styles tool button on the right-hand toolbar.

<p align="center">
  <img src="https://github.com/jacobmswisher/images/blob/main/ArcGIS%20Online/Figure%2044.JPG">
</p>

The styles tool allows you to adjust the symbology of your feature layer. Like the filters tool, the styles tool uses fields from a feature layer's attribute table to create different data visualizations. As you change the field using the add field button, you'll notice that the style options available to you will change based on the [data type](#p-aligncentertable-2-field-data-types-in-arcgis-onlinep) of the chosen field. For a comprehensive list of style options and their associated field data types, consult this [ESRI resource](https://doc.arcgis.com/en/arcgis-online/create-maps/apply-styles-mv.htm).

To begin changing the symbology for Administrative Forest Boundaries, click the add field button and add the REGION field.

*Tip: After selecting a field, you can use the add expression button to build an SQL expression that will instruct ArcGIS Online to adjust the symbology for features that meet the criteria of the expression.*

<p align="center">
  <img src="https://github.com/jacobmswisher/images/blob/main/ArcGIS%20Online/Figure%2045.JPG">
</p>

After adding the REGION field (field data type: text), you'll notice you have a new style option in the styles tool pane. Select the unique symbols option and then take a look at your Map Viewer.

Unique symbols changes the color of features to match the data in the selected field (REGION), with each different (unique) entry that appears in the attribute table recieving a unique assigned color.

To adjust to colors assigned using the REGION field and the unique symbols style, click the style options button.

<p align="center">
  <img src="https://github.com/jacobmswisher/images/blob/main/ArcGIS%20Online/Figure%2046.JPG">
</p>

The style options feature of the styles tool provides you with various options to customize your data visualization. Clicking on the edit (pencil) button will allow you to adjust colors, transparency, and feature outlines. Additionally, you can click and drag the various unique symbols to reorder the list of unique features. Reordering the unique symbols list will also reorder the features in the map legend on the bottom-left-hand corner of the Map Viewer if you don't like the default order (unique symbols sorts by the quantity of each unique entry in the attribute table).

<p align="center">
  <img src="https://github.com/jacobmswisher/images/blob/main/ArcGIS%20Online/Figure%2047.JPG">
</p>

Using the edit tool, adjust the data visualization for Administrative Forest Boundaries to your liking. Then, click the done button at the bottom of the styles tool pane to add the new style options to the feature layer.

*Tip: You can adjust whether a legend appears for the selected feature class on your map by clicking the legend button on the left-hand toolbar.*

### Step 2: Adjust the Basemap

In addition to using the styles tool to manage feature layer symbology, it is also important to select and appropriate **basemap** for your data visualization. 

**Basemap** - an imagery layer that usually serves as the backdrop for a map.

To adjust the basemap in the Map Viewer, click the basemap button on the left-hand toolbar.

<p align="center">
  <img src="https://github.com/jacobmswisher/images/blob/main/ArcGIS%20Online/Figure%2048.JPG">
</p>

Then, scroll through the basemap options and select a basemap that you think pairs well with Adminstrative Forest Boundaries.

### Step 3: Export Your Data Visualization

After adjusting the symbology for Administrative Forest Boundaries and choosing a basemap, it's time to export your data visualization. 

To export a data visualization, click on the print button on the left-hand toolbar in the Map Viewer.

<p align="center">
  <img src="https://github.com/jacobmswisher/images/blob/main/ArcGIS%20Online/Figure%2049.JPG">
</p>

The print tool allows you to export your map in a file format of your choice. Exporting as a layout is the preferable method, as the layout options allow you to include a legend, scale, north arrow, author information, and title with your map. Exporting with the map only option will simply export an image of the map viewer.

Click the export button to export a pdf of your map with the default options and then click the link to open the exported file to examine the map layout.

<p align="center">
  <img src="https://github.com/jacobmswisher/images/blob/main/ArcGIS%20Online/Figure%2050.JPG">
</p>

*Tip: Take full advantage of the capabilities of ArcGIS Online by [embedding](https://doc.arcgis.com/en/arcgis-online/share-maps/embed-maps-groups.htm) an interactive version of your data visualization on the web.*

### Exercise 6: Explore the Styles Tool

**Task: On your own, create at least two different data visualizations using Administrative Forest Boundaries or a layer of your choice. Choose a different field for each data visualization. Then, export at least one of your data visualizations using the print tool.**

[<<< Previous](https://github.com/jacobmswisher/ArcGIS-Online/blob/main/Sections/Part%205%20-%20Inquiry%20with%20Spatial%20Data.md) | [Next >>>](https://github.com/jacobmswisher/ArcGIS-Online/blob/main/Sections/Part%207%20-%20Resources.md)  