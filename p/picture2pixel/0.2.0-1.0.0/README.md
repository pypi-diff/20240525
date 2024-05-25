# Comparing `tmp/picture2pixel-0.2.0.tar.gz` & `tmp/picture2pixel-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picture2pixel-0.2.0.tar", last modified: Fri May 17 19:54:52 2024, max compression
+gzip compressed data, was "picture2pixel-1.0.0.tar", last modified: Sat May 25 10:34:13 2024, max compression
```

## Comparing `picture2pixel-0.2.0.tar` & `picture2pixel-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 19:54:52.937959 picture2pixel-0.2.0/
--rw-rw-rw-   0        0        0     4293 2024-05-17 19:54:52.935958 picture2pixel-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3506 2024-05-17 19:50:56.000000 picture2pixel-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 19:54:52.916959 picture2pixel-0.2.0/picture2pixel/
--rw-rw-rw-   0        0        0      132 2024-05-16 16:35:45.000000 picture2pixel-0.2.0/picture2pixel/__init__.py
--rw-rw-rw-   0        0        0     4731 2024-05-17 19:23:44.000000 picture2pixel-0.2.0/picture2pixel/convert2picture.py
--rw-rw-rw-   0        0        0     1825 2024-05-17 18:18:07.000000 picture2pixel-0.2.0/picture2pixel/convert2pixel.py
--rw-rw-rw-   0        0        0     2095 2024-05-16 16:36:00.000000 picture2pixel-0.2.0/picture2pixel/image_processing.py
-drwxrwxrwx   0        0        0        0 2024-05-17 19:54:52.932959 picture2pixel-0.2.0/picture2pixel/tests/
--rw-rw-rw-   0        0        0        0 2024-05-17 18:26:32.000000 picture2pixel-0.2.0/picture2pixel/tests/__init__.py
--rw-rw-rw-   0        0        0     1409 2024-05-17 19:15:22.000000 picture2pixel-0.2.0/picture2pixel/tests/test_picture2pixel.py
--rw-rw-rw-   0        0        0     2247 2024-05-17 19:15:39.000000 picture2pixel-0.2.0/picture2pixel/tests/test_pixel2picture.py
--rw-rw-rw-   0        0        0     2851 2024-05-16 16:39:07.000000 picture2pixel-0.2.0/picture2pixel/verilog_generator.py
-drwxrwxrwx   0        0        0        0 2024-05-17 19:54:52.934958 picture2pixel-0.2.0/picture2pixel.egg-info/
--rw-rw-rw-   0        0        0     4293 2024-05-17 19:54:52.000000 picture2pixel-0.2.0/picture2pixel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      477 2024-05-17 19:54:52.000000 picture2pixel-0.2.0/picture2pixel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 19:54:52.000000 picture2pixel-0.2.0/picture2pixel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-05-17 19:54:52.000000 picture2pixel-0.2.0/picture2pixel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-17 19:54:52.000000 picture2pixel-0.2.0/picture2pixel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-17 19:54:52.937959 picture2pixel-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1066 2024-05-17 19:54:47.000000 picture2pixel-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 10:34:13.795548 picture2pixel-1.0.0/
+-rw-rw-rw-   0        0        0     1080 2024-05-25 09:28:46.000000 picture2pixel-1.0.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     5644 2024-05-25 10:34:13.793548 picture2pixel-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4844 2024-05-25 10:33:13.000000 picture2pixel-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-25 10:34:13.777548 picture2pixel-1.0.0/picture2pixel/
+-rw-rw-rw-   0        0        0      132 2024-05-16 16:35:45.000000 picture2pixel-1.0.0/picture2pixel/__init__.py
+-rw-rw-rw-   0        0        0     4739 2024-05-25 09:30:19.000000 picture2pixel-1.0.0/picture2pixel/convert2picture.py
+-rw-rw-rw-   0        0        0     1825 2024-05-17 18:18:07.000000 picture2pixel-1.0.0/picture2pixel/convert2pixel.py
+-rw-rw-rw-   0        0        0     2095 2024-05-16 16:36:00.000000 picture2pixel-1.0.0/picture2pixel/image_processing.py
+drwxrwxrwx   0        0        0        0 2024-05-25 10:34:13.789546 picture2pixel-1.0.0/picture2pixel/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-17 18:26:32.000000 picture2pixel-1.0.0/picture2pixel/tests/__init__.py
+-rw-rw-rw-   0        0        0     1409 2024-05-17 19:15:22.000000 picture2pixel-1.0.0/picture2pixel/tests/test_picture2pixel.py
+-rw-rw-rw-   0        0        0     2247 2024-05-17 19:15:39.000000 picture2pixel-1.0.0/picture2pixel/tests/test_pixel2picture.py
+-rw-rw-rw-   0        0        0     2851 2024-05-16 16:39:07.000000 picture2pixel-1.0.0/picture2pixel/verilog_generator.py
+drwxrwxrwx   0        0        0        0 2024-05-25 10:34:13.791549 picture2pixel-1.0.0/picture2pixel.egg-info/
+-rw-rw-rw-   0        0        0     5644 2024-05-25 10:34:13.000000 picture2pixel-1.0.0/picture2pixel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      489 2024-05-25 10:34:13.000000 picture2pixel-1.0.0/picture2pixel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 10:34:13.000000 picture2pixel-1.0.0/picture2pixel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-25 10:34:13.000000 picture2pixel-1.0.0/picture2pixel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-25 10:34:13.000000 picture2pixel-1.0.0/picture2pixel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-25 10:34:13.795548 picture2pixel-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1050 2024-05-25 10:33:48.000000 picture2pixel-1.0.0/setup.py
```

### Comparing `picture2pixel-0.2.0/PKG-INFO` & `picture2pixel-1.0.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,19 @@
-Metadata-Version: 2.1
-Name: picture2pixel
-Version: 0.2.0
-Summary: A package for processing images and generating Verilog code for FPGA
-Home-page: https://www.comp.nus.edu.sg/~guoyi/project/picture2pixel/
-Author: Chen Guoyi
-Author-email: guoyi@comp.nus.edu.sg
-License: MIT
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Requires-Dist: numpy
-Requires-Dist: matplotlib
-Requires-Dist: imageio
-Requires-Dist: Pillow
-
-# Picture2Pixel
-
-By: Chen Guoyi; Fang Sihan. National University of Singapore.
+<center><img src="https://www.comp.nus.edu.sg/~guoyi/project/picture2pixel/img/title.png" width="100%"></center>
 
 **Picture2Pixel** is an open-source Python library designed to transform images into pixel art that can be displayed on FPGA-driven OLED screens. By employing advanced computer graphics techniques, this library preprocesses images to minimize distortion during the pixelation process. The resulting artwork is expressed as combinations of predicate logic in Verilog language, ensuring compatibility with FPGA technology. This optimization not only enhances display efficiency on OLED screens but also reduces energy consumption, making it ideal for developers looking to integrate low-power, high-efficiency visual displays into their hardware projects.
 
-**For more information about this project, please nevigate to project homepage: https://www.comp.nus.edu.sg/~guoyi/project/picture2pixel/**
+**Picture2Pixel** can also convert both single images and batches of images (including GIFs) into formats suitable for FPGA OLED displays. Please view more magnificent demos on our website: [Picture2Pixel.org](https://www.comp.nus.edu.sg/~guoyi/project/picture2pixel/)
 
-## Table of Contents
-
-- [Installation](#installation)
-- [Usage](#usage)
-  - [Convert Image to Pixel Data](#convert-image-to-pixel-data)
-  - [Convert Pixel Data to Image](#convert-pixel-data-to-image)
-- [Project Structure](#project-structure)
-- [License](#license)
+## Project Wiki (MUST READ!)
+We have created a comprehensive [Wiki](https://github.com/gu0y1/picture2pixel/wiki) for the Picture2Pixel project, which includes development documentation, tutorials, and examples to help developers deploy, use, and further develop our project.
+- **[Tutorial](https://github.com/gu0y1/picture2pixel/wiki/Tutorial)**: Detailed Python and Verilog tutorials, including examples, to help you achieve stunning FPGA display effects similar to those on our [official website](https://www.comp.nus.edu.sg/~guoyi/project/picture2pixel/).
+- **Technical Standards**: Detailed development documentation, including function descriptions and technical standards to facilitate further development of our Python Library.
+  - [Python Library Technical Standards](https://github.com/gu0y1/picture2pixel/wiki/Python-Library-Technical-Standard).
+  - [Verilog Technical Standards](https://github.com/gu0y1/picture2pixel/wiki/Verilog-Techinal-Standard)
 
 ## Installation
 
 Install the `picture2pixel` package using pip:
 
 ```bash
 pip install picture2pixel
@@ -54,32 +28,32 @@
 ```bash
 python -m picture2pixel.convert2pixel <image_url> <width> <height> <svd_r> <output_dir>
 ```
 
 Example:
 
 ```bash
-python -m picture2pixel.convert2pixel https://www.comp.nus.edu.sg/~guoyi/project/picture2pixel/default.png 96 64 20 output_directory
+python -m picture2pixel.convert2pixel https://www.comp.nus.edu.sg/~guoyi/project/picture2pixel/tests/default.png 96 64 20 output_directory
 ```
 
 ### Convert Pixel Data to Image
 
-Convert pixel data from a `.p2p` file back into an image:
+This function is for Convert pixel data from a `.p2p` file back into an image:
 
 ```bash
 python -m picture2pixel.convert2picture <p2p_file> <width> <height> <output_dir>
 ```
 
 Example:
 
 ```bash
-python -m picture2pixel.convert2picture https://www.comp.nus.edu.sg/~guoyi/project/picture2pixel/default.p2p 96 64 output_directory
+python -m picture2pixel.convert2picture https://www.comp.nus.edu.sg/~guoyi/project/picture2pixel/tests/default.p2p 96 64 output_directory
 ```
 
-## Project Structure
+## Library Structure
 
 ```plaintext
 picture2pixel/
 ├── __init__.py
 ├── convert2pixel.py
 ├── convert2picture.py
 ├── image_processing.py
@@ -90,16 +64,26 @@
 │   ├── test_pixel2picture.py
 │   ├── test_integrated.py
 README.md
 requirements.txt
 setup.py
 ```
 
-## License
+## MIT License
 
 Copyright (c) <2024> <copyright Chen Guoyi, Fang Sihan>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+
+------------
+
+**Picture2Pixel** Python Library is developed and maintained, also copyrighted by:
+- Chen [Guoyi@comp.nus.edu.sg](mailto:guoyi@comp.nus.edu.sg)
+- Fang [Sihan@comp.nus.edu.sg](mailto:sihan@comp.nus.edu.sg)
+
+**Picture2Pixel** Python Library is released to [PyPI](https://pypi.org/project/picture2pixel/).
+
+THIS PROJECT IS SPONSORED BY THE DEPARTMENT OF ELECTRICAL AND COMPUTER ENGINEERING, NATIONAL UNIVERSITY OF SINGAPORE.
```

### Comparing `picture2pixel-0.2.0/picture2pixel/convert2picture.py` & `picture2pixel-1.0.0/picture2pixel/convert2picture.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     base_filename = os.path.splitext(os.path.basename(p2p_file))[0]
     output_path = os.path.join(output_dir, f"{base_filename}.png")
     
     image_array, unfound_pixels = load_p2p_file(p2p_file, width, height)
     save_image(image_array, output_path)
     
     if unfound_pixels:
-        print("\n[  !  ] Uncolored pixels found at:")
+        print("\n[  !  ] Uncolored (black) pixels found at:")
         for pixel in unfound_pixels:
             print(f"({pixel[0]}, {pixel[1]})")
     else:
         print("[ OK! ] All pixels colored successfully.")
     
     # Clean up the downloaded file if it was used
     if p2p_file == 'downloaded.p2p':
```

### Comparing `picture2pixel-0.2.0/picture2pixel/convert2pixel.py` & `picture2pixel-1.0.0/picture2pixel/convert2pixel.py`

 * *Files identical despite different names*

### Comparing `picture2pixel-0.2.0/picture2pixel/image_processing.py` & `picture2pixel-1.0.0/picture2pixel/image_processing.py`

 * *Files identical despite different names*

### Comparing `picture2pixel-0.2.0/picture2pixel/tests/test_picture2pixel.py` & `picture2pixel-1.0.0/picture2pixel/tests/test_picture2pixel.py`

 * *Files identical despite different names*

### Comparing `picture2pixel-0.2.0/picture2pixel/tests/test_pixel2picture.py` & `picture2pixel-1.0.0/picture2pixel/tests/test_pixel2picture.py`

 * *Files identical despite different names*

### Comparing `picture2pixel-0.2.0/picture2pixel/verilog_generator.py` & `picture2pixel-1.0.0/picture2pixel/verilog_generator.py`

 * *Files identical despite different names*

### Comparing `picture2pixel-0.2.0/setup.py` & `picture2pixel-1.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='picture2pixel',
-    version='0.2.0',
-    description='A package for processing images and generating Verilog code for FPGA',
+    version='1.0.0',
+    description='A Python library for converting images into FPGA-displayable pixel art.',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url='https://www.comp.nus.edu.sg/~guoyi/project/picture2pixel/',
+    url='https://github.com/gu0y1/picture2pixel',
     author='Chen Guoyi',
     author_email='guoyi@comp.nus.edu.sg',
     license='MIT',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'matplotlib',
```

