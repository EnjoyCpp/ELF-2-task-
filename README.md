# Video Frame Processing and Clustering

## Description

This project provides a set of functions for processing video frames, assessing their quality based on blur and motion scores, and performing tasks such as identifying bad frames, clustering frames, and visualizing the results. This code extracts frames from video files, analyzes their quality, marks bad frames, clusters frames based on quality scores, and stores the results in organized folders. It also visualizes the clustering results using a scatter plot of blur and motion scores.

### Features

- **Frame Extraction:** Extracts frames from given video files.
- **Bad Frame Identification:** Marks frames with high blur or motion scores as "bad" frames and saves them.
- **Frame Clustering:** Uses KMeans clustering to categorize frames based on their quality scores (blur and motion).
- **Visualization:** Visualizes the frame clustering with a scatter plot of blur and motion scores.
- **Results Output:** Saves results in text files, detailing frame IDs and their associated blur and motion scores.

---

## Installation

To use this code, you need to install the following dependencies:

- **OpenCV**: For frame extraction and manipulation.
- **NumPy**: For handling arrays and numerical operations.
- **Matplotlib**: For visualizing the clustering results.
- **Scikit-learn**: For KMeans clustering.
- **TQDM**: For progress bars.

You can install all the required packages by running the following command:

```bash
pip install opencv-python numpy matplotlib scikit-learn tqdm
```

Usage
1. Upload the Video

The code uses the Google Colab interface for uploading video files. After running the code, it will prompt you to upload one or more video files.

2. Run Frame Extraction and Processing

Once the video is uploaded, the extract_frames function will:
    Extract frames from the video.
    Analyze the quality of each frame (blur and motion).
    Identify "bad frames" and save them in a specified folder.
    Cluster the frames based on their quality scores and save the clustered frames in separate folders.

3. View Results

    A CSV file will be generated with the results of the analysis for the bad frames.
    A directory will be created with clustered frames based on their quality.
    The code will also generate a scatter plot visualizing the clustering results based on the blur and motion scores.



