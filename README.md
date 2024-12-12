# PDF Quiz Generator

The **PDF Quiz Generator** is a Flask-based web application that allows users to upload a PDF file, extract and summarize its content, generate multiple-choice questions (MCQs), and interact with the content using a chat interface. This project uses the Groq Cloud API for text summarization, question generation, and chat functionality.

---

## Features

- **PDF Upload**: Users can upload PDF files, which are processed to extract text content.
- **Content Summarization**: Summarizes the PDF content using the Groq Cloud API.
- **Dynamic Question Generation**: Generates MCQs based on the PDF content.
- **Chat with PDF**: Allows users to interact with the PDF content through a chat interface.

---

## Project Structure

project/ │ ├── flask_session/ # Directory for server-side session data (auto-created) │ ├── static/ # Directory for static assets (CSS, JS, etc.) │ ├── templates/ # HTML templates │ ├── index.html # Main page for uploading PDFs │ ├── result.html # Page for displaying results (summary, questions, chat) │ ├── uploads/ # Directory for storing uploaded PDF files │ ├── app.py # Main Flask application file │ ├── venv/ # Python virtual environment │ └── requirements.txt # Dependencies for the project (to be created)

yaml
Copy code

---

## Installation and Setup

### Prerequisites

- Python 3.10 or later
- pip (Python package manager)
- A Groq Cloud API key

### Steps

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/pdf-quiz-generator.git
   cd pdf-quiz-generator
Set Up Virtual Environment:

python -m venv venv
source venv/bin/activate        # For Linux/MacOS
venv\Scripts\activate          # For Windows

Install Dependencies: Create a requirements.txt file with the following:

Flask==2.3.2
Flask-Session==0.4.0
requests==2.31.0
PyPDF2==3.0.1

Then install them:

pip install -r requirements.txt
Set Up Upload Directory: Ensure the uploads/ directory exists in the root folder:

mkdir uploads
Configure API Key: Replace the API_KEY in app.py with your Groq Cloud API key:

API_KEY = "your_groq_api_key_here"
Run the Application:

python app.py
The app will be available at http://127.0.0.1:5000.

Navigate to the Upload Page.
Upload a PDF file.
View the extracted text and summarized content.
Generate dynamic questions or interact with the content using the chat feature.
Technologies Used
Flask: Web framework for Python.
PyPDF2: For extracting text from PDF files.
Groq Cloud API: For summarization, question generation, and chat functionalities.
HTML/CSS: For the user interface.

Future Enhancements
Add a file preview feature for uploaded PDFs.
Enhance question generation with additional formatting options.
Improve chat accuracy and responsiveness.
Contributing

Contributions are welcome! Please follow these steps:

Fork the repository.
Create a new branch (git checkout -b feature/YourFeatureName).
Commit your changes (git commit -m 'Add a new feature').
Push to the branch (git push origin feature/YourFeatureName).
Open a pull request.
License
This project is licensed under the MIT License. See the LICENSE file for details.


Author
Developed by SABERA BANU.

Acknowledgments

Flask Documentation
PyPDF2 Documentation
Groq Cloud API
vbnet
