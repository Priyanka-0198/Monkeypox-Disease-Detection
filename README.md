**Monkeypox Disease Detection using YOLO model**

**Overview**
This project detects Monkeypox from skin lesion images using deep learning.  
It integrates YOLOv5 for lesion detection and a CNN classifier for final diagnosis.  
A Flask web app provides an easy interface for uploading images, running predictions, and viewing results.

**Features**
- Upload images for Monkeypox detection.  
- YOLOv5 for object detection.  
- CNN classifier trained on augmented and non-augmented datasets.  
- Web interface built with Flask.  
- User authentication with OTP verification.  
- Real-time webcam detection.  

**Repository Structure**
├── app.py #Flask web application
├── Detection.ipynb #Detection workflow
├── With Augment.ipynb #Training with augmentation
├── Without Augment.ipynb #Training without augmentation
├── static/ #Uploaded images & assets
├── templates/ #HTML templates for Flask
└── model.h5 / best.pt #Trained models (not uploaded here due to size)

**Install Dependencies:**
pip install -r requirements.txt

**Run the file app.py(flask)**
python app.py
Then open the below link in the browser
http://localhost:5000

**Dataset**
Monkeypox and similar lesion images (public sources).
Preprocessed and augmented using Roboflow.
Both augmented and non-augmented datasets were used for model training.

**Results**
CNN trained with augmentation showed higher accuracy compared to without augmentation.
YOLOv5 successfully detected lesion regions with reliable confidence.
Flask app provides instant predictions with user-friendly output.


