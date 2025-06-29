# AlpersPi 🚓🔍

A real-time number plate detection and recognition system built using OpenCV and deep learning, designed to run on lightweight devices like Raspberry Pi. This project aims to automate vehicle monitoring and surveillance using license plate detection and OCR (Optical Character Recognition).

## 🚀 Overview

**AlpersPi** processes live video streams to detect number plates and extract the license numbers from vehicles in real-time. The system uses pre-trained object detection models to locate the plate and applies OCR techniques to extract readable text.

## 🧠 Features

- 📹 Real-time video stream processing (Raspberry Pi camera or USB webcam)
- 🪪 Automatic number plate detection using deep learning (YOLO or Haar Cascades)
- 🔠 OCR-based license number extraction using Tesseract or EasyOCR
- 💾 Optional logging of detected numbers with timestamp
- 🧠 Lightweight design optimized for edge devices

## 🛠️ Tech Stack

- **Python**
- **OpenCV**
- **YOLO / Haar Cascade**
- **EasyOCR / Tesseract**
- **Raspberry Pi**

## 📁 Project Structure

```
AlpersPi/
│
├── models/                  # Pre-trained models for plate detection
├── src/
│   ├── detector.py          # Plate detection logic
│   ├── ocr.py               # OCR logic for reading plate numbers
│   ├── utils.py             # Helper functions
│   └── main.py              # Main execution script (video capture + detection)
├── samples/                 # Sample test images and videos
├── logs/                    # Detected plates and timestamps
├── README.md                # Project documentation
└── requirements.txt         # Python dependencies
```

## ⚙️ How It Works

1. Captures frames from a live video stream.
2. Detects license plate in each frame using a trained model.
3. Extracts the plate region and runs OCR to recognize characters.
4. Displays the result in real-time and optionally logs the plate info.

## 📦 Installation

1. Clone the repository:

```bash
git clone https://github.com/WinUdupa/AlpersPi.git
cd AlpersPi
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Run the system:

```bash
python src/main.py
```

## 🧪 Example Output

```
[INFO] Detected Plate: KA03MR1234 at 2025-06-29 16:30:12
[INFO] Detected Plate: KA01AB5678 at 2025-06-29 16:30:45
```

## 📌 To Do

- [ ] Improve OCR accuracy under low-light conditions
- [ ] Add vehicle make/model classification
- [ ] Integrate with cloud database or dashboard

## 📜 License

This project is licensed under the MIT License.

## 🤝 Contributing

Pull requests and suggestions are welcome. Let's build a smarter traffic surveillance system together!

---

**Created by [Vineeth Udupa](https://github.com/WinUdupa)** 🎯
