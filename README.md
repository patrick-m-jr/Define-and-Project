# Define-and-Project
Quick solution for defining and projecting several shapefiles with an undefined coordinate system. This is a v10.0 ESRI Toolbox

## Basics

This is a simple tool that will save a bunch of time.  Based on a workspace containing a group of shapefiles with undefined coordinate systems, it’ll read the number of shps in the workspace, define their projection, and then it’ll project data based on a designated projected coordinate system. It’s not super complex but definitely saves about 8-10 clicks per shp.

Four of the five fields on the tool are "required" while the last is optional.
1. Input workspace: Folder that containing undefined shapefiles.
2. Output workspace: Designated folder for newly "projected" shapefiles.
3. Select GCS: Highlight your GCS. This will "fix" all shapefiles in the original input workspace. 
4. Select PCS: This will create new, "projected shapefiles"
5. Add Custom Text to Generated Output: This is optional but is highly recommended considering that the tool uses the same name as the original shapefile. This optional allows you to add a prefix to the output such as a tag indicating the PCS, i.e.
```
input name = undefined.shp
output name = utm15_undefined.shp
```
<img src= "images/Define and Project.jpg" height = "400">


## Acknowledgments and Tech Used

* PYTHON 2.7, Lib ARCPY - ESRI Desktop v10.6



