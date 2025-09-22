# Barcode, QR, and Vehicle Detection using YOLO

This project implements a **web application** for detecting **barcodes, QR codes, and vehicles** in images using YOLOv8, YOLOv9, and YOLOv10 models. The models are trained separately using the **Ultralytics YOLO framework**.

---

## Features

* **Model Selection:** Choose between barcode/QR code detection and vehicle detection.
* **Upload Image:** Upload an image containing objects for detection.
* **Object Detection:** Run detection using YOLO models.
* **Results Display:** View detection results directly on the web interface.

---

## Models

| Detection Type       | YOLO Versions           | Dataset                    |
| -------------------- | ----------------------- | -------------------------- |
| Vehicle Detection    | YOLOv8, YOLOv9, YOLOv10 | Top-view vehicle images    |
| Barcode/QR Detection | YOLOv8, YOLOv9, YOLOv10 | Barcode and QR code images |

---

## Requirements

* Python 3.x
* Streamlit
* Pillow (PIL)
* Ultralytics YOLO
* Pre-trained YOLO model weights (`vehicle.pt` and `barcode.pt`)

---

## Setup

1. **Clone the repository:**

   ```bash
   git clone https://github.com/Het1014/YOLO-Object-Detection.git
   cd YOLO-Object-Detection
   ```

2. **Install the required Python packages:**

   ```bash
   pip install -r requirements.txt
   ```

3. **Download pre-trained YOLO model weights:**

   ```bash
   python download_models.py
   ```
     Place files in the **root directory** of the project.

4. **Run the Streamlit web app:**

   ```bash
   streamlit run main.py
   ```

---

## Usage

1. Open the web app in your browser.
2. Select the model type: **Vehicle Detection** or **Barcode/QR Detection**.
3. Upload an image containing objects.
4. Click **Detect** to see the results.
5. Download or save the output image if needed.

---

## Demo

Check the live demo here: [Live Demo](https://yolo-barcode-vehicle-detection.streamlit.app/)

![Demo Screenshot](docs/demo_screenshot.png)
*Replace `docs/demo_screenshot.png` with your actual screenshot path.*

---

## Screenshots

### Vehicle Detection

![Vehicle Detection](docs/vehicle_detection.png)

### Barcode/QR Detection

![Barcode/QR Detection](docs/barcode_detection.png)

*Replace `docs/vehicle_detection.png` and `docs/barcode_detection.png` with your actual screenshots.*

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
