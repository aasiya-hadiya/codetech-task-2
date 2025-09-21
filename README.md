

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

