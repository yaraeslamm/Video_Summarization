

## Dynamic Video Summarization using Object Detection & Tracking


---

## Objective

This project summarizes object movement in a video by:

- Detecting and tracking moving objects
- Timestamping their appearance
- Placing them on a clean reference frame to visualize all detected activity

---

## Methodology

- **Background Modeling**:  
  Computed the median frame of the video to serve as a static reference.

- **Object Detection**:  
  Detected motion via background subtraction and morphological processing.

- **Tracking**:  
  Used a Euclidean distance tracker to assign consistent IDs to objects.

- **Summarization**:  
  Cropped detected objects, labeled them with timestamps, and overlaid them on a reference image.

---

## Output

- `frames/`: Frames with bounding boxes and object timestamps  
- `reference_frame`: Final reference image with all detected objects  

---

## How to Run

This project was built in Google Colab.

1. Open the notebook in [Google Colab](https://colab.research.google.com/drive/10g3m26OQoeoPdO2K7TURkKhgeQqhqqv9) and take a copy in your Drive  
2. Upload your `.avi` video to your Google Drive.
3. **Before running, update the paths as needed:**

```bash
VIDEO_PATH = '/content/drive/My Drive/your_video.avi'
OUTPUT_DIR = '/content/drive/My Drive/your_path'
```
4. Run the cell. Output images will be saved inside OUTPUT_DIR

##  Requirements

-  Python 3
-  OpenCV
-  NumPy
