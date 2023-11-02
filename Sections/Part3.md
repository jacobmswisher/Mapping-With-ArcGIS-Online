[<<< Previous](Part2.md) | [Next >>>](Part4.md)  

## Part 3: Gathering Spatial Data

Now that you have taken some time to explore the [Map Viewer](https://notredame.maps.arcgis.com/apps/mapviewer/index.html) and ArcGIS Online's file storage system, it's time to start working with some data! In this section of the workshop, you will learn how to get data into the Map Viewer through two methods:
1. [Searching for available data through ArcGIS Online](#method-1-searcing-for-data-with-arcgis-online)
2. [Importing data into ArcGIS Online via files stored on your computer](#method-2-importing-data-to-arcgis-online-with-the-content-tab)

### Method 1: Searcing for Data with ArcGIS Online

As the saying goes, work smarter, not harder. This philosophy applies in the world of GIS where, luckily for you, thousands of universities, government agencies, and individual people have already created many different datasets and made them available to the public. Additionally, through your organizational account, you also have access to ESRI's [Living Atlas](https://livingatlas.arcgis.com/en/home/) which contains various large datasets curated by ESRI. 

When working with GIS data, its always a good idea to determine if somebody else has already created the thing you need for your project and to save yourself considerable amounts of time by not having to create datasets on your own. One of the strengths of ArcGIS Online's Map Viewer is the ability to search for layers in the Living Atlas as well as those published by other ArcGIS Online users.

### Step 1: Navigate to the Add Layer Function and Set Your Search Parameters

To start searching for spatial data with the Map Viewer, navigate to the add layer function by clicking on the layers button on the left-hand taskbar. Then, click the add layer button.

<p align="center">
  <img src="https://github.com/jacobmswisher/images/blob/main/ArcGIS%20Online/Figure%209.JPG">
</p>

After clicking the add layer button, you will have the option to search for layers on the left-hand side of your browser. At the top of the add layer tool, ArcGIS Online allows you to change your search parameters to one of the following options in order to help you find the data you need for your project:

#### <p align="center">Table 1. Data Search Parameters in ArcGIS Online.</p>
<table align="center">
  <tr>
    <th>Category</th>
    <th>Effect</th>
  </tr>
  <tr>
    <td align="center">My Content</td>
    <td>Limits your search to only include content items you own</td>
  </tr>
  <tr>
    <td align="center">My Favorites</td>
    <td>Limits your search to only inlude content items you star as a favorite. You can manage this in the content tab or by clickking on a layer in the Map Viewer.</td>
  </tr>
  <tr>  
    <td align="center">My Groups</td>
    <td>Limits your search to only include content items assigned to a defined group of users. You can manage groups in the groups tab of ArcGIS Online and manage sharing permissions in the content tab.</td>
  </tr>
  <tr>  
    <td align="center">My Organization</td>
    <td>Limits your search to only include content items published at the organization level. This is a publication setting configured in the content tab that shares a dataset with all users who you have accounts with your organization (ex. University of Notre Dame users).</td>
  </tr>
  <tr>
    <td align="center">Subscription Content</td>
    <td>Allows you to search content for which your organization has a paid subscription.</td>
  </tr>
  <tr>
    <td align="center">Living Atlas</td>
    <td>Limits your search to only include content items that are part of ESRI's Living Atlas</td>
  </tr>
  <tr>  
    <td align="center">ArcGIS Online</td>
    <td>Allows you to search for all datasets made available to everyone on ArcGIS Online. You can set your content to the everyone sharing permission in the content tab.</td>
  </tr>
</table>

**Note: If you haven't worked in ArcGIS Online before, the My Content search parameter will not show any content. This will change once you create your own content later in the workshop.**

For your first search with ArcGIS Online, adjust your parameters to search the Living Atlas using the dropdown menu at the top of the add layer tool.

<p align="center">
  <img src="https://github.com/jacobmswisher/images/blob/main/ArcGIS%20Online/Figure%2010.JPG">
</p>

Next, search for World Countries, a feature layer hosted by ESRI.

<p align="center">
  <img src="https://github.com/jacobmswisher/images/blob/main/ArcGIS%20Online/Figure%2011.JPG">
</p>

### Step 2: Evaluate Your Search Results

Before you add a layer created by a third party to your Map Viewer, it's important to take a moment to evaluate the dataset for its quality. In ArcGIS Online, the best way to do this is to take a look at the **metadata** for a layer.

**Metadata** - Data about data. The set of data attached to a layer or other piece of content that provides information about that dataset.

To look at the metadata for World Countries, click on the hyperlinked title of the feature layer.

<p align="center">
  <img src="https://github.com/jacobmswisher/images/blob/main/ArcGIS%20Online/Figure%2012.JPG">
</p>

As you read through the metadata for World Countries, what do you notice about it? Does this stirke you as a thoroughly-documented dataset? Is there anything you think is missing from the description?

Just as you would evaluate other sources of information, checking the metadata associated with layers available online is a good first step to make sure that the data you have found is (1) appropriate for your project and (2) from a reliable source.

### Step 3: Add Data to the Map Viewer

Now that you have examined the metadata for World Countries, it's time to add the layer to your Map Viewer. You can add World Countries to the Map Viewer in two ways: using the add button in the seach results or clicking the add to map button that appears at the bottom of the screen when viewing the World Countries metadata.

Go ahead and add World Countries to your Map Viewer.

<p align="center">
  <img src="https://github.com/jacobmswisher/images/blob/main/ArcGIS%20Online/Figure%2013.jpg">
</p>

Congratulations! You have succesfully added your first layer to the Map Viewer! Your Map Viewer should look like this:

<p align="center">
  <img src="https://github.com/jacobmswisher/images/blob/main/ArcGIS%20Online/Figure%2014.JPG">
</p>

### Step 4: Take a Second Look at the Data

Once you have added World Countries to the Map Viewer, its time to take a closer look at the features in the dataset. In addition to reviewing the metadata for a layer, examining the **attribute table** is another way to assess the datasets you find via ArcGIS Online or elsewhere on the internet.

**Attribute table** - A tabular representation of information associated with a feature class. An attribute table is composed of **records** and **fields**.

Each **record** (or row) in the attribute table corresponds to a feature in the feature class.

Each **field** (or column) in the attribute table corresponds to an attribute (a category of information) that is assocociated with each feature in the feature class.

To open the attribute table for World Countries, navigate to the layers tab on the left-hand side of the Map Viewer and click the three-dot options button on the right-hand side of the World Countries layer. Then, click the show table button.

<p align="center">
  <img src="https://github.com/jacobmswisher/images/blob/main/ArcGIS%20Online/Figure%2015.JPG">
</p>

Take a look at the attribute table for World Countries. Can you answer the following questions?
1. How many features are in the feature class World Countries? *Hint: What is a record?*
2. How many attributes are associated with each feature in World Countries?

<p align="center">
  <img src="https://github.com/jacobmswisher/images/blob/main/ArcGIS%20Online/Figure%2016.JPG">
</p>

Examining a feature class's attribute table is not only a way to figure out what kind of information is associated with the features in the feature class but can also be a method for assessing the reliability of a dataset. Always look in the attribute table to determine whether the data appears **clean**.

**Clean data** - data that has been checked for accuracy (ex. fixing spelling errors).

### Step 5 (Optional): Stylize World Countries

At this point, you may be wondering how to change the **symbology** of layers in ArcGIS Online.

**Symbology** - The visual characteristics of mapped features, including color, icon, outline, etc.

You can adjust using the styles tool on the right-hand toolbar. We will cover symbology in greater detail in [Part 6](#part-6-data-visualization-in-arcgis-online) of this workshop.

<br>
<p align="center">
  :rotating_light: :rotating_light: :rotating_light: <b>CAUTION! SAVE YOUR MAP!</b> :rotating_light: :rotating_light: :rotating_light:
</p>
<br>

Before we move on to importing data into ArcGIS Online with the content tab, take a moment to stop and save your map using the save and open button on the left-hand toolbar.

<p align="center">
  <img src="https://github.com/jacobmswisher/images/blob/main/ArcGIS%20Online/Figure%2017.JPG">
</p>

Saving a map creates a copy of the map in your content tab that you can reopen, update, and save for future use.

**It is incredibly important that you save your work frequently. ArcGIS Online currently does have an autosave feature. If you close the the Map Viewer tab in your browser and forget to save, you will lose your work.**

### Exercise 1: Practice Searching for Layers with ArcGIS Online

Now that you have gone through the process of finding the World Countries layer, adding it to the Map Viewer, and saving your map, take some time to explore the incredible trove of data available on ArcGIS Online. 

**Task: Using the Living Atlas or ArcGIS Online search paramaters, find and add three datasets that interest you to the Map Viewer.**

### Method 2: Importing Data to ArcGIS Online with the Content Tab

Though there are thousands of datasets published on ArcGIS Online, you can't always find what you are looking for using the platform's search function. Sometimes, users need to bring spatial data they have acquired elsewhere into ArcGIS Online for analysis by importing data through the content tab.

### Step 1: Find the Data You Want to Import

GIS data is often readliy accessible on the internet, especially in the case of data that comes from government sources. Today, we'll practice importing spatial data into ArcGIS Online by finding a feature class for the administrative units of the United States Forest Service (USFS).

Start by navigating to the [USFS data clearinghouse](https://data.fs.usda.gov/geodata/).

Data clearinghouses are common platforms through which federal agencies host geospatial data available for public use and are an excellent source of different kinds of data for GIS projects, such as road and street data, census data, or elevation rasters.

You'll find the Administrative Forest Boundaries feature class under the [Enterprise Data](https://data.fs.usda.gov/geodata/edw/index.php) section of the USFS data clearinghouse. Click on [Enterprise Data](https://data.fs.usda.gov/geodata/edw/index.php) and then navigate to the [National Datasets](https://data.fs.usda.gov/geodata/edw/datasets.php) subsection of the Enterprise Data Warehouse.

Type "administrative forest boundaries" into the search by keyword box. Then, click the [shape file](https://data.fs.usda.gov/geodata/edw/edw_resources/shp/S_USA.AdministrativeForest.zip) hyperlink to download a copy of the feature class.

<p align="center">
  <img src="https://github.com/jacobmswisher/images/blob/main/ArcGIS%20Online/Figure%2018.JPG">
</p>

**Note: If you are struggling to find the Administrative Forest Boundaries feature class through the USFS website, you can download a copy [here](https://github.com/jacobmswisher/ArcGIS-Online/raw/main/Administrative%20Forest%20Boundaries.zip).**

### Step 2: Upload Your Data

Clicking on the shape file hyperlink will download a zipped (compressed) version of the feature class stored as a shape file, a common file format for storing vector data. To import the feature class into ArcGIS Online, we simply need to upload the zipped shapefile via the Content Tab.

**Note: ArcGIS Online can also interpret feature classes stored as a file geodatabase, the other download option from the USFS clearinghouse.**

To upload Administrative Forest Boundaries to ArcGIS Online, navigate to the content tab and click on the new item button on the upper-left-hand side of the browser.

<p align="center">
  <img src="https://github.com/jacobmswisher/images/blob/main/ArcGIS%20Online/Figure%2019.JPG">
</p>

Then, either drag and drop the zipped Administrative Forest Boundaries folder into the new item window or click the your device button to open the folder from your downloads.

When you add the zipped Administrative Forest Boundaries folder to the new item window, ArcGIS Online will provide you with a few options to manage how the file is added to your Content Tab:

<p align="center">
  <img src="https://github.com/jacobmswisher/images/blob/main/ArcGIS%20Online/Figure%2021.JPG">
</p>

Make sure ArcGIS Online has identified the item type for the zipped Administrative Forest Boundaries folder as a shape file, then choose the option to add Administrative Forest Boundaries.zip and create a hosted feature layer and click next.

**Note: If you encounter an error stating that your layer already exists, it may exist either in your content folder or in the content folder of another member of the Notre Dame ArcGIS Online organization. If this occurs, rename the zipped folder to include a unique identifier, such as the date or your initials.**

Before ArcGIS Online saves the feature class to your Content Tab, the platform will provide you with an opportunity to change the name of the feature class, assign the feature class to a file folder, add tags (which can help you effeciently search through your content), and add initial metadata to the file.

<p align="center">
  <img src="https://github.com/jacobmswisher/images/blob/main/ArcGIS%20Online/Figure%2022.JPG">
</p>

Edit the information in these categories as you see fit. Then, click the save button.

After saving your upload, ArcGIS Online will immediately take you to the page for that content item. Here, you can edit the metadata, sharing permissions, and other elements of the Administrative Forest Boundaries feature layer.

### Step 3: Add Your Imported Data to the Map Viewer

Now that you have uploaded the Administrative Forest Boundaries shape file into ArcGIS Online as a feature layer, its time to take a look at your dataset!

Head over to the Map Viewer and add Administrative Forest Boundaries to your map. You will find your layer under the My Content section of the add layer tool.

<p align="center">
  <img src="https://github.com/jacobmswisher/images/blob/main/ArcGIS%20Online/Figure%2024.JPG">
</p>

Congratulations! You have successfully uploaded spatial data to ArcGIS Online!

### Exercise 2: Uploading Data

On your own, take some time to browse the internet and find some GIS data that interests you. A good way to begin is by hopping on your favorite search engine, and searching for a GIS data related to your topic of interest (ex. education GIS data).

**Task: Find two datasets online and upload them to ArcGIS Online.**

[<<< Previous](Part2.md) | [Next >>>](Part4.md)  
