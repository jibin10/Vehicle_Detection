# Vehicle Detection and Counting (OpenCV)

This project is a computer vision exercise using **OpenCV** to work with traffic videos.

It includes two notebook tasks:

- **Task 1:** Detect and track moving cars in a traffic camera video.
- **Task 2:** Count cars and estimate how many vehicles move toward the city center using motion direction (optical flow).

The work is provided as Jupyter notebooks and can be run step-by-step.

---

## What’s inside

### Notebooks
- `Task_1_Detect_and_track_vehicles.ipynb`
  - Detects moving cars using **background subtraction (MOG2)**
  - Uses image processing steps (grayscale, blur, threshold, dilation)
  - Finds vehicle shapes using contours and draws bounding boxes

- `Task_2_Count_vehicles.ipynb`
  - Counts cars using detections from background subtraction
  - Tracks objects across frames to avoid counting the same car again
  - Uses **dense optical flow (Farneback)** to understand motion direction
  - Estimates cars moving toward the city center based on the dominant motion angle

---

## Input files

The notebooks expect traffic videos to be available in .mp4 format locally.

**Note:** Place the video file(s) in the same folder as the notebook(s), or update the file path inside the notebook.

---

## How to run

1. Open the notebooks in Jupyter Notebook / JupyterLab (or Google Colab).
2. Run the cells from top to bottom.

The notebooks include `pip install` commands for required packages.

---

## Requirements

- Python 3
- Jupyter Notebook / JupyterLab
- Main libraries used:
  - `opencv-python`
  - `numpy`
  - `scipy` (used for simple statistics in Task 2)