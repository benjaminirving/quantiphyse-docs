=======================
Loading and Saving Data
=======================

File Formats
============

This software package works with NIFTI volumes. DICOM files will need to be converted to NIFTI first using one 
of a number of tools including: 

 - `itk-snap <http://www.itksnap.org/pmwiki/pmwiki.php>`_
 - `dcm2nii <https://www.nitrc.org/plugins/mwiki/index.php/dcm2nii:MainPage>`_
 - Or the batch version which allows a number of volumes to be converted 
   `dcm2niibatch <https://github.com/rordenlab/dcm2niix>`_

Loading data
============

Drag and drop
-------------

You can drag and drop single or multiple files onto the main window to load data. You will be prompted to 
choose the type of data:

.. image:: screenshots/drag_drop_choice.png

Generally the name can be left alone - changing it may be useful if you are loading multiple files with the same
name. If you drag and drop multiple files you will be asked to choose the type of each one. If you select *cancel* 
the data file will not be loaded.

menu
----

The following menu options can be used to load data files:

 - File -> Load Image Volume
 
.. image:: screenshots/1.png

When dragging and dropping, a window will pop up to specify whether the image is the 4D main volume, and ROI or an overlay. 

.. image:: screenshots/2.jpg

The image will appear in the 3 orthographic views. 

.. image:: screenshots/3.png

Load ROI and overlays
---------------------

Drag-and-drop or use the `File` menu to load overlays and ROIs in a similar way.

For overlays a type must be given - a list of standard types is provided or you can specify your own.

.. image:: screenshots/4.jpg

You can switch between loaded or generated overlays using the list box below the main viewing windows, or from the *current overlays* section of the **Volumes** widget. 

.. image:: screenshots/5.png

Save a screen shot or plot
--------------------------

- Right click on an image or plot
- Click *Export*
- A view box will appear with the various format options. 
- *svg* format will allow editing of the layers and nodes in inkscape or another vector graphics viewer. 

.. image:: screenshots/17.jpg

Save an overlay to NIFTI file
-----------------------------

File -> Save Current overlay