CellProfiler-plugins
====================
[![Build Status](https://travis-ci.org/CellProfiler/CellProfiler-plugins.svg?branch=master)](https://travis-ci.org/CellProfiler/CellProfiler-plugins)

A home for community-contributed and experimental CellProfiler modules. 

## Beginner-level instructions
Please see help here: https://github.com/CellProfiler/CellProfiler/blob/master/cellprofiler/data/help/other_plugins.rst

## system requirements
for windows

If you want to use deep learning module ClassifyPixels-UNet make sure you have [Visual Studio 2017](https://visualstudio.microsoft.com/downloads/) installed,
otherwise required python 2 [https://www.python.org/downloads/windows/](https://www.python.org/downloads/windows/)


## Use
1. Clone the CellProfiler-plugins from this repository by command:
    ```
    cd PLUGIN_DIRECTORY
    git clone https://github.com/CellProfiler/CellProfiler-plugins.git
    ```
    or download the CellProfiler-plugins from [link](https://github.com/CellProfiler/CellProfiler-plugins/archive/master.zip) and unzip all file to `PLUGIN_DIRECTORY`

1. Install required dependencies:
	```
	cd CellProfiler-plugins
	pip install -r requirements.txt
	```

    To install CellProfiler-plugins on a windows machine with support for the deep learning module ClassifyPixels-UNet make sure you have [Visual Studio 2017](https://visualstudio.microsoft.com/downloads/) installed first then use
    ```
    cd CellProfiler-plugins
    pip install -r requirements-windows.txt
    ```
    
    ---
    **Note**
    1. Must select `python2` features during install Visual Studio 2017.
    1. If return`'pip' is not recognized as an internal or external command, operable program or batch file.`, mean need give whole path of pip file. usally under c:\\Python27\\
    ---

1. Configure CellProfiler plugins directory in the GUI via `Preferences > CellProfiler plugins directory` (you will need to restart CellProfiler for the change to take effect). When running CellProfiler via the command line, use the `--plugins-directory` flag to specify the plugins directory, for example:
    ```
    cellprofiler --run --run-headless --project PROJECT_FILE --plugins-directory PLUGIN_DIRECTORY/CellProfiler-plugins
    ```
