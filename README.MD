# Wrong_Way_Vehicle_Detection_with_Automatic_Number_Plate_Recognition
This project is an intelligent traffic monitoring system that detects vehicles moving in the wrong direction on roadways and captures their license plate numbers automatically using ANPR (Automatic Number Plate Recognition).

# Wrong Way Vehicle Detection Project

## Overview
This project uses YOLO object detection and SORT tracking to identify vehicles moving in the wrong direction in a video.

## Structure
- `src/main.py`: Main script to run detection and tracking.
- `data/car.mp4`: Input video (add your own video here).
- `sort.py`: SORT tracking code, downloaded automatically.
- `results/tracked_output.mp4`: Output video with tracking.
- `results/wrong_way_snaps/`: Snapshots of detected wrong-way vehicles.

## Setup

1. **Clone the repository and enter the directory:**
   ```sh
   git clone https://github.com/<yourusername>/<yourrepo>.git
   cd <yourrepo>
   ```

2. **Install dependencies:**
   ```sh
   pip install -r requirements.txt
   ```

3. **Add your input video:**
   Place your video file in the `data/` directory and name it `car.mp4`.

4. **Download YOLOv11 weights (`yolo11n.pt`):**
   Place the weights file in your project root directory.

## Usage

Run the main script:
```sh
python src/main.py
```

- Output video and snapshots will appear in the `results/` folder.

## Notes
- You can change input/output paths by editing `src/main.py`.
- The script automatically downloads and prepares `sort.py`.

## Requirements
See `requirements.txt` for dependencies.
