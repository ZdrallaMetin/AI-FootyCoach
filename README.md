# AI-FootyCoach
# AI FootyCoach - Proof of Concept

## Overview
AI FootyCoach is an AI-powered football coaching platform designed to help young players (ages 2-18) improve their skills, fitness, and game intelligence. Using artificial intelligence and computer vision, the platform provides real-time feedback, personalized training plans, and tactical analysis. This proof of concept (PoC) focuses on dribbling analysis, key body tracking, and ball detection.

## Features
- **Pose Tracking**: Utilizes MediaPipe to detect key points such as head, shoulders, elbows, knees, and feet.
- **Ball Detection**: Uses a YOLOv8 model for accurate ball tracking.
- **AI Feedback System**: Provides real-time voice and text feedback based on foot-to-ball distance.
- **Automated Dataset Collection**: Saves frames with labeled ball positions for model training.
- **YOLO Model Training**: Fine-tuned training pipeline for ball detection improvements.
- **Cloud Integration**: Uploads trained YOLO models to GitHub.
- **Web Interface**: Streamlit-based UI for uploading and analyzing videos.

## Installation
### Prerequisites
- Python 3.8+
- pip
- Git

### Setup Instructions
1. Clone the repository:
   ```sh
   git clone https://github.com/your_username/ai-footycoach-poc.git
   cd ai-footycoach-poc
   ```
2. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```
3. Run the application:
   ```sh
   streamlit run app.py
   ```

## Usage
- Upload a football dribbling video via the Streamlit interface.
- The system will detect the ball and key body points.
- AI feedback will be provided on dribbling control.
- Collected frames will be saved for training a better YOLO model.
- Optionally, trigger YOLO model training within the UI.

## Training the YOLO Model
1. Collect labeled data (automated in the pipeline).
2. Train the model with:
   ```sh
   python train.py
   ```
3. Upload the trained model to GitHub.

## Roadmap
- Improve AI feedback precision.
- Add shot power and accuracy tracking.
- Expand dataset for better generalization.
- Integrate smart wearable device support.

## Contributing
We welcome contributions! Feel free to open issues or submit pull requests.

## License
MIT License. See LICENSE file for details.

