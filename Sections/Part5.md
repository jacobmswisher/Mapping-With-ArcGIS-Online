[<<< Previous](Part4.md) | [Next >>>](Part6.md)  

## Part 5: Inquiry with Spatial Data

Now that you've learned how to bring data into ArcGIS Online in multiple ways, its time to start leveraging the tools available in ArcGIS Online to learn how to integrate GIS **workflows** into your research process.

**Workflow** - A planned, series of operations that integrates data and computational processes to complete a task. In research applications, the task a workflow addresses most often is answering a question.

For this workshop, we are going to implement a workflow that uses Administrative Forest Boundaries and the filters tool to figure out how many national forests contain at least 2 million acres of land.

### Step 1: Pose a Research Question

Building a GIS workflow begins with posing a question.

**Workshop Research Question: How many national forests in the United States contain at least 2 million acres of land?**

Taking the time to clearly define a research question before developing and implemeneting a GIS workflow is an important step, especially for larger projects where workflows can require a large number of datasets and operations.

### Step 2: Determine What Data You Need and Add It to the Map Viewer

After posing a question, the next step in the inquiry process is to determine what data is needed to answer your question. In our case, we need a dataset that contains information about all of the national forest units in the United States. Fortunately, we have the perfect dataset: the Adminstrative Forest Boundaries feature layer! Go ahead and add Administrative Forest Boundaries to the Map Viewer.

### Step 3: Apply a Filter to Administrative Forest Boundaries

Part of developing a workflow involves determining which computational processes will help you to answer your research question. In GIS, one common method of answering questions that rely on fields in an attribute table is to make a **selection**.

**Selection** - In GIS, the process of selecting features in a feature class that meet certain criteria based on the feature's attributes or location.

To answer our question, we are going to select features based on their attributes using the filter tool in ArcGIS Online. In order to select by attribute in ArcGIS Online, the filter tool uses **structured query language (sql) expressions**.

**SQL Expression** - A combination of fields and conditions that, when applied to a feature layer, return all records (features) that meet the criteria of the expression.

SQL expressesions select features from a feature layer where the information in the selected field meets the specified conditions.

In computational terms, an SQL expression does three things:
1. SELECT features 
2. FROM feature layer 
3. WHERE [Field][Condition]

In an SQL expression, the [Condition] consists of a Boolean Operator (ex. is, and, or, less than, greater than) and a value.

Using the filter tool, you will set the parameters for the [Field] and [Condition] portions of the SQL expression.

To apply a filter, begin by clicking on the Administrative Forest Boundaries feature layer. Then, open the filter tool using the right-hand toolbar.

<p align="center">
  <img src="https://github.com/jacobmswisher/images/blob/main/ArcGIS%20Online/Figure%2038.JPG">
</p>

Next, click the add expression button in the filter tool pane.

<p align="center">
  <img src="https://github.com/jacobmswisher/images/blob/main/ArcGIS%20Online/Figure%2039.JPG">
</p>

Then, define the parameters for your filter using the filter tool pane.

**Note: You will notice that different fields allow you to select different operators. This is because certain operators can only be used with certain field data types (ex. you cannot use the "is less than" with a string (text) field.)**

<p align="center">
  <img src="https://github.com/jacobmswisher/images/blob/main/ArcGIS%20Online/Figure%2040.JPG">
</p>

To determine how many national forests contain at least 2 million acres of land, we need to use the filters tool to build a SQL expression that uses the GIS_ACRES field. Try to create the expression on your own, then check your work using the image below.

<p align="center">
  <img src="https://github.com/jacobmswisher/images/blob/main/ArcGIS%20Online/Figure%2041.JPG">
</p>

Then, save the expression to apply the filter to Administrative Forest Boundaries.

**Note: If you need to apply a filter to select features that meet multiple criteria, click the add expression button again to build a filter with multiple SQL expressions.**

### Step 4: Open the Attribute Table

After saving the expression, you will notice a visual change in the Map Viewer. When you save a filter, the Map Viewer will hide all of the features that don't meet the parameters of the filter's SQL expression. However, this is unhelpful when you need to know the exact number of features that meet the parameters of your SQL expression. To view a list of the features selected by the filter tool, simply open the attribute table.

*Tip: Filters can be useful for more than just inquiry. By using filters creatively, you can create a series of differnt data visualizations using the same feature class.*

As you'll notice, the attribute table has changed to reflect the application of a filter to the feature class. In the attribute table, you can view a list of all selected feature and, by looking at the top of the table, you can determine how many features met the parameters of your selection (46 in this case).

<p align="center">
  <img src="https://github.com/jacobmswisher/images/blob/main/ArcGIS%20Online/Figure%2042.JPG">
</p>

Congratulations! You have succesfully used filters to answer our workshop research question.

*Tip: To remove a filter, retun to the filter tool pane and click the remove filter button.*

<p align="center">
  <img src="https://github.com/jacobmswisher/images/blob/main/ArcGIS%20Online/Figure%2043.JPG">
</p>

### Exercise 5: Using Filters

**Task: Using the filters tool and the Administrative Forest Boundaries feature layer, answer the following questions.**
1. How many national forests are in the Southern Region (08)?
2. How many national forests have a name that starts with the letter A?
3. How many forests contain more than 1,000,000 acres of land but less than 2,000,000 acres of land?
4. Which national forest is in the Eastern Region (09), contains "Mountain" in its name, and is smaller than 900,000 acres?

[Answer Key](https://github.com/jacobmswisher/ArcGIS-Online/blob/main/Sections/Part%207%20-%20Resources.md#exercise-5-answer-key)

[<<< Previous](Part4.md) | [Next >>>](Part6.md)  
