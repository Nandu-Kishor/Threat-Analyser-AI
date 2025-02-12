# Threat Analyzer AI 🔍🛡️

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python Version](https://img.shields.io/badge/Python-3.10%2B-blue.svg)](https://www.python.org/)
[![MongoDB Atlas](https://img.shields.io/badge/MongoDB-Cloud-green.svg)](https://www.mongodb.com/atlas)

Transform unstructured cyber threat data into structured intelligence using Gemini LLM and MongoDB Atlas.

![Workflow Diagram](![image](description.png)) <!-- Replace with actual diagram -->

## Table of Contents
- [Features](#features)
- [Installation](#installation)
- [Configuration](#configuration)
- [Usage](#usage)
- [Tech Stack](#tech-stack)
- [API Reference](#api-reference)
- [Screenshots](#screenshots)
- [Future Enhancements](#future-enhancements)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)

## Features ✨
- **AI-Powered Analysis**: Gemini LLM API for threat extraction
- **Structured Data Output**:
  - Attack Identification
  - MITRE ATT&CK Tactics Mapping
  - Technique/Sub-technique Classification
  - Detailed Mitigation Strategies
- **Cloud Storage**: MongoDB Atlas integration
- **Interactive Dashboard**:
  - Threat Visualization
  - Advanced Search & Filtering
  - Timeline Analysis

## Installation ⚙️

### Prerequisites
- Python 3.10+
- HTML, CSS, JS (for frontend)
- MongoDB Atlas account
- Gemini API key

### Backend Setup
```bash
git clone https://github.com/Guhan-Sachi/Threat-Analyser-AI
cd Threat-Analyser-AI/backend
pip install -r requirements.txt
```

### Frontend Setup
```bash
cd ../frontend
# Follow the instructions for setting up the frontend
```

## Configuration 🔧

1. **MongoDB Atlas**: Set up your MongoDB Atlas cluster and get the connection string.
2. **Gemini API**: Obtain your Gemini API key and configure it in the application.
3. Create a `.env` file in the root directory of the backend with the following content:

```ini
MONGODB_URI=your_mongodb_connection_string
GEMINI_API_KEY=your_gemini_api_key
```

## Usage 🚀

Start the backend server:
```bash
cd backend
python app.py
```

Open the frontend in your browser to interact with the dashboard.

## Tech Stack 🛠️
- **Backend**: Python, Flask
- **Frontend**: HTML, CSS, JavaScript
- **Database**: MongoDB Atlas
- **AI**: Gemini LLM API

## API Reference 📚

### Threat Analysis Endpoint
- **URL**: `/api/analyze`
- **Method**: `POST`
- **Request Body**:

```json
{
  "data": "unstructured threat data"
}
```

- **Response**:

```json
{
  "threats": [
    {
      "Title" : "Name of the Cyber Attack"
      "detailed description": "Description of the cyber attack",
      "date" : "Uploaded date in database",
      "attack_type": "Data Breach",
      "Risk Factor": "Severity of cyber attack",
      "Key points" : "points about cyber attack",
      "tactic": "Initial Access",
      "technique": "Phishing",
      "mitigation": "User training and awareness"
    }
  ]
}
```

## Screenshots 📸
![Dashboard Screenshot](https://via.placeholder.com/800x400.png?text=Dashboard) <!-- Replace with actual screenshot -->
![Screenshot 2025-02-11 191410](https://github.com/user-attachments/assets/19458157-2c56-4ffa-ab6e-edb1d7d30765)

## Future Enhancements 🚀
- Integration with additional threat intelligence sources
- Real-time threat detection and alerting
- Machine learning-based threat prediction

## Contributing 🤝
Contributions are welcome! Please read the contributing guidelines for more information.

## License 📄
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements 🙏
- **[Gemini LLM](https://aistudio.google.com/)**
- **[MongoDB Atlas](https://www.mongodb.com/atlas)**
