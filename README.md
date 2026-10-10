# mri-tumor-segmentation-analysis
An end-to-end medical image processing workflow implemented in Python. Working with an axial brain MRI scan containing three distinct hyperintense lesions, the project explores how classical computer vision techniques can be leveraged for non-invasive medical diagnosis. 

## Overview

The primary objective is the automated isolation and characterization of 3 distinct hyperintense tumor regions. 

Key implementation steps include:
* **Preprocessing & Binarization:** Converting the source image to binary format using both histogram-based manual thresholding and Otsu’s automated method.
* **Connected-Component Labeling:** Isolating candidate regions and displaying individual and combined segmented masks.
* **Feature Extraction & Filtering:** Analyzing regional geometric properties (e.g., area, eccentricity/shape metrics) to isolate tumors and calculating individual tumor areas.
* **Visualization & Annotation:** Delineating tumor boundaries with red contours and labeling detected lesions with visual annotations.
* **Mathematical Morphology:** Applying structuring elements for dilation, erosion, opening, closing, and internal/external boundary extraction.


## Quantitative Findings

By filtering connected components based on pixel area and shape descriptors, the three lesions were successfully isolated from the surrounding skull and cerebral tissue
