"# Sign-Language-detection-system" 
# Sign Language Detection System 

A real-time sign language detection system built using **Python, OpenCV, MediaPipe, and Machine Learning**. The application uses a webcam to capture hand gestures, extracts hand landmarks, and predicts the corresponding sign using a trained Random Forest classifier. A Tkinter-based graphical user interface displays the results.

The project aims to make communication more accessible for people with hearing and speech impairments by translating recognized hand signs into text.

## Features

- **Real-time gesture detection** using a webcam.
- **Hand landmark detection** with MediaPipe.
- **Image and video processing** using OpenCV.
- **Machine learning classification** using a Random Forest model.
- **Alphabet recognition** for signs from A to Z.
- **Graphical user interface** built with Tkinter.
- **Dataset collection and labeling** for training hand gesture recognition models.
- **Performance evaluation** using accuracy and a confusion matrix.

##  Tech Stack

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| OpenCV | Webcam access and image processing |
| MediaPipe | Hand tracking and landmark extraction |
| Scikit-learn | Random Forest classification |
| NumPy | Numerical computations |
| Pandas | Dataset handling and manipulation |
| Matplotlib | Visualization and evaluation |
| Tkinter | Graphical user interface |
| Pickle | Saving and loading the trained model |

##  How It Works

The system follows these steps:

1. **Capture:** The webcam captures live video frames of the user's hand.
2. **Preprocess:** OpenCV processes the captured frames.
3. **Landmark extraction:** MediaPipe identifies hand landmarks, including finger joints and wrist positions.
4. **Classification:** The extracted features are passed to the trained Random Forest model.
5. **Prediction:** The model predicts the corresponding hand gesture or alphabet.
6. **Display:** The Tkinter interface displays the recognized result.

##  Model Performance

The project report records an average training accuracy of approximately **95%**.

Actual recognition performance may vary depending on lighting conditions, hand positioning, partially obscured gestures, and differences between users.

##  System Requirements

The project report specifies the following hardware and software requirements:

- **Operating system:** Windows 11 or Linux
- **RAM:** 8 GB
- **Storage:** 512 GB SSD
- **Camera:** Webcam for live gesture capture
- **Python:** A compatible Python environment
- **IDE:** Visual Studio Code or another Python-compatible editor

##  Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/rashmitha-03/sign-language-detection-system.git
```

Navigate to the project directory:

```bash
cd sign-language-detection-system
```

### 2. Create a virtual environment

```bash
python -m venv venv
```

Activate the environment.

**Windows:**

```bash
venv\Scripts\activate
```

**Linux:**

```bash
source venv/bin/activate
```

### 3. Install dependencies

Install the required Python libraries:

```bash
pip install opencv-python mediapipe scikit-learn numpy pandas matplotlib
```

Tkinter is commonly included with standard Python installations. On Linux, it may need to be installed separately through the operating system's package manager.

### 4. Add the trained model

Place the trained model file in the location expected by the application. The project report refers to a serialized model named `model.p`.

Make sure the model file and its expected input features match the implementation.

### 5. Run the application

Run the main Python application:

```bash
python main.py
```

**Note:** Replace `main.py` with the actual entry-point filename in your repository. The installation and execution commands should be adjusted to match the files included in the project.

##  Dataset and Training

The dataset was collected using real-time webcam images of hand gestures.

The process includes:

- Capturing hand gesture frames using OpenCV.
- Assigning labels to the captured gestures.
- Organizing frames into categories corresponding to the alphabet labels.
- Extracting hand landmarks using MediaPipe.
- Training a Random Forest classifier.
- Evaluating the model using accuracy and a confusion matrix.

The reported dataset covers alphabet signs from **A to Z**, with multiple frames captured from different angles.

## Suggested Project Structure

The following is an example structure for organizing the repository. Update it to reflect the files and directories in your actual project.

```text
sign-language-detection-system/
│
├── main.py                 # Main application
├── model.p                 # Trained model (if included)
├── dataset/                # Hand gesture dataset (if included)
│   ├── A/
│   ├── B/
│   └── ...
├── requirements.txt        # Python dependencies
├── README.md               # Project documentation
└── .gitignore              # Files excluded from Git
```

##  Limitations

- Recognition may be affected by poor lighting or partially hidden hands.
- Accuracy can vary with hand orientation, background conditions, and individual signing styles.
- The current implementation focuses primarily on alphabet-level gesture recognition.
- Continuous sign language interpretation, sentence construction, and support for additional sign languages require further development.

##  Future Enhancements

Potential improvements include:

- Expanding the vocabulary to recognize more gestures and complete words.
- Supporting Indian Sign Language and other regional sign languages.
- Improving recognition accuracy across different users and environments.
- Adding speech output for recognized gestures.
- Developing a mobile application.
- Integrating wearable devices or augmented reality.
- Allowing users to correct predictions and contribute additional training examples.

##  Applications

- Assistive communication
- Inclusive educational environments
- Sign language learning and demonstration
- Accessibility-focused applications
- Helps with sign language learning process, and active communication


## 🎓 Academic Project

This project demonstrates the application of computer vision and machine learning to an accessibility-focused problem. It explores how hand landmark extraction and gesture classification can support real-time sign-to-text recognition.

**If you find this project useful, consider giving the repository a ⭐ on GitHub!**
