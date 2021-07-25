# About                                                                                                

Repository for single- and multi-input multiprocessing clipping script tools.

The sets of files in this repository are specifically for applying multiprocessing enhancements to a geoprocessing clipping tool. The first set of files is for users who wish to use a single-input clipping function and the second set is for users applying the same function to multiple input clipping features.

Users should either use the paramertized script tool (.tbx) for use in ArcGIS Pro, or replace parameterization with local references to 1) a clipping shapefile or feature class, 2) features to be clipped, and 3) output location. Each feature in the clipping feature class will be used to clip the features in the to-be-clipped input feature class and exported to a defined folder. 

In the context of these scripts, multiprocessing allows for the breaking up of repetitive geoprocessing tasks that are independent of each other to make the overall runtime more efficient. For this repository, it is done through importing the multiprocessing module, creating a jobs list of tasks, calling a function called worker() which holds the geoprocessing statements in a separate SingleInputClipFunction.py or MultiInputClipFunction.py script, and then executing it.

![alt text](https://static.thenounproject.com/png/1390001-200.png)
