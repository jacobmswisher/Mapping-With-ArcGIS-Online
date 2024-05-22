# Part 4: Creating and Editing Feature Layers

In some cases, you may need to create spatial data for research project. In ArcGIS Online, you can create new feature layers with point, line, or polygon geometry via the Content Tab and edit those feature layers in the Map Viewer.

## Step 1: Create an Editable Feature Layer in ArcGIS Online

To create a new, editable feature layer, navigate to the Content Tab, click the new item button, and select the option to create a new feature layer.

<div align="center">

<img src="https://github.com/jacobmswisher/images/blob/main/ArcGIS%20Online/Figure%2025.JPG" alt="">

</div>

Select the option to define your own layer, then click the next button.

For this demonstration, we are going to create an editable feature layer that visualizes places you visited in the last week using point geometry.

In the create a feature layer window, assign your new layer a name (ex. places\_I\_visited) and make sure the geometry is set to point layer. Then, click the next button.

<div align="center">

<img src="https://github.com/jacobmswisher/images/blob/main/ArcGIS%20Online/Figure%2026.JPG" alt="">

</div>

Though we won't use these options in this exercise, when creating a new feature layer ArcGIS Online does allow you to build more complex datasets by:

1. **Adding multiple layers to a feature layer.** Using this function creates what ArcGIS Online refers to as a **group layer**, or a feature layer that contains multiple feature classes. Using this tool can be useful when, for example, you want to import a single feature layer that represents a collection of features with different geometries (ex. some features as points and others as polygons).
2. **Adding GPS metadata fields.** Enabling this option automatically generates fields for recording information about GPS recievers used to create new features in the feature layer. ArcGIS Online facilitates data creation with GPS recievers through a separate application called [ArcGIS Field Maps](https://www.esri.com/en-us/arcgis/products/arcgis-field-maps/overview).
3. **Enabling Z-values.** This option allows you to store Z coordinates for features, in addition to the standard creation of X,Y coordinates for each feature. Enable this option if you want to create 3D models or track the elevation of features in ArcGIS Online.

Finally, update the metadata and tags as needed for places\_I\_visited. Then, save the new feature layer.

## Step 2: Add Fields

After creating the places\_I\_visited feature layer, we need to finish setting up the layer before creating new features. This involves two steps:

1. Adding fields (attributes)
2. Making the feature layer "editable"

Let's begin by adding a couple of fields (attributes) to the places\_I\_visited feature layer to help document the name of each place and the date that you visited.

To add fields, start by clicking navigating to the data tab from the content page for the places\_I\_visited feature layer.

<div align="center">

<img src="https://github.com/jacobmswisher/images/blob/main/ArcGIS%20Online/Figure%2027.JPG" alt="">

</div>

In the upper-right hand corner, use the fields button to switch from the table view to the field list view. Then, click the add button on the left to create your first field.

<div align="center">

<img src="https://github.com/jacobmswisher/images/blob/main/ArcGIS%20Online/Figure%2028.JPG" alt="">

</div>

Next, complete the add field form to create a field that will capture the names of the features in the places\_I\_visited feature class. Use the table below as a guide and, after you have completed the form, check your add field form against the image below the table.

_Tip: It's generally a good idea to enable the allow null Values option. Null values indicate that the attribute field for a record has no value. This is different than a field that is empty, which in the case of text (or string) fields, would mean that the field has a value of "", which essentially means "nothing". This will become important later on when we begin working with filters, as some filters will return empty values but will not return null values. More on this in \[Part 5: Inquiry with Spatial Data]\(Sections/Part 5 - Inquiry with Spatial Data.md)._

### Table 2. Field data types in ArcGIS Online.

| Field Data Type | Storeable Range                   | Use                                                                        |
| --------------- | --------------------------------- | -------------------------------------------------------------------------- |
| String          | 255 characters (default)          | Stores information as text                                                 |
| Short Integer   | -32,768 to 32,767                 | Stores whole numbers                                                       |
| Long Integer    | -2,147,483,648 to 2,147,483,647   | Stores whole numbers                                                       |
| Float           | approximately -3.4E38 to 1.2E38   | Stores numbers with decimal places                                         |
| Double          | approximately -2.2E308 to 1.8E308 | Stores numbers with decimal places                                         |
| Date            | mm/dd/yyyy hh:mm:ss AM/PM         | <p>Stores date and time information.<br>Can be sorted chronologically.</p> |

\


<div align="center">

<img src="https://github.com/jacobmswisher/images/blob/main/ArcGIS%20Online/Figure%2029.JPG" alt="">

</div>

After adding a field for the name of features in places\_I\_visited, add a second field that will contain information for the date you visited each place.

**Note: Clicking on a field name in the data tab will allow you to make changes to the field or, if needed, delete the field from the attribute table.**

## Step 3: Make the Feature Layer Editable

After creating fields for your new feature layer, you need to make sure that the feature layer "editable" before you can create new features. Editing settings are managed in the settings tab for your feature layer.

<div align="center">

<img src="https://github.com/jacobmswisher/images/blob/main/ArcGIS%20Online/Figure%2030.JPG" alt="">

</div>

Navigate to the settings tab for places\_I\_visited. Then, scroll down the page until you find the editing settings.

<div align="center">

<img src="https://github.com/jacobmswisher/images/blob/main/ArcGIS%20Online/Figure%2031.JPG" alt="">

</div>

Confirm that the enable editing box is checked and that places\_I\_visited allows all kinds of editing (Add, Delete, Update) for both attributes and geometry. If you needed to change any settings, you also need to save your changes at the bottom of the page. Save if needed and then navigate back to the overview tab for places\_I\_visited.

_Tip: The editing settings also allow you to manage how collaborators can interact with your feature layer. These settings can be helpful for managing group work on GIS projects._

## Step 4: Update Metadata

If needed, update the metadata (description, terms of use, etc.) and sharing permissions for places\_I\_visited.

## Step 5: Create New Features

Now that you have completed the process of creating an editable feature layer, its time to head back to the Map Viewer and create new features for places\_I\_visited!

Begin by navigating to the Map Viewer and adding places\_I\_visited to the map (you can do this quickly by clicking the open in Map Viewer button at the top-right of the overview tab).

Once you are in the Map Viewer, open the editor tool by clicking the edit button on the right-hand toolbar.

<div align="center">

<img src="https://github.com/jacobmswisher/images/blob/main/ArcGIS%20Online/Figure%2032.JPG" alt="">

</div>

The editor tool allows you to create, edit, and delete features in a feature layer. You can create features by clicking the new feature button and can edit or delete features via the select button (editing after we create our first feature). The filter types function comes into play when editing group layers.

_Tip: Snapping is a setting that, when enabled, automatically connects (snaps) a new edge or vertex of a feature to an existing edge or vertex of another feature when the new edge/vertex is created next to the old one. This feature is particularly useful when creating new polygons, as it ensures that you eliminate empty space (known as a sliver) between polygon features that are supposed to share edges._

Click the new feature button to start creating your first feature.

<div align="center">

<img src="https://github.com/jacobmswisher/images/blob/main/ArcGIS%20Online/Figure%2033.JPG" alt="">

</div>

After you click the new feature button, your cursor will transform into a data creation tool allowing you to create a new point feature by clicking anywhere on the map. We are going to start by creating a point for the Hesburgh Library at the University of Notre Dame in South Bend, Indiana.

Zoom in on the map, find the Hesburgh Library, and click on the center of the library to create a new point feature. After clicking on the map, a pane will appear on the right side of the browser where you can populate the fields for the new feature. Populate the fields with the name of the feature and today's date and time (_Hint: Hitting tab after entering the date will automatically populate the time with your local time_). Then, click the create button to finish creating the feature.

<div align="center">

<img src="https://github.com/jacobmswisher/images/blob/main/ArcGIS%20Online/Figure%2034.JPG" alt="">

</div>

**Note: After creating a new feature, ArcGIS Online will allow you to keep creating additional features in the Map Viewer until you exit the create feature tool.**

Congratulations! You have succesfully created a new feature in ArcGIS Online. If you want, you can open the attribute table for places\_I\_visited to look at the attribute information for the feature.

## Exercise 4: Creating More Features

**Task: On your own, create at least 5 more features for places you have visited in the last week.**

## Step 6: Edit Features in the Feature Layer

The editor tool also allows you to edit and delete existing features in a dataset. We'll learn about both functions by editing, then deleting the Hesburgh Library point from the places\_I\_visited.

To edit and delete features, click the select button in the Editor tool.

<div align="center">

<img src="https://github.com/jacobmswisher/images/blob/main/ArcGIS%20Online/Figure%2035.JPG" alt="">

</div>

Then, click on the point for the Hesburgh Library to manage the feature. Let's practice editing the feature by adjusting the date visited field. Change the date field to reflect that you visited the Hesburgh Library early in the morning at 6:00 AM. Then, click the update button to save your changes.

<div align="center">

<img src="https://github.com/jacobmswisher/images/blob/main/ArcGIS%20Online/Figure%2036.JPG" alt="">

</div>

## Step 7: Delete Features in the Feature Layer

To delete a feature from a feature layer, repeat the process from [Step 6: Edit Features in the Feature Layer](<Part 4 Creating and Editing Feature Layers.md#step-6-edit-features-in-the-feature-layer>). However, instead of updating the feature in the edit feature tool, simply click the delete button at the bottom of the pane to delete the selected feature. After deleting the feature, you will be asked to confirm that you want to delete the feature as a deletion is irreversible in ArcGIS Online.

Go ahead and delete the point for the Hesburgh Library now.

<div align="center">

<img src="https://github.com/jacobmswisher/images/blob/main/ArcGIS%20Online/Figure%2037.JPG" alt="">

</div>

**Note: ArcGIS Online automatically saves creations, edits, and deletions for feature layers.**

## Exercise 5: Creating Feature Layers in ArcGIS Online

**Task: On your own, create a feature layer with point, line, and/or polygon geometry in ArcGIS Online using the Content Tab. Choose whatever theme you want for your layer or, alternatively, create a layer with random features. Include at least five features and at least two attribute fields in your dataset.**
