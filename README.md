# Applicant Tracking System (ATS) Project

## Overview

This project is an Applicant Tracking System (ATS) that allows users to upload resumes in PDF format, analyze them using Google Generative AI, and compare them with job descriptions. The system provides insights and evaluations based on the uploaded resume's content, including a percentage match against the job description.

## Features

- **Resume Upload and Conversion:** Upload a resume in PDF format, which is then converted to an image for processing.
- **AI-Powered Analysis:** Uses Google Generative AI (Gemini model) to evaluate resumes against job descriptions.
- **Interactive User Interface:** Built using Streamlit for easy interaction and visualization of results.
- **Environment Variable Management:** Securely handles API keys and other sensitive information using Python-Dotenv.

## Requirements

Before you begin, ensure you have the following installed:

- Python 3.8 or higher
- pip (Python package installer)

## Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/your-username/ats-project.git
   cd ats-project
   ```

2. **Create a virtual environment:**

   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. **Install dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

4. **Set up environment variables:**

   Create a `.env` file in the root directory and add the necessary environment variables:

   ```env
   GOOGLE_API_KEY=your-google-api-key
   ```

## Usage

1. **Run the Streamlit app:**

   ```bash
   streamlit run app.py
   ```

2. **Upload a resume:**

   - Upload a PDF file using the file uploader provided in the web interface.
   - The system will convert the first page of the PDF to an image and process it.

3. **Analyze the Resume:**

   - **Tell Me About the Resume:** Click this button to get a professional evaluation of the resume in relation to the provided job description.
   - **Percentage Match:** Click this button to get a percentage match of the resume against the job description, including keywords missing and an overall assessment.

4. **View Results:**

   The AI-generated responses, including the evaluation and match percentage, will be displayed in the Streamlit interface.

## File Structure

```bash
├── app.py                # Main Streamlit application
├── requirements.txt      # Python dependencies
├── .env                  # Environment variables
├── README.md             # Project documentation
└── src/
    ├── utils.py          # Utility functions (if applicable)
    └── ...               # Additional modules and scripts
```

## Dependencies

- **Streamlit:** For creating the web interface.
- **google-generativeai:** To leverage Google Generative AI for text analysis.
- **python-dotenv:** For managing environment variables securely.
- **pdf2image:** For converting PDF files to images.
- **Pillow (PIL):** For handling image processing in Python.

## Contributing

Contributions are welcome! Please fork this repository and submit a pull request with your changes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Contact

For any inquiries or feedback, please contact [your-email@example.com](mailto:your-email@example.com).

```

This `README.md` should cover the essential details of your project and guide users through setup and usage. If you have any other specific details or features you'd like to include, feel free to add them!
