# SportsJumpMotion

Dataset for the CVPR CVSports 2025 Workshop – contains detailed information about the dataset files and structure.

## Overview

The **SportsJumpMotion** dataset is designed for analyzing jump events in sports. It includes comprehensive data to support various computer vision tasks in sports analytics, such as:

- **Player Detection and Tracking:**  
  Tracklets of cropped bounding boxes extracted from original video frames.
- **Event Analysis:**  
  Detailed annotations of jump events and jersey number information at the tracklet level.
- **Binary Segmentation:**  
  Binary segmentation masks provided as `.png` files at original frame resolution.
- **Spatial Analysis:**  
  Original video frames and optional homography `.npy` files for advanced geometric transformations.
- **Jersey Number Legibility:**  
  JSON files that indicate jersey number visibility on a frame-by-frame basis.

## Dataset Structure

The dataset is organized into the following directories:

- **`data/`**:  
  Contains the raw data files (e.g., video clips, images).
  
- **`annotations/`**:  
  Contains metadata and annotations corresponding to the data files.
  
- **`scripts/`**:  
  Contains helper scripts for data processing and analysis.
  
- **`README.md`**:  
  This file, which provides detailed information about the dataset.

### Directory Details

- **`event_annotations/`**  
  Contains annotation files for jump events and jersey number annotations at the tracklet level. These files provide the temporal and spatial details of each jump event, along with corresponding jersey numbers.

- **`images/`**  
  Contains tracklets of cropped bounding boxes for players. Each sequence in this folder represents a series of images extracted from the original video frames, focusing on individual players.

- **`images_binary/`**  
  Contains binary segmentation `.png` files that match the original frame resolution. These masks are useful for extracting and analyzing player regions or bounding boxes in the images.

- **`json_legibility/`**  
  Contains JSON files that specify jersey number visibility for each frame within a tracklet. A value of `1` indicates that the jersey number is visible, while `0` indicates it is not.

- **`video/`**  
  Contains the original video frames or video clips from which the tracklets are derived. This folder may also include optional homography `.npy` files that can be used for mapping or transforming coordinates in spatial analysis tasks.

## Accessing the Dataset

The full dataset is hosted on OneDrive. You can download it using the following link:

[Download SportsJumpMotion Dataset](https://o365ust-my.sharepoint.com/:u:/g/personal/yinmay_office_ust_ac_kr/EVKOOgwTsuVOk2bYfvvNBr8BydMN45JV0ETHTFTJ8fToEA?e=vg1tPj)

**Steps to Access:**
1. Click the link above.
2. Download the entire dataset folder.
3. Extract the files locally.
4. Follow any additional instructions provided within the dataset package.

## Usage

- **Event Annotation Analysis:**  
  Use the files in the `event_annotations/` folder to identify jump events and view detailed jersey number annotations at the tracklet level.

- **Player Tracklets:**  
  The `images/` folder contains sequences of cropped bounding boxes for players, useful for detection and tracking tasks.

- **Binary Segmentation:**  
  The `images_binary/` folder provides binary segmentation masks that can assist in refining player localization and segmentation analyses.

- **Jersey Number Legibility:**  
  The JSON files in the `json_legibility/` folder indicate jersey number visibility (1 for visible, 0 for invisible) on a per-frame basis, which is valuable for evaluating jersey detection performance.

- **Video Reference and Homography:**  
  The `video/` folder offers original video frames/clips for reference. Additionally, optional homography `.npy` files support spatial transformations and advanced analysis.

## Citation

If you use this dataset in your research, please cite it as follows:

> **Author(s):** Your Name  
> **Title:** SportsJumpMotion Dataset for CVPR CVSports 2025 Workshop  
> **Conference:** CVPR CVSports Workshop  
> **Year:** 2025

## Contact

For further information or questions, please contact:

**Yin May Oo**  
Email: [yinmay@kist.re.kr]
