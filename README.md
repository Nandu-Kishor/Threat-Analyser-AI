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
![Dashboard Screenshot](https:![Screenshot 2025-02-11 191410](https://github.com/user-attachments/assets/ea8513c5-5919-4f0e-9dc8-5c121a5cb048)
 ![Screenshot 2025-02-11 191533](https://github.com/user-attachments/assets/59fd96d4-b95d-40dd-90a0-31941706d8e8)![Screenshot 2025-02-11 191651](https://github.com/user-attachments/assets/72067589-4c36-4253-b18b-48d659d09129)
![Screenshot 2025-02-11 191719](https://github.com/user-attachments/assets/8a56e2d2-7be3-4932-8458-ed7a5b24f0ee)
![Screenshot 2025-02-11 191808](https://github.com/user-attachments/assets/acd04c7f-e701-45d5-8941-98a35c706176)
![Screenshot 2025-02-11 191842](https://github.com/user-attachments/assets/56301dd9-a1dc-4eb1-b2aa-752ca2cf6e41)
![Screenshot 2025-02-11 191916](https://github.com/user-attachments/assets/77050b4b-2997-4cdb-b720-588856dc778e)
![Screenshot 2025-02-11 191949](https://github.com/user-attachments/assets/389645ff-78b2-4df6-bde1-fd082167b70b)
![Screenshot 2025-02-11 191949](https://github.com/user-attachments/assets/8ce065aa-57bf-40e3-95f2-904b33507f15)![Screenshot 2025-02-11 192026](https://github.com/user-attachments/assets/7bde5ac2-869d-4991-8084-75a357a88f94)

![WhatsApp Image 2025-02-12 at 09 35 03_910e61c0](https://github.com/user-attachments/assets/f08c88f5-9ffb-41f7-af9c-7a1c0df0041d)



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
