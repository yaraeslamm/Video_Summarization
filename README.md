

## ✅ README – Dynamic Video Summarization using Object Detection & Tracking

```markdown
# Dynamic Video Summarization using Object Detection & Tracking

**Author:** Yara Eslam  
**Course:** Advanced Video Processing  

---

## 🎯 Objective

This project summarizes object movement in a video by:

- Detecting and tracking moving objects
- Timestamping their appearance
- Placing them on a clean reference frame to visualize all detected activity

---

## 🧠 Methodology

- **Background Modeling**:  
  Computed the median frame of the video to serve as a static reference.

- **Object Detection**:  
  Detected motion via background subtraction and morphological processing.

- **Tracking**:  
  Used a Euclidean distance tracker to assign consistent IDs to objects.

- **Summarization**:  
  Cropped detected objects, labeled them with timestamps, and overlaid them on a reference image.

---

## 🗂️ Output

- `output_frames/`: Frames with bounding boxes and object timestamps  
- `reference_frames/`: A canvas showing all extracted objects with labels  
- `reference_frame_with_objects.png`: Final reference image with all detected objects  

---

## ▶️ How to Run

This project was built in Google Colab.

1. Open the notebook in [Google Colab](https://colab.research.google.com).  
2. Upload your `.avi` video to your Google Drive.
3. **Before running, update the paths as needed:**

```python
VIDEO_PATH = '/content/drive/My Drive/your_video.avi'
OUTPUT_DIR = '/content/drive/My Drive/AVP/Projects'

4. Run all cells. Output images will be saved inside OUTPUT_DIR

##  Requirements

-  Python 3
-  OpenCV
-  NumPy
