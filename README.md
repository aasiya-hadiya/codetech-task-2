Name: AASIYA HADIYA

Company: CODEC TECHNOLOGIES

ID: E19E86-0116588288923

Designation: Python Developer Intern

Duration: 01/09/2025 to 01/10/2025

# Resume Parsing Web Application

A powerful and user-friendly **Resume Parsing** web app built with **Python**, leveraging **SpaCy’s NER model** for extracting structured information from resumes in PDF and DOCX formats. The app uses **Flask** for web deployment and stores parsed data into a **MySQL database** for easy access and management.

---

## Features

- Upload resumes in **PDF** or **DOCX** format  
- Extract key information such as:  
  - Name  
  - Date of Birth  
  - Phone Number  
  - Email  
  - Location  
  - Education details  
  - University  
  - Previous companies worked at  
  - Primary skills  
  - Secondary skills  
- Store parsed data securely in a MySQL database  
- Simple and intuitive web interface powered by Flask  

---

## Technologies Used

- **Python** for backend processing  
- **SpaCy** for Named Entity Recognition (NER) to identify resume details  
- **Flask** for web server and routing  
- **MySQL** for storing extracted information  
- **docx2txt** and **PyMuPDF (fitz)** for extracting text from DOCX and PDF files respectively  

---

## Setup Instructions

### 1. Clone the Repository

```bash
git clone <your-repo-url>
cd <your-repo-folder>


## Setup Instructions

### 2. Install Dependencies

  Make sure you have Python installed (preferably version 3.7 or higher), then install all required packages by running:

  ```bash
  pip install -r requirements.txt

3. Prepare the SpaCy Model

  Train your custom SpaCy NER model on labeled resume data (or use the provided model named my_model)

  Place the trained model in the project directory

4. Configure MySQL Database

  Set up a MySQL database named mydatabase

  Update database connection credentials in the code (host, user, password) if necessary

  Create the table api_test with columns matching the extracted fields (NAME, DOB, PHONENO, EMAIL, LOCATION, EDUCATION, UNIVERSITY, COMPANIES, PRIMARY_SKILLS, SECONDARY_SKILLS)

5. Run the Application

  Start the Flask app locally:

  python main.py


##How It Works:

  Upload a resume file (PDF or DOCX) through the web interface

  The app extracts the textual content using fitz (for PDFs) or docx2txt (for DOCX)

  Text is processed by the SpaCy NER model to detect entities relevant to resumes

  Extracted details are cleaned, deduplicated, and converted into a structured format

  The parsed information is saved into the MySQL database for future reference

