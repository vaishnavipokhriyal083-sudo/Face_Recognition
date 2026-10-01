# Face Recognition using OpenCV

## 📌 Project Overview

This project demonstrates **face detection using Python and OpenCV**. It uses the **Haar Cascade Classifier** to identify human faces from an uploaded image.

The project is implemented in **Google Colab**, where users can upload an image along with the Haar Cascade XML file and process the image for face detection.

## 🎯 Objective

The main objective of this project is to understand the fundamentals of **Computer Vision and Face Detection** using OpenCV.

The project covers:

* Loading and processing images
* Uploading files in Google Colab
* Using OpenCV for image processing
* Using Haar Cascade for face detection
* Displaying images using PIL and OpenCV
* Verifying whether an image has been successfully loaded

## 🛠️ Technologies Used

* **Python**
* **OpenCV (cv2)**
* **PIL (Python Imaging Library)**
* **Google Colab**
* **Haar Cascade Classifier**
* **Jupyter Notebook**

## 📂 Project Structure

```text
Face-Recognition/
│
├── Face_Recognition.ipynb
├── haarcascade_frontalface_default.xml
├── photo.png
└── README.md
```

> The image and XML files are used as input files during execution. The notebook uploads these files directly in Google Colab.

## ⚙️ How It Works

### 1. Import Required Libraries

The project starts by importing OpenCV and Google Colab utilities.

```python
import cv2
from google.colab import files
from google.colab.patches import cv2_imshow
```

### 2. Upload Input Files

The notebook allows the user to upload the required files, including the Haar Cascade XML classifier and an image.

```python
uploaded = files.upload()
```

### 3. Load the Image

The uploaded image is loaded using OpenCV.

```python
img = cv2.imread("photo.png")
```

The notebook also checks whether the image was loaded successfully.

### 4. Display the Image

PIL and IPython display utilities are used to locate and display uploaded image files.

```python
from IPython.display import display
from PIL import Image
import glob
```

The notebook searches for `.jpg`, `.jpeg`, and `.png` files before displaying an available image.

### 5. Face Detection

The project uses the **Haar Cascade frontal-face classifier** to identify faces in the image.

The classifier file used is:

```text
haarcascade_frontalface_default.xml
```

## 🚀 How to Run the Project

### Option 1: Google Colab

1. Open the `Face_Recognition.ipynb` notebook in Google Colab.
2. Run the cells sequentially.
3. Upload:

   * `haarcascade_frontalface_default.xml`
   * Your `.jpg` or `.png` image
4. Execute the image-processing cells.
5. View the processed image and face-detection output.

### Option 2: Local Environment

Install the required libraries:

```bash
pip install opencv-python pillow
```

Then open the notebook using Jupyter Notebook or JupyterLab.

## 📸 Input

The project accepts common image formats such as:

* JPG
* JPEG
* PNG

The notebook searches for these image formats during execution.

## 🔍 Key Learning Outcomes

Through this project, I learned:

* Fundamentals of computer vision
* Image loading and processing using OpenCV
* Working with Haar Cascade classifiers
* Handling image files in Google Colab
* Basic image visualization using PIL
* Using Python libraries for computer vision applications

## 🔮 Future Improvements

This project can be further extended by adding:

* Real-time face detection using a webcam
* Face recognition using a trained dataset
* Multiple-face detection
* Face counting
* Attendance management using face recognition
* Face recognition with Deep Learning
* Real-time detection dashboard

## 📚 Applications

Face detection technology can be used in applications such as:

* Smart attendance systems
* Security systems
* Human-computer interaction
* Image analysis
* Surveillance systems
* Access-control systems

## 👩‍💻 Author

**Vaishnavi Pokhriyal**

B.Tech CSE Student | AI & Data Science Enthusiast

### ⭐ If you found this project useful, consider giving the repository a star!
