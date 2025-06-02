# Emotion Detection Application

## 🧠 Project Overview

The **Emotion Detection Application** is a Python-based web application that uses IBM Watson's Embeddable AI library to analyze and detect emotions from textual input. It takes a sentence or phrase as input and returns the emotional distribution across five primary emotions: **anger**, **disgust**, **fear**, **joy**, and **sadness**, as well as the **dominant emotion**.

This project demonstrates end-to-end development including emotion detection integration, unit testing, error handling, packaging, Flask web deployment, and static code analysis compliance.

---

## 🚀 Features

* Emotion analysis using Embeddable AI via a POST request
* Flask-based web deployment with a simple user interface
* Error handling for blank input and invalid responses
* Unit tests for verification of accuracy
* Fully packaged and importable module (`EmotionDetection`)
* PEP8-compliant code with a perfect 10/10 PyLint score

---

## 🧹 Project Structure

```
final_project/
│
├── EmotionDetection/
│   ├── __init__.py              # Initializes the EmotionDetection package
│   └── emotion_detection.py     # Contains the emotion_detector function
│
├── static/
│   └── mywebscript.js           # JavaScript file for frontend logic
│
├── templates/
│   └── index.html               # HTML file for user interface
│
├── server.py                    # Flask app for web deployment
├── test_emotion_detection.py    # Unit tests for emotion detection
├── requirements.txt             # Project dependencies
└── README.md                    # Project documentation
```

---

## 🧠 Installation & Setup

1. **Clone the Repository**

   ```bash
   git clone <your-repo-url>
   cd final_project
   ```

2. **Create a Virtual Environment (Optional but Recommended)**

   ```bash
   python3 -m venv env
   source env/bin/activate
   ```

3. **Install Dependencies**

   ```bash
   pip install -r requirements.txt
   ```

4. **Run the Application**

   ```bash
   python3 server.py
   ```

5. Open a browser and visit [http://localhost:5000](http://localhost:5000)

---

## ⚙️ Usage

* Enter any sentence in the input field (e.g., `I think I am having fun`)
* Click **Submit**
* The application will display the predicted emotion distribution and the **dominant emotion**
* In case of blank input, the app will display an error message:
  **"Invalid text! Please try again!"**

---

## 🧪 Unit Testing

Run the following command to execute unit tests:

```bash
python3 test_emotion_detection.py
```

Sample test cases include:

* `"I am glad this happened"` → joy
* `"I am really mad about this"` → anger
* `"I feel disgusted just hearing about this"` → disgust
* `"I am so sad about this"` → sadness
* `"I am really afraid that this will happen"` → fear

---

## 🧹 Static Code Analysis

Run static code analysis using **PyLint**:

```bash
pylint server.py
```

A perfect **10/10** PyLint score is achieved by:

* Adding **docstrings** to all functions
* Proper code formatting and organization
* Avoiding unused imports and variables

---

## ❗ Error Handling

* The application returns `None` values for all emotions if a blank input is submitted.
* The UI will display a user-friendly error message in such cases.

---

## 📆 Packaging

The core logic is packaged as `EmotionDetection`, which can be imported and reused:

```python
from EmotionDetection.emotion_detection import emotion_detector

result = emotion_detector("I love this new technology")
```

---

## 💡 Learnings

By completing this project, I have:

✅ Integrated Embeddable AI for real-time emotion detection
✅ Parsed and processed JSON API responses
✅ Created a testable and reusable Python package
✅ Built and deployed a Flask-based web application
✅ Handled edge cases and user errors gracefully
✅ Ensured PEP8 compliance via PyLint

---

## 📃 License

This project is for educational purposes and follows the guidelines of IBM Skills Network coursework.
