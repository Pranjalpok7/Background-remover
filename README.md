# Background Removal Web Application

This repository contains a web application for removing backgrounds from images using a deep learning model. The application is built with FastAPI for the backend and includes an HTML frontend for uploading images and displaying the results.

## Features

- **Upload Images**: Users can upload images via the web interface.
- **Background Removal**: Automatically removes the background from uploaded images using a pre-trained deep learning model.
- **Display Results**: Shows the original image alongside the background-removed image.

## Technologies Used

- **FastAPI**: A modern, fast (high-performance) web framework for building APIs with Python 3.7+.
- **PIL (Pillow)**: A Python Imaging Library (Pillow) that adds image processing capabilities to your Python interpreter.
- **PyTorch**: An open-source machine learning library for Python, primarily developed by Facebook's AI Research lab.
- **HTML/CSS**: For building the frontend user interface.

## Project Structure

my_project/
├── models/
│ └── __init__.py
| └── isnet.py # Model definition
├── myenv # Virtual environment (optional)
├── saved_models/ # Directory for storing model weights
│ └── isnet.pth # Pre-trained model weights
├── static/ # Static files directory
│ ├── uploads.jpg # Example uploaded image (can be replaced)
│ └── results.jpg # Example background-removed image (can be replaced)
├── bgRemove.py # Script for background removal
├── data_loader_cache.py # Data loader and preprocessing utilities
├── index.html # Home page template
├── main.py # Main FastAPI application
├── requirements.txt # List of project dependencies


<br>

## Run Our Code

<br>


### (1) Clone this repo
```
git clone https://github.com/xuebinqin/DIS.git
```

### (2) Create and activate a virtual environment (optional but recommended):
```
python -m venv myenv
source myenv/bin/activate  # On Windows, use `myenv\Scripts\activate`

```

### (3) Install the required dependencies:
```
pip install -r requirements.txt
```

### (4) Download the pre-trained model weights and place them in the saved_models directory. Ensure the weights file is named isnet.pth


###(5) Run the application:
```
uvicorn main:app --reload

```

###(6) Access the application:
<br> Open your web browser and navigate to 'http://localhost:8000'.
