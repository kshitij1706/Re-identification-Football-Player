# Re-identification-Football-Player
# 🎯 Player Re-Identification in Sports Footage (Option 2)

This project implements a player tracking and re-identification pipeline using a custom YOLOv11 model and Deep SORT tracking. The goal is to assign consistent IDs to players throughout a 15-second football clip, even when they leave and re-enter the frame.

---

## 📁 Files

- `main.py` – Main Python script to run detection and tracking.
- `liatai_yolo_model.pt` – Pretrained YOLOv11 model (provided by Liat.ai).
- `15sec_input_720p.mp4` – Input video.
- `output_tracked.avi` – Output video with player IDs.
- `test_frame_output.jpg` – Snapshot for bounding box verification.
- `report.md` – Methodology and explanation.

---

## 🛠️ Setup Instructions

### 1. Create a virtual environment (optional but recommended)

```bash
python -m venv player_reid_env
player_reid_env\Scripts\activate       # On Windows
# or
source player_reid_env/bin/activate    # On macOS/Linux
Install dependencies
pip install ultralytics opencv-python deep_sort_realtime numpy
