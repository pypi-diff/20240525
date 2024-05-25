# Comparing `tmp/GMXvg-0.4.6.tar.gz` & `tmp/gmxvg-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GMXvg-0.4.6.tar", last modified: Tue Mar 26 08:04:11 2024, max compression
+gzip compressed data, was "gmxvg-0.4.8.tar", last modified: Sat May 25 05:42:01 2024, max compression
```

## Comparing `GMXvg-0.4.6.tar` & `gmxvg-0.4.8.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 vishalkumarsahu  (1000) root         (0)        0 2024-03-26 08:04:11.735820 GMXvg-0.4.6/
-drwxr-xr-x   0 vishalkumarsahu  (1000) root         (0)        0 2024-03-26 08:04:11.735820 GMXvg-0.4.6/GMXvg.egg-info/
--rw-r--r--   0 vishalkumarsahu  (1000) root         (0)     7326 2024-03-26 08:04:11.000000 GMXvg-0.4.6/GMXvg.egg-info/PKG-INFO
--rw-r--r--   0 vishalkumarsahu  (1000) root         (0)      241 2024-03-26 08:04:11.000000 GMXvg-0.4.6/GMXvg.egg-info/SOURCES.txt
--rw-r--r--   0 vishalkumarsahu  (1000) root         (0)        1 2024-03-26 08:04:11.000000 GMXvg-0.4.6/GMXvg.egg-info/dependency_links.txt
--rw-r--r--   0 vishalkumarsahu  (1000) root         (0)       40 2024-03-26 08:04:11.000000 GMXvg-0.4.6/GMXvg.egg-info/entry_points.txt
--rw-r--r--   0 vishalkumarsahu  (1000) root         (0)       35 2024-03-26 08:04:11.000000 GMXvg-0.4.6/GMXvg.egg-info/requires.txt
--rw-r--r--   0 vishalkumarsahu  (1000) root         (0)        6 2024-03-26 08:04:11.000000 GMXvg-0.4.6/GMXvg.egg-info/top_level.txt
--rw-r--r--   0 vishalkumarsahu  (1000) root         (0)        0 2023-08-29 07:25:17.000000 GMXvg-0.4.6/LICENSE
--rw-r--r--   0 vishalkumarsahu  (1000) root         (0)     7326 2024-03-26 08:04:11.735820 GMXvg-0.4.6/PKG-INFO
--rw-r--r--   0 vishalkumarsahu  (1000) root         (0)     6750 2024-03-26 07:58:47.000000 GMXvg-0.4.6/README.md
-drwxr-xr-x   0 vishalkumarsahu  (1000) root         (0)        0 2024-03-26 08:04:11.735820 GMXvg-0.4.6/gmxvg/
--rw-r--r--   0 vishalkumarsahu  (1000) root         (0)    13364 2024-03-26 08:03:18.000000 GMXvg-0.4.6/gmxvg/GMXvg.py
--rw-r--r--   0 vishalkumarsahu  (1000) root         (0)       35 2024-03-26 08:03:27.000000 GMXvg-0.4.6/gmxvg/__init__.py
--rw-r--r--   0 vishalkumarsahu  (1000) root         (0)      826 2024-03-26 08:03:51.000000 GMXvg-0.4.6/pyproject.toml
--rw-r--r--   0 vishalkumarsahu  (1000) root         (0)       38 2024-03-26 08:04:11.735820 GMXvg-0.4.6/setup.cfg
+drwxr-xr-x   0 vishalkumarsahu  (1000) root         (0)        0 2024-05-25 05:42:01.889238 gmxvg-0.4.8/
+drwxr-xr-x   0 vishalkumarsahu  (1000) root         (0)        0 2024-05-25 05:42:01.885238 gmxvg-0.4.8/GMXvg.egg-info/
+-rw-r--r--   0 vishalkumarsahu  (1000) root         (0)     6259 2024-05-25 05:42:01.000000 gmxvg-0.4.8/GMXvg.egg-info/PKG-INFO
+-rw-r--r--   0 vishalkumarsahu  (1000) root         (0)      263 2024-05-25 05:42:01.000000 gmxvg-0.4.8/GMXvg.egg-info/SOURCES.txt
+-rw-r--r--   0 vishalkumarsahu  (1000) root         (0)        1 2024-05-25 05:42:01.000000 gmxvg-0.4.8/GMXvg.egg-info/dependency_links.txt
+-rw-r--r--   0 vishalkumarsahu  (1000) root         (0)       44 2024-05-25 05:42:01.000000 gmxvg-0.4.8/GMXvg.egg-info/entry_points.txt
+-rw-r--r--   0 vishalkumarsahu  (1000) root         (0)       35 2024-05-25 05:42:01.000000 gmxvg-0.4.8/GMXvg.egg-info/requires.txt
+-rw-r--r--   0 vishalkumarsahu  (1000) root         (0)        6 2024-05-25 05:42:01.000000 gmxvg-0.4.8/GMXvg.egg-info/top_level.txt
+-rw-r--r--   0 vishalkumarsahu  (1000) root         (0)    35829 2024-05-22 09:54:56.000000 gmxvg-0.4.8/LICENSE
+-rw-r--r--   0 vishalkumarsahu  (1000) root         (0)     6259 2024-05-25 05:42:01.889238 gmxvg-0.4.8/PKG-INFO
+-rw-r--r--   0 vishalkumarsahu  (1000) root         (0)     5661 2024-04-13 10:52:09.000000 gmxvg-0.4.8/README.md
+drwxr-xr-x   0 vishalkumarsahu  (1000) root         (0)        0 2024-05-25 05:42:01.885238 gmxvg-0.4.8/gmxvg/
+-rw-r--r--   0 vishalkumarsahu  (1000) root         (0)    14393 2024-05-25 05:40:26.000000 gmxvg-0.4.8/gmxvg/GMXvg.py
+-rw-r--r--   0 vishalkumarsahu  (1000) root         (0)      158 2024-05-25 04:17:03.000000 gmxvg-0.4.8/gmxvg/__init__.py
+-rw-r--r--   0 vishalkumarsahu  (1000) root         (0)      405 2024-05-25 04:04:42.000000 gmxvg-0.4.8/gmxvg/__metadata__.py
+-rw-r--r--   0 vishalkumarsahu  (1000) root         (0)      830 2024-05-25 04:34:03.000000 gmxvg-0.4.8/pyproject.toml
+-rw-r--r--   0 vishalkumarsahu  (1000) root         (0)       38 2024-05-25 05:42:01.889238 gmxvg-0.4.8/setup.cfg
```

### Comparing `GMXvg-0.4.6/GMXvg.egg-info/PKG-INFO` & `gmxvg-0.4.8/GMXvg.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GMXvg
-Version: 0.4.6
+Version: 0.4.8
 Summary: A tool to plot GROMACS .xvg files.
 Author-email: Vishal Kumar Sahu <mail@vishalkumarsahu.in>
 Project-URL: Homepage, https://github.com/TheBiomics/GMXvg
 Project-URL: Issues, https://github.com/TheBiomics/GMXvg/issues
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.8
@@ -15,133 +15,111 @@
 License-File: LICENSE
 Requires-Dist: UtilityLib
 Requires-Dist: pandas
 Requires-Dist: matplotlib
 Requires-Dist: latex
 
 
-```diff
-> Get older binaries for Ubuntu and Windows here -> [GMXvg v0.3](https://github.com/TheBiomics/GMXvg/releases/tag/v0.3) .
-```
-
-# GMXvg: Utility to Convert/Plot GROMACS XVG files (#xmgrace)
-
-* Commandline based GROMACS XVG File plotting utility.
-* Discovers all the XVG files in the current or subdirectories and converts them in specified file formats (default JPG).
-* Logs the summary of plots in a file (CSV file) to quickly access the plot values along with their standard deviation values.
-* This tool may be an alternative to `xmgrace`.
+# GMXvg: A tool to plot GROMACS .xvg files
 
-## Supported Platforms
+GMXvg is a command-line utility designed for converting and plotting GROMACS XVG files. It simplifies the process of handling XVG files by automatically discovering all XVG files in the current or subdirectories and converting them to specified file formats, with JPG as the default format. Additionally, GMXvg logs the summary of plots in a CSV file, providing quick access to plot values along with their standard deviation.
 
-The utility was developed and tested for following OS. However, we expect it to work on all windows and linux environment.
+## Features
+* Automatically discovers and converts GROMACS XVG files.
+* Supports conversion to multiple file formats (e.g., JPG, PNG, PDF).
+* Logs plot summaries in a CSV file for easy access to plot values and standard deviations.
+* Provides options to customize plot titles, legends, and other outputs.
+* Merge multiple plots
 
-## Easy to install and use
+## Quick Installation and Usage
 
 Install using pypi or other directly from source using python's pip module:
 
 * Install using: `pip install gmxvg`
 * Check Version: `gmxvg --version`
-* Usage:
-  - Switch to the directory where XVG files are located `cd <xvg-file-directory`
-  - Run `xvg`
-  - See further instructions to modify title, legends, or other outputs
+* Help options: `gmxvg -h`
+* Video tutorial or demo
+
+[Watch Demo](https://www.youtube.com/watch?v=99Eeqjp_0kI)
+
+[![Watch Demo](https://img.youtube.com/vi/99Eeqjp_0kI/0.jpg)](https://www.youtube.com/watch?v=99Eeqjp_0kI)
+
+* Example CSV output
+
+![image](https://user-images.githubusercontent.com/87003331/168798303-330a9d46-2fed-4a53-b05f-35307b3a939f.png)
+
+## Supported Platforms
+
+GMXvg is developed and tested for Ubuntu (20, 22, 24) and Windows (10, 11) environments. However, it is expected to work on all Windows, Linux, and macOS platforms.
 
-## Command Structure
+## Customise output
+### Command Structure
 
 * `gmxvg --<key>=<value>`: Double dash separated by equal sign
 * `gmxvg -<key> <val1> <val2> <val3>` Single dash (single dash is not recommended) and multiple values
 
-## Supported overriding variables
+### Overriding default variables
 Use `gmxvg -h` to see all options.
 
   * `path_base`: Base path if running from different directory
   * `csv_filename`: File name for CSV output else default will be used
   * `csv_filepath`: Path where CSV output file will be stored
-  * `path_move`: Path where generated images will be moved (will be deleted from the dir where XVG are stored)
-  * `path_copy`: Path where generated images will be copied (source graphics will be there)
-  * `pattern_xvg`: Pattern to specify XVG images for conversion e.g., *--new.xvg, old-*-temp-300.xvg
-  * `merge_patterns`: Pattern to select XVGs to group their output e.g., Protein-*-RMSD.xvg
-  * `export_ext`: Type of outputs, e.g., JPEG, PNG, JPG, PDF (Anything supported by Matplotlib)
-  * `dpi`: Resolution of the output, e.g., 72 for quick visualisation and 600 for many publications
-  * `flag_plot_mean`: yes|no; Use yes to enable plotting average line
-  * `flag_plot_std`: yes|no; Use yes to enable plotting standard deviation lines
-  * `flag_export_csv`: yes|no; If results should be exported in the form of CSV (includes directory name, file name, average of lines plotted and their standard deviation)
-  * `flag_export_plot`: yes|no; To specify if graphics should be exported or not
-
-## Exe Files (download and go solution!)
-
-* **Download [GMXvg executable file (Windows 10/11)](https://github.com/TheBiomics/GMXvg/releases/download/v0.3/gmxvg-win-v0.3.exe) (_or check [latest or compatible executable](https://github.com/TheBiomics/GMXvg/releases) for improved features_) and copy/paste the exe file in the directory where XVG is contained. It will discover all xvg extension files in current or child folders and process them automatically.**
-* After execution all xvgs will be converted to jpg. For example, "rmsd-protein.xvg" will be converted to "rmsd-protein.dpi300.jpeg".
-* After execution a CSV file containing mean and standard deviation of of the plotted lines in each xvg. For example, for gyration plot "gyration.xvg", the CSV file will show following columns
-  - `dir`: where xvg was stored
-  - `file`: name of the processed xvg file
-  - `plot`: label of the plotted line
-  - `mean`: Mean of the plotted line
-  - `std`: Standard deviation for the plotted line
-* Example result output
+  * `path_move`: Path where generated images will be moved (images will be deleted from the dir where XVG are stored)
+  * `path_copy`: Path where generated images will be copied (source graphics will NOT be deleted)
+  * `pattern_xvg`: Pattern to specify XVG images for conversion e.g., *--new.xvg, *-RMSD*.xvg (Helpful when you want to convert some selected files)
+  * `merge_patterns`: Pattern to select XVGs to group their output e.g., Protein-*-RMSD.xvg (This will merge file names matching the pattern into single graph for comparative visualisation)
+  * `export_ext`: Type of outputs, e.g., JPEG, PNG, JPG, PDF (Any output format supported by Matplotlib)
+  * `dpi`: Resolution of the output, e.g., 72 for quick visualisation and 600 for standard publications
+  * `flag_plot_mean`: yes|no; Use yes to enable plotting average value line
+  * `flag_plot_std`: yes|no; Use yes to enable plotting standard deviation line
+  * `flag_export_csv`: yes|no; If results should be exported in a CSV file (includes directory name, file name, average of lines plotted and their standard deviation)
+  * `flag_export_plot`: yes|no; To specify if graphics should be exported or not (in case only values are needed)
 
-![image](https://user-images.githubusercontent.com/87003331/168798303-330a9d46-2fed-4a53-b05f-35307b3a939f.png)
-
-* To obtain customised output or results see commandline operations and customisation section.
-
-## Example Commands (using source code or executable file)
-
-The utility finds *.xvg files in a directory or sub-directory. It need not to specify a file. This utility is made for bulk conversion of XVG files and extract the results in a separate directory.
+## Executable Files (Older version NOT RECOMMENDED!)
 
-### Simple (directly opening gxmvg executable file)
-This will discover XVG files in the subdirectory where `gmxvg` executable is present and plot XVG in JPEG Format
-* `gmxvg`
+* **Download [GMXvg executable file (Windows 10/11)](https://github.com/TheBiomics/GMXvg/releases/download/v0.3/gmxvg-win-v0.3.exe) and copy/paste the exe file in the directory where XVGs are contained. It will discover all xvg extension files in current or child folders and process them automatically.**
 
-### Custom options using commandline
-* `gmxvg -b <path-to-dir-containing-xvg-files>`
+### _path_base_: Define path if not running from the same directory
+* `gmxvg --path_base <path-to-dir-containing-xvg-files>`
 
-### Generate multiple qualities of graphics
+### _dpi_: Generate multiple qualities of graphics
 * `gmxvg --dpi 96 300 600 --path_copy <path-to-aggregate-results-outside>`
 
+### _path_copy_: Copy all the generated graphs to another directory
+* `gmxvg --path_copy <path-to-aggregate-results-outside>`
+
 ### Export in multiple format(s)
 * `gmxvg --export_ext JPEG pdf`
 
-### Other customisations and advance functions
+### _merge_patterns_: Merging multiple plots
 
-* To **merge multiple xvg files** having ending (e.g., /complex1/lig.xvg, /complex2/lig.xvg, /complex3/lig.xvg) passed to `-merge_patterns RMSD.xvg` so that it will combine all to plot one file. `--uid_part -1` parameter can be useful to define the Legend of the merged graphs.
+* To **merge multiple xvg files** having ending (e.g., /complex1/lig.xvg, /complex2/lig.xvg, /complex3/lig.xvg) passed to `--merge_patterns RMSD.xvg` so that it will combine all to plot one file. `--uid_part -1` parameter can be useful to define the Legend of the merged graphs.
 
-```gmxvg --dpi 96 -merge_patterns RMSD-of-Ligand.xvg RMSD-of-Protein-C-Alpha.xvg Gyration-of-Protein.xvg NPT-Temperature.xvg Inter-Ligand-Protein-H-Bonds.xvg --replacements "Receptor1--Lig2":p53-miR5 "Recptor2--Lig3":p53-miR3 --path_move <path-to-output-dir>/graphs```
+```gmxvg --merge_patterns RMSD-of-Ligand.xvg RMSD-of-Protein-C-Alpha.xvg Gyration-of-Protein.xvg NPT-Temperature.xvg Inter-Ligand-Protein-H-Bonds.xvg```
 
 * Example to merge Protein-RMSD.xvg and Ligand-RMSD.xvg files in the same directory.
-```gmxvg -merge_patterns RMSD.xvg -uid_part -1```
+```gmxvg --merge_patterns RMSD.xvg --uid_part -1```
+
+### Managing texts on the plots
 
 * Use `-replacements` options to replace any text in the plot will change the labels and legends of the plot
+```gmxvg --replacements "Receptor1--Lig2":p53-miR5 "Recptor2--Lig3":p53-miR3```
 
-## Development
+## Development and Future Plans
 
-* To make any changes, fork this repository
-* To contribute, create a pull request after you fork or comment
+GMXvg is open-source and welcomes contributions. Future plans include:
 
-### Development and Testing to Create Executable Files
+* GUI or web interface for interactive visualization.
+* Customizable labels and text through GUI.
+* Fast and efficient executable.
 
-* `python -m venv <path-to>-env` for Windows and `sudo apt-get install python3.8-venv` for Ubuntu
-* Install missing packages
-* `<path-to>-env/Scripts/activate` for Windows and `source <path-to>-env/bin/activate` for Ubuntu
-* `pip install pyinstaller`
-* `pyinstaller gmxvg --onefile`
-
-## Future Plans
-
-* GUI or web interface through local server for [interactive visualisation](https://www.chartjs.org/docs/latest/samples/animations/progressive-line.html)
-* Edit labels or text for invidiual graphs through GUI
-* Small executable size
-* Fast Executable
-* Webserver to convert and combine graphs
+For development and contributions, fork the repository or create a pull request.
 
 ## Accessory Details
-* We recommend you going through the code to access the precision and quality of the generated results before you use.
-* The code is free to be used by students, scholars, and professors.
-* Version 0.4 details
-  - DOI: [doi:10.5281/zenodo.7395525](https://doi.org/10.5281/zenodo.7395525)
-  - Authors: Vishal Kumar Sahu and Dr. Soumya Basu
-  - Title: GMXvg: GROMACS XVG Graph Plotting Tool Version 0.4
-  - Month & Year: December, 2022
-  - Published on: Zenodo
+* The code is free to use by students, scholars, and professors.
+* If you find the work useful and want to provide credit, you can cite the source code using [DOI:10.5281/zenodo.6563931](https://dx.doi.org/10.5281/zenodo.6563931).
 
 ## Troubleshooting installation
+If you encounter installation issues, try using the pip cache purge command `pip cache purge`.
+
+
 
-* Use `pip cache purge` in case of installation issue
```

### Comparing `GMXvg-0.4.6/PKG-INFO` & `gmxvg-0.4.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GMXvg
-Version: 0.4.6
+Version: 0.4.8
 Summary: A tool to plot GROMACS .xvg files.
 Author-email: Vishal Kumar Sahu <mail@vishalkumarsahu.in>
 Project-URL: Homepage, https://github.com/TheBiomics/GMXvg
 Project-URL: Issues, https://github.com/TheBiomics/GMXvg/issues
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.8
@@ -15,133 +15,111 @@
 License-File: LICENSE
 Requires-Dist: UtilityLib
 Requires-Dist: pandas
 Requires-Dist: matplotlib
 Requires-Dist: latex
 
 
-```diff
-> Get older binaries for Ubuntu and Windows here -> [GMXvg v0.3](https://github.com/TheBiomics/GMXvg/releases/tag/v0.3) .
-```
-
-# GMXvg: Utility to Convert/Plot GROMACS XVG files (#xmgrace)
-
-* Commandline based GROMACS XVG File plotting utility.
-* Discovers all the XVG files in the current or subdirectories and converts them in specified file formats (default JPG).
-* Logs the summary of plots in a file (CSV file) to quickly access the plot values along with their standard deviation values.
-* This tool may be an alternative to `xmgrace`.
+# GMXvg: A tool to plot GROMACS .xvg files
 
-## Supported Platforms
+GMXvg is a command-line utility designed for converting and plotting GROMACS XVG files. It simplifies the process of handling XVG files by automatically discovering all XVG files in the current or subdirectories and converting them to specified file formats, with JPG as the default format. Additionally, GMXvg logs the summary of plots in a CSV file, providing quick access to plot values along with their standard deviation.
 
-The utility was developed and tested for following OS. However, we expect it to work on all windows and linux environment.
+## Features
+* Automatically discovers and converts GROMACS XVG files.
+* Supports conversion to multiple file formats (e.g., JPG, PNG, PDF).
+* Logs plot summaries in a CSV file for easy access to plot values and standard deviations.
+* Provides options to customize plot titles, legends, and other outputs.
+* Merge multiple plots
 
-## Easy to install and use
+## Quick Installation and Usage
 
 Install using pypi or other directly from source using python's pip module:
 
 * Install using: `pip install gmxvg`
 * Check Version: `gmxvg --version`
-* Usage:
-  - Switch to the directory where XVG files are located `cd <xvg-file-directory`
-  - Run `xvg`
-  - See further instructions to modify title, legends, or other outputs
+* Help options: `gmxvg -h`
+* Video tutorial or demo
+
+[Watch Demo](https://www.youtube.com/watch?v=99Eeqjp_0kI)
+
+[![Watch Demo](https://img.youtube.com/vi/99Eeqjp_0kI/0.jpg)](https://www.youtube.com/watch?v=99Eeqjp_0kI)
+
+* Example CSV output
+
+![image](https://user-images.githubusercontent.com/87003331/168798303-330a9d46-2fed-4a53-b05f-35307b3a939f.png)
+
+## Supported Platforms
+
+GMXvg is developed and tested for Ubuntu (20, 22, 24) and Windows (10, 11) environments. However, it is expected to work on all Windows, Linux, and macOS platforms.
 
-## Command Structure
+## Customise output
+### Command Structure
 
 * `gmxvg --<key>=<value>`: Double dash separated by equal sign
 * `gmxvg -<key> <val1> <val2> <val3>` Single dash (single dash is not recommended) and multiple values
 
-## Supported overriding variables
+### Overriding default variables
 Use `gmxvg -h` to see all options.
 
   * `path_base`: Base path if running from different directory
   * `csv_filename`: File name for CSV output else default will be used
   * `csv_filepath`: Path where CSV output file will be stored
-  * `path_move`: Path where generated images will be moved (will be deleted from the dir where XVG are stored)
-  * `path_copy`: Path where generated images will be copied (source graphics will be there)
-  * `pattern_xvg`: Pattern to specify XVG images for conversion e.g., *--new.xvg, old-*-temp-300.xvg
-  * `merge_patterns`: Pattern to select XVGs to group their output e.g., Protein-*-RMSD.xvg
-  * `export_ext`: Type of outputs, e.g., JPEG, PNG, JPG, PDF (Anything supported by Matplotlib)
-  * `dpi`: Resolution of the output, e.g., 72 for quick visualisation and 600 for many publications
-  * `flag_plot_mean`: yes|no; Use yes to enable plotting average line
-  * `flag_plot_std`: yes|no; Use yes to enable plotting standard deviation lines
-  * `flag_export_csv`: yes|no; If results should be exported in the form of CSV (includes directory name, file name, average of lines plotted and their standard deviation)
-  * `flag_export_plot`: yes|no; To specify if graphics should be exported or not
-
-## Exe Files (download and go solution!)
-
-* **Download [GMXvg executable file (Windows 10/11)](https://github.com/TheBiomics/GMXvg/releases/download/v0.3/gmxvg-win-v0.3.exe) (_or check [latest or compatible executable](https://github.com/TheBiomics/GMXvg/releases) for improved features_) and copy/paste the exe file in the directory where XVG is contained. It will discover all xvg extension files in current or child folders and process them automatically.**
-* After execution all xvgs will be converted to jpg. For example, "rmsd-protein.xvg" will be converted to "rmsd-protein.dpi300.jpeg".
-* After execution a CSV file containing mean and standard deviation of of the plotted lines in each xvg. For example, for gyration plot "gyration.xvg", the CSV file will show following columns
-  - `dir`: where xvg was stored
-  - `file`: name of the processed xvg file
-  - `plot`: label of the plotted line
-  - `mean`: Mean of the plotted line
-  - `std`: Standard deviation for the plotted line
-* Example result output
+  * `path_move`: Path where generated images will be moved (images will be deleted from the dir where XVG are stored)
+  * `path_copy`: Path where generated images will be copied (source graphics will NOT be deleted)
+  * `pattern_xvg`: Pattern to specify XVG images for conversion e.g., *--new.xvg, *-RMSD*.xvg (Helpful when you want to convert some selected files)
+  * `merge_patterns`: Pattern to select XVGs to group their output e.g., Protein-*-RMSD.xvg (This will merge file names matching the pattern into single graph for comparative visualisation)
+  * `export_ext`: Type of outputs, e.g., JPEG, PNG, JPG, PDF (Any output format supported by Matplotlib)
+  * `dpi`: Resolution of the output, e.g., 72 for quick visualisation and 600 for standard publications
+  * `flag_plot_mean`: yes|no; Use yes to enable plotting average value line
+  * `flag_plot_std`: yes|no; Use yes to enable plotting standard deviation line
+  * `flag_export_csv`: yes|no; If results should be exported in a CSV file (includes directory name, file name, average of lines plotted and their standard deviation)
+  * `flag_export_plot`: yes|no; To specify if graphics should be exported or not (in case only values are needed)
 
-![image](https://user-images.githubusercontent.com/87003331/168798303-330a9d46-2fed-4a53-b05f-35307b3a939f.png)
-
-* To obtain customised output or results see commandline operations and customisation section.
-
-## Example Commands (using source code or executable file)
-
-The utility finds *.xvg files in a directory or sub-directory. It need not to specify a file. This utility is made for bulk conversion of XVG files and extract the results in a separate directory.
+## Executable Files (Older version NOT RECOMMENDED!)
 
-### Simple (directly opening gxmvg executable file)
-This will discover XVG files in the subdirectory where `gmxvg` executable is present and plot XVG in JPEG Format
-* `gmxvg`
+* **Download [GMXvg executable file (Windows 10/11)](https://github.com/TheBiomics/GMXvg/releases/download/v0.3/gmxvg-win-v0.3.exe) and copy/paste the exe file in the directory where XVGs are contained. It will discover all xvg extension files in current or child folders and process them automatically.**
 
-### Custom options using commandline
-* `gmxvg -b <path-to-dir-containing-xvg-files>`
+### _path_base_: Define path if not running from the same directory
+* `gmxvg --path_base <path-to-dir-containing-xvg-files>`
 
-### Generate multiple qualities of graphics
+### _dpi_: Generate multiple qualities of graphics
 * `gmxvg --dpi 96 300 600 --path_copy <path-to-aggregate-results-outside>`
 
+### _path_copy_: Copy all the generated graphs to another directory
+* `gmxvg --path_copy <path-to-aggregate-results-outside>`
+
 ### Export in multiple format(s)
 * `gmxvg --export_ext JPEG pdf`
 
-### Other customisations and advance functions
+### _merge_patterns_: Merging multiple plots
 
-* To **merge multiple xvg files** having ending (e.g., /complex1/lig.xvg, /complex2/lig.xvg, /complex3/lig.xvg) passed to `-merge_patterns RMSD.xvg` so that it will combine all to plot one file. `--uid_part -1` parameter can be useful to define the Legend of the merged graphs.
+* To **merge multiple xvg files** having ending (e.g., /complex1/lig.xvg, /complex2/lig.xvg, /complex3/lig.xvg) passed to `--merge_patterns RMSD.xvg` so that it will combine all to plot one file. `--uid_part -1` parameter can be useful to define the Legend of the merged graphs.
 
-```gmxvg --dpi 96 -merge_patterns RMSD-of-Ligand.xvg RMSD-of-Protein-C-Alpha.xvg Gyration-of-Protein.xvg NPT-Temperature.xvg Inter-Ligand-Protein-H-Bonds.xvg --replacements "Receptor1--Lig2":p53-miR5 "Recptor2--Lig3":p53-miR3 --path_move <path-to-output-dir>/graphs```
+```gmxvg --merge_patterns RMSD-of-Ligand.xvg RMSD-of-Protein-C-Alpha.xvg Gyration-of-Protein.xvg NPT-Temperature.xvg Inter-Ligand-Protein-H-Bonds.xvg```
 
 * Example to merge Protein-RMSD.xvg and Ligand-RMSD.xvg files in the same directory.
-```gmxvg -merge_patterns RMSD.xvg -uid_part -1```
+```gmxvg --merge_patterns RMSD.xvg --uid_part -1```
+
+### Managing texts on the plots
 
 * Use `-replacements` options to replace any text in the plot will change the labels and legends of the plot
+```gmxvg --replacements "Receptor1--Lig2":p53-miR5 "Recptor2--Lig3":p53-miR3```
 
-## Development
+## Development and Future Plans
 
-* To make any changes, fork this repository
-* To contribute, create a pull request after you fork or comment
+GMXvg is open-source and welcomes contributions. Future plans include:
 
-### Development and Testing to Create Executable Files
+* GUI or web interface for interactive visualization.
+* Customizable labels and text through GUI.
+* Fast and efficient executable.
 
-* `python -m venv <path-to>-env` for Windows and `sudo apt-get install python3.8-venv` for Ubuntu
-* Install missing packages
-* `<path-to>-env/Scripts/activate` for Windows and `source <path-to>-env/bin/activate` for Ubuntu
-* `pip install pyinstaller`
-* `pyinstaller gmxvg --onefile`
-
-## Future Plans
-
-* GUI or web interface through local server for [interactive visualisation](https://www.chartjs.org/docs/latest/samples/animations/progressive-line.html)
-* Edit labels or text for invidiual graphs through GUI
-* Small executable size
-* Fast Executable
-* Webserver to convert and combine graphs
+For development and contributions, fork the repository or create a pull request.
 
 ## Accessory Details
-* We recommend you going through the code to access the precision and quality of the generated results before you use.
-* The code is free to be used by students, scholars, and professors.
-* Version 0.4 details
-  - DOI: [doi:10.5281/zenodo.7395525](https://doi.org/10.5281/zenodo.7395525)
-  - Authors: Vishal Kumar Sahu and Dr. Soumya Basu
-  - Title: GMXvg: GROMACS XVG Graph Plotting Tool Version 0.4
-  - Month & Year: December, 2022
-  - Published on: Zenodo
+* The code is free to use by students, scholars, and professors.
+* If you find the work useful and want to provide credit, you can cite the source code using [DOI:10.5281/zenodo.6563931](https://dx.doi.org/10.5281/zenodo.6563931).
 
 ## Troubleshooting installation
+If you encounter installation issues, try using the pip cache purge command `pip cache purge`.
+
+
 
-* Use `pip cache purge` in case of installation issue
```

### Comparing `GMXvg-0.4.6/README.md` & `gmxvg-0.4.8/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,127 +1,105 @@
 
-```diff
-> Get older binaries for Ubuntu and Windows here -> [GMXvg v0.3](https://github.com/TheBiomics/GMXvg/releases/tag/v0.3) .
-```
-
-# GMXvg: Utility to Convert/Plot GROMACS XVG files (#xmgrace)
-
-* Commandline based GROMACS XVG File plotting utility.
-* Discovers all the XVG files in the current or subdirectories and converts them in specified file formats (default JPG).
-* Logs the summary of plots in a file (CSV file) to quickly access the plot values along with their standard deviation values.
-* This tool may be an alternative to `xmgrace`.
+# GMXvg: A tool to plot GROMACS .xvg files
 
-## Supported Platforms
+GMXvg is a command-line utility designed for converting and plotting GROMACS XVG files. It simplifies the process of handling XVG files by automatically discovering all XVG files in the current or subdirectories and converting them to specified file formats, with JPG as the default format. Additionally, GMXvg logs the summary of plots in a CSV file, providing quick access to plot values along with their standard deviation.
 
-The utility was developed and tested for following OS. However, we expect it to work on all windows and linux environment.
+## Features
+* Automatically discovers and converts GROMACS XVG files.
+* Supports conversion to multiple file formats (e.g., JPG, PNG, PDF).
+* Logs plot summaries in a CSV file for easy access to plot values and standard deviations.
+* Provides options to customize plot titles, legends, and other outputs.
+* Merge multiple plots
 
-## Easy to install and use
+## Quick Installation and Usage
 
 Install using pypi or other directly from source using python's pip module:
 
 * Install using: `pip install gmxvg`
 * Check Version: `gmxvg --version`
-* Usage:
-  - Switch to the directory where XVG files are located `cd <xvg-file-directory`
-  - Run `xvg`
-  - See further instructions to modify title, legends, or other outputs
+* Help options: `gmxvg -h`
+* Video tutorial or demo
+
+[Watch Demo](https://www.youtube.com/watch?v=99Eeqjp_0kI)
+
+[![Watch Demo](https://img.youtube.com/vi/99Eeqjp_0kI/0.jpg)](https://www.youtube.com/watch?v=99Eeqjp_0kI)
+
+* Example CSV output
+
+![image](https://user-images.githubusercontent.com/87003331/168798303-330a9d46-2fed-4a53-b05f-35307b3a939f.png)
+
+## Supported Platforms
+
+GMXvg is developed and tested for Ubuntu (20, 22, 24) and Windows (10, 11) environments. However, it is expected to work on all Windows, Linux, and macOS platforms.
 
-## Command Structure
+## Customise output
+### Command Structure
 
 * `gmxvg --<key>=<value>`: Double dash separated by equal sign
 * `gmxvg -<key> <val1> <val2> <val3>` Single dash (single dash is not recommended) and multiple values
 
-## Supported overriding variables
+### Overriding default variables
 Use `gmxvg -h` to see all options.
 
   * `path_base`: Base path if running from different directory
   * `csv_filename`: File name for CSV output else default will be used
   * `csv_filepath`: Path where CSV output file will be stored
-  * `path_move`: Path where generated images will be moved (will be deleted from the dir where XVG are stored)
-  * `path_copy`: Path where generated images will be copied (source graphics will be there)
-  * `pattern_xvg`: Pattern to specify XVG images for conversion e.g., *--new.xvg, old-*-temp-300.xvg
-  * `merge_patterns`: Pattern to select XVGs to group their output e.g., Protein-*-RMSD.xvg
-  * `export_ext`: Type of outputs, e.g., JPEG, PNG, JPG, PDF (Anything supported by Matplotlib)
-  * `dpi`: Resolution of the output, e.g., 72 for quick visualisation and 600 for many publications
-  * `flag_plot_mean`: yes|no; Use yes to enable plotting average line
-  * `flag_plot_std`: yes|no; Use yes to enable plotting standard deviation lines
-  * `flag_export_csv`: yes|no; If results should be exported in the form of CSV (includes directory name, file name, average of lines plotted and their standard deviation)
-  * `flag_export_plot`: yes|no; To specify if graphics should be exported or not
-
-## Exe Files (download and go solution!)
-
-* **Download [GMXvg executable file (Windows 10/11)](https://github.com/TheBiomics/GMXvg/releases/download/v0.3/gmxvg-win-v0.3.exe) (_or check [latest or compatible executable](https://github.com/TheBiomics/GMXvg/releases) for improved features_) and copy/paste the exe file in the directory where XVG is contained. It will discover all xvg extension files in current or child folders and process them automatically.**
-* After execution all xvgs will be converted to jpg. For example, "rmsd-protein.xvg" will be converted to "rmsd-protein.dpi300.jpeg".
-* After execution a CSV file containing mean and standard deviation of of the plotted lines in each xvg. For example, for gyration plot "gyration.xvg", the CSV file will show following columns
-  - `dir`: where xvg was stored
-  - `file`: name of the processed xvg file
-  - `plot`: label of the plotted line
-  - `mean`: Mean of the plotted line
-  - `std`: Standard deviation for the plotted line
-* Example result output
+  * `path_move`: Path where generated images will be moved (images will be deleted from the dir where XVG are stored)
+  * `path_copy`: Path where generated images will be copied (source graphics will NOT be deleted)
+  * `pattern_xvg`: Pattern to specify XVG images for conversion e.g., *--new.xvg, *-RMSD*.xvg (Helpful when you want to convert some selected files)
+  * `merge_patterns`: Pattern to select XVGs to group their output e.g., Protein-*-RMSD.xvg (This will merge file names matching the pattern into single graph for comparative visualisation)
+  * `export_ext`: Type of outputs, e.g., JPEG, PNG, JPG, PDF (Any output format supported by Matplotlib)
+  * `dpi`: Resolution of the output, e.g., 72 for quick visualisation and 600 for standard publications
+  * `flag_plot_mean`: yes|no; Use yes to enable plotting average value line
+  * `flag_plot_std`: yes|no; Use yes to enable plotting standard deviation line
+  * `flag_export_csv`: yes|no; If results should be exported in a CSV file (includes directory name, file name, average of lines plotted and their standard deviation)
+  * `flag_export_plot`: yes|no; To specify if graphics should be exported or not (in case only values are needed)
 
-![image](https://user-images.githubusercontent.com/87003331/168798303-330a9d46-2fed-4a53-b05f-35307b3a939f.png)
-
-* To obtain customised output or results see commandline operations and customisation section.
-
-## Example Commands (using source code or executable file)
-
-The utility finds *.xvg files in a directory or sub-directory. It need not to specify a file. This utility is made for bulk conversion of XVG files and extract the results in a separate directory.
+## Executable Files (Older version NOT RECOMMENDED!)
 
-### Simple (directly opening gxmvg executable file)
-This will discover XVG files in the subdirectory where `gmxvg` executable is present and plot XVG in JPEG Format
-* `gmxvg`
+* **Download [GMXvg executable file (Windows 10/11)](https://github.com/TheBiomics/GMXvg/releases/download/v0.3/gmxvg-win-v0.3.exe) and copy/paste the exe file in the directory where XVGs are contained. It will discover all xvg extension files in current or child folders and process them automatically.**
 
-### Custom options using commandline
-* `gmxvg -b <path-to-dir-containing-xvg-files>`
+### _path_base_: Define path if not running from the same directory
+* `gmxvg --path_base <path-to-dir-containing-xvg-files>`
 
-### Generate multiple qualities of graphics
+### _dpi_: Generate multiple qualities of graphics
 * `gmxvg --dpi 96 300 600 --path_copy <path-to-aggregate-results-outside>`
 
+### _path_copy_: Copy all the generated graphs to another directory
+* `gmxvg --path_copy <path-to-aggregate-results-outside>`
+
 ### Export in multiple format(s)
 * `gmxvg --export_ext JPEG pdf`
 
-### Other customisations and advance functions
+### _merge_patterns_: Merging multiple plots
 
-* To **merge multiple xvg files** having ending (e.g., /complex1/lig.xvg, /complex2/lig.xvg, /complex3/lig.xvg) passed to `-merge_patterns RMSD.xvg` so that it will combine all to plot one file. `--uid_part -1` parameter can be useful to define the Legend of the merged graphs.
+* To **merge multiple xvg files** having ending (e.g., /complex1/lig.xvg, /complex2/lig.xvg, /complex3/lig.xvg) passed to `--merge_patterns RMSD.xvg` so that it will combine all to plot one file. `--uid_part -1` parameter can be useful to define the Legend of the merged graphs.
 
-```gmxvg --dpi 96 -merge_patterns RMSD-of-Ligand.xvg RMSD-of-Protein-C-Alpha.xvg Gyration-of-Protein.xvg NPT-Temperature.xvg Inter-Ligand-Protein-H-Bonds.xvg --replacements "Receptor1--Lig2":p53-miR5 "Recptor2--Lig3":p53-miR3 --path_move <path-to-output-dir>/graphs```
+```gmxvg --merge_patterns RMSD-of-Ligand.xvg RMSD-of-Protein-C-Alpha.xvg Gyration-of-Protein.xvg NPT-Temperature.xvg Inter-Ligand-Protein-H-Bonds.xvg```
 
 * Example to merge Protein-RMSD.xvg and Ligand-RMSD.xvg files in the same directory.
-```gmxvg -merge_patterns RMSD.xvg -uid_part -1```
+```gmxvg --merge_patterns RMSD.xvg --uid_part -1```
+
+### Managing texts on the plots
 
 * Use `-replacements` options to replace any text in the plot will change the labels and legends of the plot
+```gmxvg --replacements "Receptor1--Lig2":p53-miR5 "Recptor2--Lig3":p53-miR3```
 
-## Development
+## Development and Future Plans
 
-* To make any changes, fork this repository
-* To contribute, create a pull request after you fork or comment
+GMXvg is open-source and welcomes contributions. Future plans include:
 
-### Development and Testing to Create Executable Files
+* GUI or web interface for interactive visualization.
+* Customizable labels and text through GUI.
+* Fast and efficient executable.
 
-* `python -m venv <path-to>-env` for Windows and `sudo apt-get install python3.8-venv` for Ubuntu
-* Install missing packages
-* `<path-to>-env/Scripts/activate` for Windows and `source <path-to>-env/bin/activate` for Ubuntu
-* `pip install pyinstaller`
-* `pyinstaller gmxvg --onefile`
-
-## Future Plans
-
-* GUI or web interface through local server for [interactive visualisation](https://www.chartjs.org/docs/latest/samples/animations/progressive-line.html)
-* Edit labels or text for invidiual graphs through GUI
-* Small executable size
-* Fast Executable
-* Webserver to convert and combine graphs
+For development and contributions, fork the repository or create a pull request.
 
 ## Accessory Details
-* We recommend you going through the code to access the precision and quality of the generated results before you use.
-* The code is free to be used by students, scholars, and professors.
-* Version 0.4 details
-  - DOI: [doi:10.5281/zenodo.7395525](https://doi.org/10.5281/zenodo.7395525)
-  - Authors: Vishal Kumar Sahu and Dr. Soumya Basu
-  - Title: GMXvg: GROMACS XVG Graph Plotting Tool Version 0.4
-  - Month & Year: December, 2022
-  - Published on: Zenodo
+* The code is free to use by students, scholars, and professors.
+* If you find the work useful and want to provide credit, you can cite the source code using [DOI:10.5281/zenodo.6563931](https://dx.doi.org/10.5281/zenodo.6563931).
 
 ## Troubleshooting installation
+If you encounter installation issues, try using the pip cache purge command `pip cache purge`.
+
+
 
-* Use `pip cache purge` in case of installation issue
```

### Comparing `GMXvg-0.4.6/gmxvg/GMXvg.py` & `gmxvg-0.4.8/gmxvg/GMXvg.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,73 +1,67 @@
-import os as OS
-import argparse as ARGUMENT
-import re as REGEX
-import pandas as PD
-from UtilityLib import UtilityManager
-import matplotlib.pyplot as PLOT
-import shutil as SHUtil
-
-class GMXvg(UtilityManager):
-  __package__ = "GMXvg"
-  __version__ = "0.4"
-  __subversion__ = "20230830"
-  __author__ = "Vishal Kumar Sahu"
+from . import __version__, __description__, __build__, __name__
+from UtilityLib import ProjectManager
 
+class GMXvg(ProjectManager):
+  __name__= __name__
+  __version__= __version__
+  __build__= __build__
+  __description__= __description__
+  name = __name__
+  version = __version__
+  version_info = f"{__version__} ({__build__})"
+  # log_level = 'info'
   def __init__(self, *args, **kwargs):
-    super(GMXvg, self).__init__(**kwargs)
-    _use_tex = True if SHUtil.which('latex') else False
-    PLOT.rcParams.update({
-      "text.usetex": _use_tex,
-      "font.family": "sans-serif",
-    })
-    self.__update_attr(**kwargs)
-
-  def __set_defaults(self):
-    self.csv_filepath = f"{self.path_base}{OS.sep}{self.csv_filename}"
+    super().__init__(**kwargs)
+    self.preset('data plot')
+    self.__set_defaults(**kwargs)
 
-  def __update_attr(self, *args, **kwargs):
-    if not hasattr(self, "__defaults"): self.__defaults =  {
+  def __set_defaults(self, *args, **kwargs):
+    __defaults =  {
         "replacements_gmx": {
           'Hydrogen bonds': None,
           'Rg': None,
           '(nm)': None,
           'RMSD (nm)': None,
           ".xvg": "",
           "Plot": ""
         },
         "replacements": {},
         "csv_filename": "XVG-Plot-Values.csv",
-        "csv_filepath": None,
-        "path_base": OS.getcwd(),
+        "path_base": self.OS.getcwd(),
         "path_move": None,
         "path_copy": None,
         "pattern_xvg": "*.xvg",
         "merge_patterns": [],
         "export_ext": ["jpg"],
         "dpi": 300,
         "flag_plot_mean": "yes",
         "flag_plot_std": "no",
         "flag_export_csv": "no",
         "flag_export_plot": "y",
         "uid_part": -2,
         "output_files": []
       }
 
-    # Set all defaults
-    [setattr(self, _k, self.__defaults[_k]) for _k in self.__defaults.keys() if not hasattr(self, _k)]
-    self.__defaults = dict() # Unset defaults to prevent running for second time
-    [setattr(self, _k, kwargs[_k]) for _k in kwargs.keys()]
-
-    self.__set_defaults()
+    __defaults.update(kwargs)
+    self.require('shutil', 'SHUtil')
+    _use_tex = True if self.SHUtil.which('latex') else False
+    self.PLOT.rcParams.update({
+      "text.usetex": _use_tex,
+      "font.family": "sans-serif",
+    })
+    self.require('re', 'REGEX')
+    self.update_attributes(self, __defaults)
 
-  def __plot_xvgs(self, *args, **kwargs):
-    _xvgs = args[0] if len(args) > 0 else kwargs.get("xvg_paths")
+  def _plot_xvgs(self, *args, **kwargs):
+    """Plots XVG files from the given list"""
+    _xvgs = kwargs.get("xvg_paths", args[0] if len(args) > 0 else None)
     _result_dict = []
     for _xvg in _xvgs:
-      _result = self.__plot_xvg(_xvg, **kwargs)
+      _result = self._plot_xvg(_xvg, **kwargs)
       _file_name = self.filename(_xvg)
       _dir_name = _xvg.split(self.path_base)[-1]
       _dir_name = _dir_name.replace(self.filename(_xvg, with_ext=True), "")
       _dir_name = _dir_name.strip("/")
       for _col in _result.columns[1:].tolist():
         _result_dict.append({
             "dir": _dir_name,
@@ -78,93 +72,100 @@
             "min": _result[_col].min(),
             "q_10": _result[_col].quantile(0.1),
             "q_50": _result[_col].quantile(0.5),
             "q_90": _result[_col].quantile(0.9),
             "max": _result[_col].max(),
         })
     if getattr(self, "flag_export_csv", False) and len(_result_dict) > 0:
-      _results = PD.DataFrame(_result_dict)
-      self.log_info(f"Writing results to {self.csv_filepath}.")
-      _results.to_csv(self.csv_filepath, index=False)
+      _results = self.DF(_result_dict)
+      self.log_info(f"Writing results to {self.csv_filename}.")
+      _results.to_csv(self.get_path(self.csv_filename), index=False)
     else:
       self.log_info("Not writing the results.", type="warn")
 
-  def __find_xvgs(self, *args, **kwargs):
+  def _find_gmxvg_files(self, *args, **kwargs):
+    """Finds files with XVG extension"""
+
+    _file_type = kwargs.get('file_type', args[0] if len(args) > 0 else '.xvg')
+
     _xvgs = []
     if hasattr(self, "pattern_dir"):
       self.pattern_dir = [self.pattern_dir] if isinstance(self.pattern_dir, str) else self.pattern_dir
       _directories = []
       for _dp in self.pattern_dir:
         _d = self.search_dirs(self.path_base, _dp)
         _directories.extend(_d)
       for _dir in _directories:
         for _px in self.pattern_xvg:
           _x = self.search_files(_dir, _px)
           _xvgs.extend(_x)
     else:
-      _xvgs = self.get_file_types(self.path_base, (".xvg"))
+      _xvgs = self.get_file_types(self.path_base, (_file_type))
 
     return _xvgs
 
-  def __rearrange_files(self):
+  def _rearrange_files(self):
     _bool_copy = getattr(self, "path_copy") and len(self.path_copy) > 2
     _bool_move = getattr(self, "path_move") and len(self.path_move) > 2
-    self.output_files.append(self.csv_filepath)
+
+    if not any([_bool_copy, _bool_move]):
+      self.log_debug('No action set to file rearrange.')
+      return
+
+    self.output_files.append(self.get_path(self.csv_filename))
     for _file in self.output_files:
       _rel_path = _file.split(self.path_base)[-1]
       _rel_path = _rel_path.strip("/")
 
-      self.copy(_file, f"{self.path_copy}/{_rel_path}") if _bool_copy and self.check_path(_file) else None
-      self.move(_file, f"{self.path_move}/{_rel_path}") if _bool_move and self.check_path(_file) else None
+      self.copy(_file, f"{self.path_copy}/{_rel_path}".replace('//', '/')) if _bool_copy and self.check_path(_file) else None
+      self.move(_file, f"{self.path_move}/{_rel_path}".replace('//', '/')) if _bool_move and self.check_path(_file) else None
 
-  @staticmethod
-  def process_text(_str):
-      _str = _str.strip()
-      _str = r'{}'.format(_str)
-      _str = REGEX.sub(r'\s{2,}', " ", _str)
-      _str = REGEX.sub(r'[\s-]{1,}', " ", _str)
-      _str = _str.replace("_", "-")
-      _str = REGEX.sub(r'\\S(\w+)\\N', "$^\\1$", _str)
-      _str = REGEX.sub(r'\\s(\w)\\N', "$_\\1$", _str)
-      return _str
-
-  @staticmethod
-  def process_attrib(_line):
-      _line = _line.strip("@").strip()
-      _matches = REGEX.findall('(.*)"([^"]*)"', _line)
-      _attribs = {}
-      if _line.startswith("legend"):
-          _ls = _line.split(" ", 1)
-          _attribs["plot_display_setting"] = GMXvg.process_text(_ls[-1])
-      elif len(_matches) > 0:
-        for _v in _matches:
-          _attribs[GMXvg.process_text(_v[0])] = GMXvg.process_text(_v[-1])
-      elif len(_line.split(" ", 1)) == 2:
-          _ls = _line.split(" ", 1)
-          _attribs[GMXvg.process_text(_ls[0])] = GMXvg.process_text(_ls[-1])
-      return _attribs
+  def process_text(self, _str):
+    _str = _str.strip()
+    _str = r'{}'.format(_str)
+    _str = self.REGEX.sub(r'\s{2,}', " ", _str)
+    _str = self.REGEX.sub(r'[\s-]{1,}', " ", _str)
+    _str = _str.replace("_", "-")
+    _str = self.REGEX.sub(r'\\S(\w+)\\N', "$^\\1$", _str)
+    _str = self.REGEX.sub(r'\\s(\w)\\N', "$_\\1$", _str)
+    return _str
+
+  def process_attrib(self, _line):
+    _line = _line.strip("@").strip()
+    _matches = self.REGEX.findall('(.*)"([^"]*)"', _line)
+    _attribs = {}
+    if _line.startswith("legend"):
+      _ls = _line.split(" ", 1)
+      _attribs["plot_display_setting"] = self.process_text(_ls[-1])
+    elif len(_matches) > 0:
+      for _v in _matches:
+        _attribs[self.process_text(_v[0])] = self.process_text(_v[-1])
+    elif len(_line.split(" ", 1)) == 2:
+      _ls = _line.split(" ", 1)
+      _attribs[self.process_text(_ls[0])] = self.process_text(_ls[-1])
+    return _attribs
 
   def __parse_xvg_table_attributes(self, _xvg_path):
     _xvg_content = self.read_text(_xvg_path)
 
     _data_rows = []
     _attributes = {}
     for _line in _xvg_content:
-        _line = _line.strip("\n").strip()
-        if _line.startswith("#"):
-          continue # As it is a comment
-        elif _line.startswith("@"):
-          _attr = self.process_attrib(_line)
-          if len(_attr.keys()) > 0 and isinstance(_attr, dict):
-            _attributes.update(_attr)
-        else:
-          _data_rows.append(_line.split())
+      _line = _line.strip("\n").strip()
+      if _line.startswith("#"):
+        continue # As it is a comment
+      elif _line.startswith("@"):
+        _attr = self.process_attrib(_line)
+        if len(_attr.keys()) > 0 and isinstance(_attr, dict):
+          _attributes.update(_attr)
+      else:
+        _data_rows.append(_line.split())
 
-    _df = PD.DataFrame(_data_rows)
-    _df = _df.apply(PD.to_numeric)
+    _df = self.DF(_data_rows)
+    _df = _df.apply(self.PD.to_numeric)
 
     _xaxis_label = _attributes.get('xaxis label')
     _yaxis_label = _attributes.get('yaxis label')
     _legends = [_attributes[_k] for _k in _attributes if "legend" in _k]
 
     if _df.shape[1] == 2 and len(_legends) < 1:
       _legends = [_yaxis_label]
@@ -173,75 +174,76 @@
     if len(_df.columns) == len(_legends):
       _df.columns = _legends
     else:
       self.log_info(f"Cannot change the column names in {_xvg_path}.\nCOLUMNS = {_df.columns}\nLEGENDS={_legends}", type="error")
     return (_df, _attributes)
 
   # Parse XVG File and Plot Graph
-  def __plot_xvg(self, *args, **kwargs):
+  def _plot_xvg(self, *args, **kwargs):
     _xvg = args[0] if len(args) > 0 else kwargs.get("xvg_path")
-    self.log_info(f"Plotting {_xvg}.")
+    _rel_fp = _xvg.replace(self.path_base, './').replace('//', '/')
+    self.log_info(f"Plotting {_rel_fp}.")
 
     _df, _attributes = self.__parse_xvg_table_attributes(_xvg)
 
     self.export_ext = [self.export_ext] if isinstance(self.export_ext, (str)) else self.export_ext
 
     _xaxis_label = _attributes.get('xaxis label')
     _yaxis_label = _attributes.get('yaxis label')
 
     _exp = getattr(self, "flag_export_plot", "yes")
 
     if _exp.lower().startswith("y"):
       _plot_title = self.process_text(self.filename(_xvg))
 
       if _attributes.get("subtitle"):
-          _subtitle = self.process_text(_attributes.get("subtitle"))
-          _plot_title = f"{_plot_title}\n{_subtitle}"
+        _subtitle = self.process_text(_attributes.get("subtitle"))
+        _plot_title = f"{_plot_title}\n{_subtitle}\n"
 
       _plot = _df.set_index(_df.columns[0]).plot(title=_plot_title, linewidth=1)
 
       for _pl in _plot.get_lines():
-          _pl_ydata = _pl.get_ydata()
-          _pl_ydata_mean = _pl_ydata.mean()
+        _pl_ydata = _pl.get_ydata()
+        _pl_ydata_mean = _pl_ydata.mean()
 
-          if self.flag_plot_mean.lower().startswith("y"):
-            _plot.axhline(y=_pl_ydata_mean, color=_pl.get_color(), linestyle="--", linewidth=1)
+        if self.flag_plot_mean.lower().startswith("y"):
+          _plot.axhline(y=_pl_ydata_mean, color=_pl.get_color(), linestyle="--", linewidth=1)
 
-          if self.flag_plot_std.lower().startswith("y"):
-            _pl_ydata_std = _pl_ydata.std()
-            _pl_ydata_upper = _pl_ydata_mean + _pl_ydata_std
-            _pl_ydata_lower = _pl_ydata_mean - _pl_ydata_std
-            _plot.axhline(y=_pl_ydata_upper, color=_pl.get_color(), linestyle="--", linewidth=0.5)
-            _plot.axhline(y=_pl_ydata_lower, color=_pl.get_color(), linestyle="--", linewidth=0.5)
+        if self.flag_plot_std.lower().startswith("y"):
+          _pl_ydata_std = _pl_ydata.std()
+          _pl_ydata_upper = _pl_ydata_mean + _pl_ydata_std
+          _pl_ydata_lower = _pl_ydata_mean - _pl_ydata_std
+          _plot.axhline(y=_pl_ydata_upper, color=_pl.get_color(), linestyle="--", linewidth=0.5)
+          _plot.axhline(y=_pl_ydata_lower, color=_pl.get_color(), linestyle="--", linewidth=0.5)
 
       _legend = _plot.legend(fontsize=8)
       _plot.set_xlabel(_xaxis_label)
       _plot.set_ylabel(_yaxis_label)
 
       for _ext in self.export_ext:
         _dpi = [self.dpi] if isinstance(self.dpi, (str, int)) else self.dpi
         for _d in _dpi:
           _out_file = self.change_ext(_xvg, f"{_d}dpi.{_ext}")
           self.output_files.append(_out_file)
           _figure = _plot.get_figure()
           _figure.savefig(_out_file, dpi=int(_d), bbox_inches='tight')
       _figure.clear()
-      PLOT.close(_figure)
+      self.PLOT.close(_figure)
 
     return _df
 
   def __merge_xvgs(self, *args, **kwargs):
-    self.__update_attr(**kwargs)
+    self.update_attributes(**kwargs)
 
     self.merge_patterns = [self.merge_patterns] if isinstance(self.merge_patterns, str) else self.merge_patterns
     _replacements = {}
     _replacements.update(self.replacements_gmx)
 
     for _r in self.replacements:
-      _k_v = REGEX.split('[:=]', _r)
+      _k_v = self.REGEX.split('[:=]', _r)
       if len(_k_v) > 1:
         _k = _k_v[0]
         _v = _k_v[-1]
         _replacements[_k.strip()] = _v.strip()
 
     if isinstance(self.path_base, (str)):
       for _mp in self.merge_patterns:
@@ -270,16 +272,15 @@
           _df_min = _df_min.rename(columns=_xvg_str_rep) #
 
           if _merged_df is None:
             _merged_df = _df_min
           else:
             _merged_df[_complex_name] = _df_min[_complex_name]
 
-
-        if isinstance(_merged_df, PD.DataFrame):
+        if isinstance(_merged_df, self.PD.DataFrame):
           _plot = _merged_df.set_index(_required_cols[0]).plot(title=_plot_name, lw=1)
           _legend = _plot.legend(fontsize=6)
           _plot.set_ylabel(self.process_text(_y_label))
           for _pl in _plot.get_lines():
             _pl_ydata = _pl.get_ydata()
             _pl_ydata_mean = _pl_ydata.mean()
 
@@ -298,46 +299,60 @@
           for _d in _dpi:
             _out_file = f"{self.path_base}/Combined-{_plot_name}.{_d}.jpg"
             self.output_files.append(_out_file)
             _figure = _plot.get_figure()
             _figure.savefig(_out_file, dpi=int(_d), bbox_inches='tight')
 
           _figure.clear()
-          PLOT.close(_figure)
-          PLOT.cla()
+          self.PLOT.close(_figure)
+          self.PLOT.cla()
         else:
           self.log_error("Some error occurred.")
     else:
-      self.log_error("Error with working dir.")
+      self.log_error(f"Error with working dir. path_base (-b) is not defined or current directory ({self.path_base}) does not contain xvg files.")
 
+  key__multidir = 'plot_multidir'
   def export_xvg(self, *args, **kwargs):
-    self.__update_attr(**kwargs)
+    self.update_attributes(self, kwargs)
     self.pattern_xvg = [self.pattern_xvg] if isinstance(self.pattern_xvg, str) else self.pattern_xvg
 
-    if isinstance(self.path_base, (str)):
+    if hasattr(self, self.key__multidir) and isinstance(getattr(self, self.key__multidir), (tuple, set, list)):
+      self.log_info(f'Plotting in multiple directories.')
+      for _enum, _bp in enumerate(getattr(self, self.key__multidir)):
+        self.log_info(f'>>> Processing {_enum+1}: {_bp}')
+        self.path_base = _bp
+        self.__merge_xvgs() if len(self.merge_patterns) > 0 else ""
+        self._plot_xvgs(self._find_gmxvg_files())
+        self._rearrange_files()
+    elif isinstance(self.path_base, (str)):
+      self.log_info(f'Plotting in single directory {self.path_base}.')
       self.__merge_xvgs() if len(self.merge_patterns) > 0 else ""
-      self.__plot_xvgs(self.__find_xvgs())
-      self.__rearrange_files()
+      self._plot_xvgs(self._find_gmxvg_files())
+      self._rearrange_files()
     else:
-      self.log_error("Error with working dir.")
+      self.log_error(f"There seems some error with working dir ({self.path_base}).")
 
-def xvgplot():
-  print(f"{GMXvg.__package__} v{GMXvg.__version__} (Build-{GMXvg.__subversion__})")
-  print("=" * 80)
-  print(f"Other available options are:")
-  print(f"csv_filename, csv_filepath, path_base, path_move, path_copy, pattern_xvg, merge_patterns,")
-  print(f"export_ext, dpi, flag_plot_mean, flag_plot_std, flag_export_csv, flag_export_plot, output_files")
-  print("=" * 80)
-  _plotter = GMXvg()
-  _parser = ARGUMENT.ArgumentParser(prog=GMXvg.name)
-
-  _parser.add_argument('-b', '--path_base', nargs = None, default = OS.getcwd(), help = 'Provide base directory. Default: %(default)s.')
-  _parser.add_argument('-e', '--export_ext', nargs = "*", default = ["jpg"], help = 'Output formats. Default: %(default)s.')
-  _parser.add_argument('-d', '--dpi', nargs = "*", default = [300], help = 'Output quality. Default: %(default)s.')
-
-  _reg_args, _unreg_args = _parser.parse_known_args()
-  _reg_args = vars(_reg_args)
-  _reg_args = {_k: _reg_args[_k] for _k in _reg_args.keys() if _reg_args[_k] is not None}
-
-  _params = _plotter.unregistered_arg_parser(_unreg_args)
-  _params.update(_reg_args)
-  _plotter.export_xvg(**_params)
+  def _clean_gmxvg_files(self):
+    """@precaution: Take backup before cleaning files as it may lose important data."""
+    _n_files = sum(self.delete_files(self._find_gmxvg_files(('jpg', 'csv', 'svg'))))
+    self.log_info(f'Deleted {_n_files} files.')
+
+  # Manage commandline operations
+  def _update_cli_args(self):
+    # key: (['arg_k1', 'arg_k2'], nargs, default, help, {})
+    _version_info = f"{self.name} {self.version} ({self.__build__})"
+    _cli_settings = {
+      "log_level": (['-log'], None, 'info', 'Provide logging level', {}),
+      "path_base": (['-b'], None, self.OS.getcwd(), 'Provide base directory(s) to run GMXvg.', {}),
+      "plot_multidir": (['-md'], "*", None, 'Plot multiple directories.', {}),
+      "export_ext": (['-e'], "*", ["jpg"], 'Output formats like svg, jpg, png, wmf, emf etc. One of multiple output extensions can be defined.', {}),
+      "dpi": (['-d'], "*", [300], 'Output quality(s). 72 for quick view and 600/1200 for publication.', {}),
+    }
+
+    _params = self.get_cli_args(_cli_settings, version=_version_info)
+
+    self.log_info("{}\n{}\n{}".format("=" * len(_version_info), _version_info, "=" * len(_version_info)))
+    self.update_attributes(self, _params)
+
+  def plot_cli(self, *args, **kwargs):
+    self._update_cli_args()
+    self.export_xvg(**kwargs)
```

### Comparing `GMXvg-0.4.6/pyproject.toml` & `gmxvg-0.4.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
   requires = ["setuptools>=68.0"]
   build-backend = "setuptools.build_meta"
 
 [project]
   name = "GMXvg"
   description = "A tool to plot GROMACS .xvg files."
-  version = "0.4.6"
+  version = "0.4.8"
   authors = [
     { name="Vishal Kumar Sahu", email="mail@vishalkumarsahu.in" },
   ]
   readme = "README.md"
   requires-python = ">=3.8"
   classifiers = [
     'Operating System :: OS Independent',
@@ -22,12 +22,12 @@
     'UtilityLib',
     'pandas',
     'matplotlib',
     'latex',
   ]
 
 [project.scripts]
-  gmxvg = "gmxvg:xvgplot"
+  gmxvg = "gmxvg:xvgplot_cli"
 
 [project.urls]
   Homepage = "https://github.com/TheBiomics/GMXvg"
   Issues = "https://github.com/TheBiomics/GMXvg/issues"
```

