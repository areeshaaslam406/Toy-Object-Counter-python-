
# 🧸 Toy Counter — Object Detection & Counting

A computer vision project that detects and counts toys in images or video streams using **background subtraction**, **contour detection**, and **thresholding**.  
Designed to work with offline images, live webcam feeds, or pre-recorded videos.

---

## 📌 Features
- Detect toys based on **movement** or **color/shape contrast**.
- Count multiple toys simultaneously.
- Works with both **static images** and **video streams**.
- Adjustable detection parameters (threshold, contour area, etc.).
- Real-time display with bounding boxes and count overlays.
- Simple, modular code structure for easy customization.

---

## 🛠️ Tech Stack
- **Language**: Python 3.x
- **Libraries**:
  - [OpenCV](https://opencv.org/) — Image processing & computer vision
  - [NumPy](https://numpy.org/) — Numerical operations
  - [Matplotlib](https://matplotlib.org/) — Visualization
  - [Pandas](https://pandas.pydata.org/) — Data logging & analysis

## 🚀 Getting Started

### 1️⃣ Clone Repository

git clone https://github.com/yourusername/toy-counter.git
cd toy-counter


### 2️⃣ Install Dependencies


pip install -r requirements.txt


### 3️⃣ Run with Sample Image


python src/toy_counter.py --input data/sample_toys.jpg


### 4️⃣ Run with Video or Webcam


# For video file
python src/toy_counter.py --input data/toy_video.mp4

# For webcam
python src/toy_counter.py --webcam 0



## ⚙️ Configuration

Edit `config.py` to adjust:

* `MIN_CONTOUR_AREA` → Minimum object size to detect
* `BG_DIFF_THRESH` → Background subtraction sensitivity
* `DISPLAY_RESULTS` → Show output window (True/False)


## 🧪 How It Works

1. **Background Subtraction** — Removes static elements, keeping only moving/foreground objects.
2. **Thresholding & Morphology** — Cleans up noise and enhances toy shapes.
3. **Contour Detection** — Finds object outlines and measures size.
4. **Counting** — Counts objects above the area threshold.

---

## 📜 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

