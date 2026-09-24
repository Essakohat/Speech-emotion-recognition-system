# Speech Emotion Recognition System

Speech Emotion Recognition project using the Wav2Vec2-base model to classify audio into six emotions: Angry, Sad, Happy, Fear, Disgust, and Neutral. Includes training scripts, inference pipeline, and workflow examples.

## Project Structure

- `emotion_recognition_notebook.ipynb`: Core notebook for model training, evaluation, and experiments.
- `sorting dataset.ipynb`: Notebook for preprocessing, organizing, and preparing the dataset.
- `gradio_app.py`: A web interface built with Gradio to test the emotion recognition model interactively.
- `requirements.txt`: List of Python dependencies required to run the project.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Essakohat/Speech-emotion-recognition-system.git
   cd Speech-emotion-recognition-system
   ```

2. Create a virtual environment (optional but recommended):
   ```bash
   python -m venv venv_emotion_recognition
   # On Windows:
   venv_emotion_recognition\Scripts\activate
   # On macOS/Linux:
   source venv_emotion_recognition/bin/activate
   ```

3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Dataset

The dataset used for this project is hosted on Kaggle due to GitHub file size limits.

👉 **[Download the Speech Emotion Recognition Dataset on Kaggle](https://www.kaggle.com/datasets/muhammadessaai/speech-emotions-recognition-dataset)**

Once downloaded, extract the archive and place the raw audio files inside a folder named `dataset/` in the root directory before running the preprocessing or training notebooks.

## Usage

### Web Interface

To launch the interactive web application, run:
```bash
python gradio_app.py
```
This will start a local Gradio server where you can upload audio files or record your voice to see the model's predictions.

### Notebooks

You can use Jupyter to open and run the provided notebooks:
```bash
jupyter notebook
```
- Start with `sorting dataset.ipynb` if you need to prepare your data.
- Then, proceed to `emotion_recognition_notebook.ipynb` to train or evaluate the model.
