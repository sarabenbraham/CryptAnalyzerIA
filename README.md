# CryptAnalyzer AI 🔐

> An AI-powered web platform for automatic cipher detection and cryptanalysis of classical encryption systems.

![Python](https://img.shields.io/badge/Python-3.10+-blue?style=flat-square&logo=python)
![Flask](https://img.shields.io/badge/Flask-2.x-black?style=flat-square&logo=flask)
![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-orange?style=flat-square&logo=scikit-learn)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)
![Status](https://img.shields.io/badge/Status-In%20Development-yellow?style=flat-square)

---

## Overview

**CryptAnalyzer AI** automatically identifies the type of classical cipher used on an encrypted text, launches the appropriate cryptanalysis attack, and returns the decrypted plaintext along with a security score — all through a clean web interface.

Built as part of **AI EXPO 2026** — Student Creativity and Innovation, Blida 1 University.

---

## Features

- 🤖 **AI-based cipher classification** — Automatically detects Classic ciphers using a trained ML model
- ⚔️ **Automated attacks** — Brute-force and frequency analysis attacks per cipher type
- 📊 **Security scoring** — Evaluates the strength of the detected cipher
- 🌐 **Web interface** — Simple, responsive UI built with Flask

---

## Supported Ciphers

| Cipher       | Attack Method                  | Keys Space |
|--------------|--------------------------------|------------|
| Caesar       | Brute-force                    | 26         |
| Affine       | Brute-force                    | 312        |
| Hill 2×2     | Frequency analysis             | ~157,000   |
|Vigenère      |Kasiski + IC                    |🔨 en cours |
|Playfair      |Analyse bigrammes               |🔨 en cours |
|Substitution  |Algorithme génétique simplifié  |🔨 en cours |
|OTP           |Indéchiffrable (affiché)        |🔨 en cours |

---

## Project Structure

```
cryptanalyzer-ai/
├── app.py               # Flask application entry point
├── attacks.py           # Cryptanalysis attack scripts
├── classifier.py        # ML cipher classification model
├── models/
│   └── cipher_model.pkl # Trained scikit-learn model
├── templates/
│   └── index.html       # Web interface
├── static/
│   └── style.css
├── requirements.txt
└── README.md
```

---

## Getting Started

```bash
# Clone the repository
git clone https://github.com/your-username/cryptanalyzer-ai.git
cd cryptanalyzer-ai

# Install dependencies
pip install -r requirements.txt

# Run the app
python app.py
```

Then open `http://localhost:5000` in your browser.

---

## Tech Stack

- **Backend** — Python, Flask
- **Machine Learning** — scikit-learn, NumPy
- **Frontend** — HTML, CSS, JavaScript
- **Cryptography** — Custom implementations of Classics ciphers

---

## Author

**Benbraham Sara** — Computer Science Student, University of Sciences and technology Houari Boumediene 
[![GitHub](https://img.shields.io/badge/GitHub-@sarabenbraham-black?style=flat-square&logo=github)](https://github.com/sarabenbraham)

---

## License

This project is licensed under the [MIT License](LICENSE).
