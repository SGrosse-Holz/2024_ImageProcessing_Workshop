Live-cell image processing workshop
===================================

This repository contains materials for a workshop on image processing in live-cell fluorescence microscopy taught at the NSF's 2024 International Summer School & Genome Architecture and Function Workshop.

Software
--------
For the first part of the workshop you will need to install [Fiji/ImageJ](https://imagej.net/software/fiji/downloads) and its [ThunderSTORM plug-in](https://zitmen.github.io/thunderstorm/) on your local machine **before coming to the workshop** (we will run into connection issues if everyone tried to download these at the same time). For detailed installation instructions see below.

The rest of the workshop runs in python, using a Jupyter notebook.
+ if you have a python environment set up on your local machine, you can just clone this repo and run everything locally. Again, please download and install everything **before coming to the workshop**; including the python dependencies. You can do so by executing the second cell of the workshop Jupyter notebook or installing the libraries listed there manually.
+ as an alternative, you can run the python part of the workshop in [Google Colab](https://colab.research.google.com/). In the "Open notebook" dialog, select "GitHub". Search for "SGrosse-Holz", select this repo ("2024_ImageProcessing_Workshop") and open the notebook in it. Follow the instructions in the first cell of the notebook.

Fiji, ThunderSTORM, and the data ( !! needs to be done before the workshop !! )
-------------------------------------------------------------------------------
+ **download Fiji**: go to the [Fiji website](https://imagej.net/software/fiji/downloads) and download the right version for your OS. This will be a zip-compressed folder.
  - **extract** the folder to a location in your user space
    + **on Windows** the recommended location is `C:\Users\<your user>\Fiji`. Note that the website warns against installing to `C:\Program Files`, since Fiji might not have write permissions there).
    + **on MacOS** extracting will produce a standalone app. Place it in (e.g.) `/Users/<your user>/`. Note that you might have to allow execution for the "unverified App" Fiji in Settings.
  - **locate Fiji's plug-in folder** (it should already contain a whole library of `.jar` files)
    + **on Windows** it should be at `Fiji.app\plugins`.
    + **on MacOS** right-click the Fiji app and select "Show package contents". This should open a Finder window where you can select the plugin folder.

+ **ThunderSTORM**: go to [the website](https://zitmen.github.io/thunderstorm/) and click the "download ThunderSTORM" button on the top left. You will be redirected to GitHub.
  - download the file `Thunder_STORM.jar` and
  - place it in Fiji's plug-in folder

+ **start Fiji/ImageJ**
  - **on Windows** it should be `Fiji.app\ImageJ-win64.exe` (not "Fiji"!).
  - **on MacOS** it is just the package you extracted from the zip folder.
  - check that `Plugins > ThunderSTORM` exists in the Menu bar.

+ create a new folder somewhere in your user space and **download the [raw data](https://github.com/SGrosse-Holz/2024_ImageProcessing_Workshop/raw/main/processing/localization_demo_U2OS_H2B_JF549.tif)** into it. You can also find this file under `processing/localization_demo_U2OS_H2B_JF549.tif`.
