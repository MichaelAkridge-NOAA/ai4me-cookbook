# FAQ

## [Glossary](https://www.ultralytics.com/glossary)

## Object Detection FAQ

### General Object Detection

**Q: What is object detection?**  
A: computer vision task that identifies and locates objects in images using bounding boxes.

**Q: What are common challenges?**  
A: Small/occluded objects, class imbalance, limited data, and computational cost for training/real-time detection.

**Q: How do I select a model?**  
A: Start with YOLO for speed and ease of use. Pretrained models help with small datasets and startup.

**Q: How do I measure performance?**  
A: Use mAP (mean Average Precision) and IoU (Intersection over Union). Higher mAP = better detection.

**Q: What hardware is needed?**  
A: GPUs (NVIDIA, 8GB+ VRAM) speed up training. CPUs work but are slower. Use cloud if needed.

---

### AI4ME Cookbook-Specific FAQs

**Q: How do I set things up?**  
A: Clone the repo, install dependencies (`pip install -r requirements.txt`), and follow the notebooks.

**Q: Common errors and fixes?**  
A: Missing modules (`pip install` needed), incorrect file paths, or insufficient GPU memory.

**Q: Can I use my own dataset?**  
A: Yes, format it properly (e.g., COCO/YOLO format) and update the training scripts accordingly.

---

### Python for R Users FAQs

**Q: How does Python compare to R for ML?**  
A: Python is better for deep learning and production, while R excels at statistics and visualization.

**Q: What Python libraries are used for detection?**  
A: TensorFlow, PyTorch, Ultralytics YOLO, OpenCV for preprocessing, and several others.

**Q: How do pandas and dplyr compare?**  
A: Pandas is Python’s equivalent of dplyr, using methods like `.groupby()`, `.apply()`, and `.filter()`.

**Q: How does object detection code differ?**  
A: in Python, `YOLO('yolov8n.pt')` from `ultralytics` does the same.

**Q: How do I debug Python if I’m used to R?**  
A: Read error tracebacks, use `print()`, check 0-based indexing, and verify library installations.
