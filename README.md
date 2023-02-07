Here's a condensed version of your content:

---

# License Plate Detection Project

## Overview

This project, undertaken as a Final Year Project for a Bachelor's degree in Electronics Engineering, is based on Adrian Rosebrock's PyImageSearch post titled "OpenCV: Automatic License/Number Plate Recognition (ANPR) with Python." It has been adapted to detect Malaysian license plates, which typically have white text on a black background.

## Objectives

The primary goals of this project are as follows:
- Automatic detection of Malaysian license plates and overseas license plates
- Comparison of three license plate detection methods: Scharr operator, Canny edge detector, and an edge-less approach

## Prerequisites

The project utilizes the following libraries and versions:
- Python v3.8.6
- OpenCV v4.4.0.46
- imutils v0.5.3
- scikit-image v0.17.2
- pytesseract v0.3.6
- Tesseract-OCR v5.0.0 (alpha)

Please note that Tesseract-OCR should be installed using the Windows installer and not via pip.

## How It Works

1. The project consists of two modules: the driver module (`anprdriver.py`) and the class module (`anprclass.py`). The driver module is executed by the user with specific arguments, while the class module contains the license plate detection algorithms and related functions.

2. The driver module is run from a terminal using Python, and various arguments can be appended, including the path to the input image directory, enabling debug mode, selecting the algorithm, and more.

3. The script processes the images, performs license plate detection using the specified algorithm, and saves the results in separate folders based on the chosen algorithm and plate type (Malaysian or overseas).

## Typical Usage

To run the script, use the following command:

```
python anprdriver.py -i /path/to/images/
```

While only the `-i` argument (input directory) is required, ensure that you choose the appropriate algorithm (`-a`) and morphological operation (`-m`) as needed.

Sample images of license plates are provided in the `malaysian` and `overseas` folders, and the results are saved in corresponding folders based on the selected algorithm.

---