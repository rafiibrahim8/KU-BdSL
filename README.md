[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
[![DOI:10.17632/scpvm2nbkm.1](https://img.shields.io/badge/DOI-10.17632/scpvm2nbkm.1-45BF10.svg)](https://doi.org/10.17632/scpvm2nbkm.1)
# KU-BdSL
Khulna University Bengali Sign Language dataset

## Table of Contents

* [About the Dataset](#about-the-dataset)
    * [USLD](#usld)
    * [MSLD](#msld)
    * [AMSLD](#amsld)
* [About Class Names](#about-class-names)
* [Authors](#authors)
* [Citation](#citation)
* [License](#license)

## About the Dataset
The KU-BdSL refers to a Bengali sign language dataset, which includes three variants of the data. The variants are - 

1. Uni-scale Sign Language Dataset (USLD)
2. Multi-scale Sign Language Dataset (MSLD)
3. Annotated Multi-scale Sign Language Dataset (AMSLD)

The dataset consists of images representing single-hand gestures for BdSL alphabets. Several smartphones are taken into account to capture images from 33 participants (25 males and 8 females). Each version includes 30 classes that resemble the 39 consonants ('shoroborno') of Bengali alphabets. There is a total of 1,500 images in jpg format in each variant. The images are captured on flat surfaces at different times of the day to vary the brightness and contrast. **Class names are Unicode values corresponding to the Bengali alphabets for USLD and MSLD.**

### USLD
USLD has a unique size for all the images that is 512*512 pixels. The intended hand position is placed in the middle of the majority of cases in this dataset.

### MSLD
The raw images are stored in MSLD so that researchers can make changes to the dataset. The use of various smartphones yields us a wide variety of image sizes.

### AMSLD
AMSLD has multi-scale annotated data, which is suitable for tasks like localization and classification. From many annotation formats, the YOLO DarkNet annotation has been selected. Each image has an annotation text file containing five numbers separated by white space. The initial number is an integer, and the rest are floating numbers. The first number of the file indicates the class ID corresponding to the label of that image. Class IDs are mapped in a separate text file named `obj.names`. The second and third values are the beginning normalized coordinates, while the fourth and fifth define the bounding box's normalized width and height.

## About Class Names
Each class name is a Unicode value corresponding to the Bengali alphabets for USLD and MSLD. You can easily convert the class name to the Bengali alphabet using Python's [`chr()`](https://docs.python.org/3/library/functions.html#chr) method.

For example:

```python
>>> chr(2453)
'ক'
``` 

Here is the complete map for class names to Bengali characters -

|    Class Name   | Bengali Character(s)|
|:---------------:|:-------------------:|
|       2433      |          ঁ          |
|       2434      |          ং          |
|       2435      |          ঃ          |
|       2453      |          ক          |
|       2454      |          খ          |
|       2455      |          গ          |
|       2456      |          ঘ          |
|       2457      |          ঙ          |
|       2458      |          চ          |
|       2459      |          ছ          |
|    2460-2479    |         জ-য         |
|       2461      |          ঝ          |
|       2462      |          ঞ          |
|       2463      |          ট          |
|       2464      |          ঠ          |
|       2465      |          ড          |
|       2466      |          ঢ          |
|    2467-2472    |         ণ-ন         |
|    2468-2510    |         ত-ৎ         |
|       2469      |          থ          |
|       2470      |          দ          |
|       2471      |          ধ          |
|       2474      |          প          |
|       2475      |          ফ          |
|    2476-2477    |         ব-ভ         |
|       2478      |          ম          |
|  2480-2524-2525 |        র-ড়-ঢ়        |
|       2482      |          ল          |
|  2486-2488-2487 |        শ-স-ষ        |
|       2489      |          হ          |


## Authors
* [Abdullah Al Jaid Jim](https://orcid.org/0000-0002-1929-0939)
* [Ibrahim Rafi](https://orcid.org/0000-0002-4660-4999)
* [Md. Zahid Akon](https://orcid.org/0000-0002-4346-1339)
* [Abdullah-Al Nahid](https://orcid.org/0000-0003-2391-5767)

## Citation
If you want to use KU-BdSL, please cite it from [Mendeley Data](https://data.mendeley.com/datasets/scpvm2nbkm/1) as follows -
> Jaid Jim, Abdullah Al; Rafi, Ibrahim; Akon, Md. Zahid; Nahid, Abdullah-Al (2021), “KU-BdSL: Khulna University Bengali Sign Language dataset”, Mendeley Data, V1, doi: 10.17632/scpvm2nbkm.1

## License
<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.

