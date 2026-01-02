# Cotton Leaf Disease Prediction with OpenCV

![Plant Health Demo](demo.gif) *Example of disease detection workflow*

## Project Overview
This web application uses computer vision (OpenCV) and machine learning to detect diseases in cotton plant leaves. Users can upload leaf images, and the system analyzes them to identify common cotton diseases like bacterial blight, fusarium wilt, or verticillium wilt.

## Features
- **Image Processing**: Preprocesses leaf images using OpenCV for noise reduction and feature enhancement
- **Disease Detection**: Identifies common cotton diseases based on visual symptoms
- **User-Friendly Interface**: Simple web interface for image upload and results display
- **Visual Feedback**: Highlights affected areas on the leaf image
- **Responsive Design**: Works on both desktop and mobile devices

## Tech Stack
- **Backend**: Python Flask
- **Computer Vision**: OpenCV
- **Frontend**: HTML5, CSS3, JavaScript
- **Machine Learning**: [Specify ML library if used - e.g., TensorFlow, PyTorch]
- **Dependencies**: See requirements.txt

## Project Structure
cotton-leaf-disease-prediction/
├── README.md # Project documentation
├── app.py # Flask application backend
├── templates/
│ └── index.html # Main web interface
├── static/
│ ├── style.css # Stylesheet
│ └── uploads/ # Stores uploaded images
├── requirements.txt # Python dependencies
└── model/ # Trained ML models [if applicable]
└── cotton_model.h5

text

## Installation
1. Clone the repository:
```bash
git clone https://github.com/yourusername/cotton-leaf-disease-prediction.git
cd cotton-leaf-disease-prediction
Install dependencies:

bash
pip install -r requirements.txt
[Optional] Place trained model files in the model/ directory

Usage
Start the Flask server:

bash
python app.py
Visit in your browser:

text
http://localhost:5000
Use the interface:

Click "Upload Image" to select a cotton leaf photo

View disease prediction results

See affected areas highlighted on the image

How It Works
Image Preprocessing:

Converts image to HSV color space

Applies Gaussian blur for noise reduction

Uses thresholding to isolate leaf and spots

Feature Extraction:

Calculates spot characteristics (size, shape, distribution)

Analyzes color patterns in affected areas

Disease Prediction:

[Describe ML model inference process]

Compares features against disease patterns

Result Visualization:

Generates overlay highlighting affected areas

Displays disease diagnosis and confidence

Contributing
Contributions are welcome! Please follow these steps:

Fork the repository

Create your feature branch (git checkout -b feature/your-feature)

Commit your changes (git commit -m 'Add some feature')

Push to the branch (git push origin feature/your-feature)

Open a pull request

License
Distributed under the MIT License. See LICENSE for more information.

Future Improvements
Expand to other crops

Add disease prevention recommendations

Implement live camera capture mode

Enhance model accuracy with more training data

Create mobile app version

text

## Key Files Explained:
1. **app.py** - Contains:
   - Flask routes for web endpoints
   - Image processing functions using OpenCV
   - Machine learning model loading and inference
   - File handling for image uploads

2. **index.html** - Features:
   - Image upload form
   - Result display area
   - Canvas for image visualization
   - Responsive design elements

3. **style.css** - Provides:
   - Clean interface styling
   - Mobile-responsive layouts
   - Visualization element formatting

4. **README.md** (this file) - Includes:
   - Project overview and features
   - Setup and usage instructions
   - Technical documentation
   - Contribution guidelines

For best results:
1. Ensure you have Python 3.7+ installed
2. Add your trained ML model to the `model/` directory
3. Install all required packages from requirements.txt
4. For production deployment, consider using:
   - Gunicorn/UWSGI for WSGI server
   - Nginx as reverse proxy
   - Containerization with Docker
