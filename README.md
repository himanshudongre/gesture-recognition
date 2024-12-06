# CSCA 5642 Introduction to Deep Learning : Gesture Recognition Final Project

## Problem Statement

Imagine you are working as a Machine Learning (ML) Engineer at a home electronics company that manufactures state-of-the-art smart televisions. The goal is to develop a feature for smart TVs to recognize five different gestures performed by the user, allowing control of the TV without using a remote. 

Each gesture corresponds to a specific command:
- **Thumbs up:** Increase the volume
- **Thumbs down:** Decrease the volume
- **Left swipe:** Jump backwards 10 seconds
- **Right swipe:** Jump forward 10 seconds
- **Stop:** Pause the movie

The gestures are continuously monitored by the webcam mounted on the TV, with each video consisting of a sequence of 30 frames (or images).


## Dataset Description

The dataset contains a total of **773 videos**, categorized into one of five classes:
- **Training Set:** 663 videos
- **Validation Set:** 100 videos

### Folder Structure
The data is provided in a compressed ZIP file containing:
1. Two main folders: `train` and `val`.
2. Each folder (`train` and `val`) is divided into subfolders where:
   - Each subfolder represents a single video.
   - The subfolder contains **30 frames (images)** corresponding to that video.

### Frame Dimensions
- All images within a video subfolder share the same dimensions.
- Different videos may have different dimensions: either **360x360** or **120x160** depending on the recording webcam.

### CSV Files
- Each main folder (`train` and `val`) includes a corresponding CSV file (`train.csv` and `val.csv`).
- Each row in these CSV files provides the following information:
  1. The **name of the subfolder** containing the video frames.
  2. The **gesture name** (e.g., thumbs up, thumbs down).
  3. The **numeric label** of the video (0-4) corresponding to the gesture class.

This dataset is available at: https://www.kaggle.com/datasets/abhishek14398/gesture-recognition-dataset
