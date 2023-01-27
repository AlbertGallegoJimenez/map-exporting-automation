# map_exporting_automatization
## Overview
This repository contains the necessary files and the description of the methodology followed for the automatization of mapping and exporting in ArcGIS Pro by using Notebooks.

So what framework has been used?
<p align="center"><img src="https://github.com/AlbertGallegoJimenez/map_exporting_automatization/blob/main/images/Framework.png", width=500></p>

On the one hand, **ArcGIS Pro** software has been used to build the map template, while the code that automates the process of mapping and exporting in image files has been developed in the form of **Jupyter Notebook**. This is an easy and simple process as the ArcGIS Pro software integrates the use of **Python** codes in the form of notebooks in a very friendly way.

## Contents of the repository
This repository is organised in two folders: 
+ <a href=https://github.com/AlbertGallegoJimenez/map_exporting_automatization/tree/main/data>data folder</a>
where the code is stored in a notebook (.ipynb), as well as the other files used in this task.
+ <a href=https://github.com/AlbertGallegoJimenez/map_exporting_automatization/tree/main/images>images folder</a>
where the images of this readme file are stored.

## Workflow description
First, let's make sure we have all the necessary files we're going to use:
<p align="center"><img src="https://github.com/AlbertGallegoJimenez/map_exporting_automatization/blob/main/images/Used_files.png", width=250></p>

The **ArcGIS project** is where the files are going to be uploaded. The **Shapefile** (using another spatial file also works, such as a File GDB) contains the data, distributed in fields, that we want to map. The **Symbology file** is an ArcGIS-specific file that contains instructions on how you want to represent the data (colours, labels, etc.) and is dependent on the geometry of the file. And finally, the **Jupyter Notebook** is where the code is written.

Then, we prepare the project with the map frame (in this case I also use another map frame, called "BaseMap" which is going to appear in the extent as a location map), the layout, and the notebook. In the table of contents you also need to have uploaded the layer (the shapefile) where the symbology file is to be applied.
<p align="center"><img src="https://github.com/AlbertGallegoJimenez/map_exporting_automatization/blob/main/images/Screenshot_project.png", width=500></p>

If we look in detail the attribute table, we can see the fields we are going to map.
<p align="center"><img src="https://github.com/AlbertGallegoJimenez/map_exporting_automatization/blob/main/images/Attribute_table.png", width=500></p>

We have to bear in mind, which items of the layout extent are static and which are dynamic (those that are going to be updated on each loop).
<p align="center"><img src="https://github.com/AlbertGallegoJimenez/map_exporting_automatization/blob/main/images/Screenshot_layout.png", width=500></p>

Finally, we run the notebook (see <a href=https://github.com/AlbertGallegoJimenez/map_exporting_automatization/blob/main/data/notebook_ArcGIS.ipynb>here</a>) and we get those kind of maps.
<p align="center"><img src="https://github.com/AlbertGallegoJimenez/map_exporting_automatization/blob/main/images/Map_HBE.png" width="300"/> <img src="https://github.com/AlbertGallegoJimenez/map_exporting_automatization/blob/main/data/Map_RBEPop.png" width="300"/> <img src="https://github.com/AlbertGallegoJimenez/map_exporting_automatization/blob/main/data/Map_VBETS.png" width="300"/></p>
