Speech Emotion Recognition using Wav2Vec2

This project implements a Speech Emotion Recognition (SER) system that can classify human speech into six emotions:
Angry, Sad, Happy, Fear, Disgust, Neutral.

It is powered by Hugging Face’s Wav2Vec2 model and trained on custom audio datasets. The system processes raw speech audio, extracts meaningful features, and predicts the underlying emotion.

🔍 Why This Project?

Human communication is not just about what we say, but how we say it. Emotions in speech carry important signals for:

Improving human-computer interaction (e.g., empathetic voice assistants).

Enhancing call center analytics and customer service.

Supporting mental health monitoring and well-being applications.

Building more natural conversational AI.

This project is designed to demonstrate how modern transformer-based speech models (like Wav2Vec2) can be fine-tuned for emotion classification.

🛠 Features

End-to-end audio emotion recognition pipeline.

Uses Wav2Vec2 base model for feature extraction.

Supports custom datasets organized by emotion labels.

Handles audio resampling (converts everything to 16kHz).

Evaluates performance with confusion matrix, F1-score, and classification report.

📂 Project Structure
├── data/                 # Dataset folders (train/test split by emotion)
├── notebooks/            # Jupyter notebooks for experimentation
├── scripts/              # Training and evaluation scripts
├── images/               # Visualizations (confusion matrix, model workflow, etc.)
├── workflows/            # GitHub workflows (CI/CD if enabled)
├── model/                # Saved model checkpoints
├── requirements.txt      # Python dependencies
└── README.md             # Project documentation

🚀 Getting Started
1. Clone the repository
git clone https://github.com/your-username/speech-emotion-recognition.git
cd speech-emotion-recognition

2. Install dependencies
pip install -r requirements.txt

3. Prepare dataset

Organize your dataset into folders like:

data/train/
    ├── Angry/
    ├── Sad/
    ├── Happy/
    ├── Fear/
    ├── Disgust/
    └── Neutral/
data/test/ (same structure)

4. Train the model
python train.py

5. Evaluate
python evaluate.py

📊 Results

Achieves reliable classification across six emotions.

Generates confusion matrix and classification report for evaluation.

Can be extended to more datasets or additional emotions.

🔧 Technologies Used

PyTorch — deep learning framework.

Torchaudio — audio processing and loading.

Transformers (Hugging Face) — Wav2Vec2 processor and model.

Scikit-learn — label encoding and evaluation metrics.

Matplotlib & Seaborn — visualizations.

🌍 Real-World Applications

Customer support sentiment tracking.

Emotion-aware virtual assistants.

Therapy and mental health monitoring.

Interactive entertainment and gaming.

📌 Future Work

Improve robustness for noisy/real-world audio.

Add multilingual support.

Deploy as a real-time web or mobile application.

Experiment with advanced architectures (HuBERT, Whisper, etc.).

🤝 Contributing

Contributions are welcome!

Fork the repo

Create a new branch (feature/your-feature)

Commit changes

Submit a pull request

📜 License

This project is licensed under the MIT License — feel free to use and modify with proper attribution.

🙌 Acknowledgements

Hugging Face for Transformers.

PyTorch & Torchaudio for audio deep learning support.

Open-source datasets used for training and testing.
