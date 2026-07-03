# Dysgraphia Text Translator

A Streamlit web application that detects dysgraphic handwriting and converts it into clear, readable English using AI.

## Features

- Detects dysgraphic handwriting from uploaded images.
- Extracts handwritten text using EasyOCR.
- Classifies handwriting as **Normal** or **Dysgraphic**.
- Reconstructs dysgraphic text into grammatically correct English using Google Gemini.
- Displays the original OCR output alongside the corrected text.
- Simple and responsive Streamlit interface.

## Technologies Used

- Python
- Streamlit
- EasyOCR
- Google Gemini API
- OpenCV
- Pillow (PIL)
- NumPy

## Installation

Clone the repository:

```bash
git clone <repository-url>
cd <repository-folder>
```

Install the required libraries:

```bash
pip install streamlit
pip install easyocr
pip install google-generativeai
pip install opencv-python
pip install pillow
pip install numpy
```

## Configuration

Create a `.streamlit/secrets.toml` file and add your Gemini API key:

```toml
GEMINI_API_KEY = "YOUR_API_KEY"
```

## Run the Application

```bash
streamlit run app.py
```

## How It Works

1. Upload an image containing handwritten or printed text.
2. EasyOCR extracts the text from the image.
3. Gemini analyzes the handwriting to determine whether dysgraphia is present.
4. If dysgraphia is detected, the text is reconstructed into clear, grammatically correct English.
5. The application displays the detection result and the translated text.

## Project Structure

```
├── app.py
├── .streamlit/
│   └── secrets.toml
└── README.md
```

## License

This project is intended for educational and research purposes.
