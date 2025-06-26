# player-reidentification-assignment
Player Re-identification using YOLOv8 + SORT + ReID
# 🏃‍♂️ Player Re-Identification in Sports Footage 🎥

This project performs **player re-identification** in sports videos. It detects players using YOLOv8, tracks them using SORT, and identifies each unique player using features extracted from EfficientNet. The final output video highlights each player with a consistent ID across frames.

---
## 📦 Model Checkpoint

The trained YOLOv8 model file used in this project (`best.pt`) was provided by the company.

🔗 **[Download best.pt (Google Drive)](https://drive.google.com/file/d/1cFxwi0pgxcb0x6MeKbm01O5jI0_ys4SP/view?usp=sharing)**

---

## 🎬 Test Video

This video was used to test the Re-Identification pipeline.

🔗 **[Download test video (Google Drive)](https://drive.google.com/file/d/1SuNCwp3C3COCqJqbcmK8HNvV2bAhppee/view?usp=sharing)**


---

## 🧠 Workflow Summary

### ✅ Step-by-step pipeline:

1. **Player Detection** using YOLOv8 `best.pt`  
2. **Tracking** using SORT tracker  
3. **Player Cropping** from video frames  
4. **Feature Extraction** using EfficientNet-B0  
5. **Player Re-Identification** by clustering similar features  
6. **Final Output Video** with consistent player IDs

---

## ⚙️ Tools & Libraries Used

| Tool        | Purpose                             |
|-------------|-------------------------------------|
| YOLOv8      | Player detection                    |
| SORT        | Object tracking                     |
| EfficientNet-B0 | Feature extraction             |
| OpenCV      | Video processing                    |
| PyTorch     | Deep learning & model handling      |
| NumPy       | Feature vector computation          |
| LaTeX       | Documentation (explanation.pdf)     |

---

## 📽️ Output Video

- Filename: `final_output.avi`
- Contains tracked and re-identified players.
- Each unique player is assigned a unique ID throughout the video.

> ✅ Successfully detects **5891 player crops**  
> ✅ Groups into **1256 unique players** using feature similarity

---

## 📊 Results

- 🎯 Total frames processed: `460`
- 🧠 Player crops generated: `5891`
- 🔢 Unique players identified: `1256`
- ⏱️ Processing done in Google Colab environment

---

## 🚀 How to Run (Colab)

1. Upload `best.pt` and your input video to Colab
2. Run the `player_reidentification_assignment.py` script step-by-step
3. Extracted crops, features, groupings and final video will be auto-generated

---

## 📘 Explanation PDF

The LaTeX-generated `explanation.pdf` contains:

- Model pipeline explanation
- Code walkthrough
- Sample outputs and screenshots
- Summary of each module

---

## 🙋‍♀️ Developed By
 
Developed with 💻 and ❤️ by **[SAKSHI TIWARI]**.

---

## 📎 Note

This project is optimized for Colab. If running locally, make sure all dependencies are installed and hardware acceleration is enabled.



