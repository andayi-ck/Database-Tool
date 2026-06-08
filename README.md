# Database-Tool
# 📂 Local Document Management & Automated Reporting Engine

A full-stack, local web application that automates business reporting and paperless document ingestion. This tool allows users to run complex, predefined database queries to generate downloadable Excel sheets and integrates an OCR pipeline to digitize scanned physical documents into a searchable database.


---

## 🚀 Key Features

- **Automated Reporting:** Execute parameterized database queries via a secure dropdown UI with zero SQL injection risk.
- **Excel Export Engine:** Dynamically processes raw database rows into clean, structured, and native Excel formats (`.xlsx`).
- **Paperless OCR Ingestion:** Uploads scanned images or PDFs, extracts text automatically using Optical Character Recognition, and indexes the text for search.
- **Hybrid Storage Architecture:** Saves physical soft copies to an isolated local directory while storing lightweight metadata and searchable content inside the database.

---

## 🛠️ Tech Stack

- **Frontend / UI:** Streamlit
- **Backend Core:** Python (v3.10+)
- **Data Engineering:** Pandas, NumPy, OpenPyXL
- **Database Engine:** SQLite (Local Relational Database)
- **Computer Vision / OCR:** Tesseract OCR (PyTesseract)

---

## ⚙️ Architecture & Data Flow

```text
[User Web UI] ──────► 1. Run Predefined Query ──────► [Pandas DataFrame] ──► [Excel Download]
              ──────► 2. Upload Scan (Image/PDF) ───► [Tesseract OCR]
                                                             │
                                     ┌───────────────────────┴───────────────────────┐
                                     ▼ (Save File URL & Text)                        ▼ (Save File Binary)
                           [Local SQLite Database]                        [Local Object Storage Folder]
```

---

## 💻 Local Installation & Setup

Follow these steps to set up and run this application on your local computer (`localhost`).

### 1. Prerequisites
- **Python:** Ensure Python 3.10 or higher is installed on your machine.
- **Tesseract OCR Engine:**
  - **Mac:** Run `brew install tesseract` via Homebrew.
  - **Windows:** Download the binary installer from GitHub (e.g., UB-Mannheim) and add Tesseract to your System PATH variables.

### 2. Clone the Repository
```bash
git clone https://github.com[YOUR_GITHUB_USERNAME]/[YOUR_REPOSITORY_NAME].git
cd [YOUR_REPOSITORY_NAME]
```

### 3. Initialize a Virtual Environment
Isolate the project dependencies from your global computer workspace:
```bash
# Windows
python -m venv venv
venv\Scripts\activate

# Mac/Linux
python -m venv venv
source venv/bin/activate
```

### 4. Install Dependencies
```bash
pip install streamlit pandas sqlalchemy openpyxl pytesseract pillow
```

### 5. Boot Up the Application
Launch the local web server:
```bash
streamlit run app.py
```
The browser will automatically open your web app at `http://localhost:8501`.

---

## 📊 Database Schema Design

The application automatically initializes a local relational SQLite database (`local_app.db`) on its first run with the following structures:

- **`sales` Table:** Manages mock business transactions (ID, Item, Amount, Category, Date) for Excel export testing.
- **`documents` Table:** Manages the DMS metadata (ID, Doc_Name, File_Path, Extracted_Text).

---

## 👨‍💻 Developer Profile

Built by Enoch W.Magero
- **LinkedIn: # 📂 Local Document Management & Automated Reporting Engine

A full-stack, local web application that automates business reporting and paperless document ingestion. This tool allows users to run complex, predefined database queries to generate downloadable Excel sheets and integrates an OCR pipeline to digitize scanned physical documents into a searchable database.

---

## 🚀 Key Features

- **Automated Reporting:** Execute parameterized database queries via a secure dropdown UI with zero SQL injection risk.
- **Excel Export Engine:** Dynamically processes raw database rows into clean, structured, and native Excel formats (`.xlsx`).
- **Paperless OCR Ingestion:** Uploads scanned images or PDFs, extracts text automatically using Optical Character Recognition, and indexes the text for search.
- **Hybrid Storage Architecture:** Saves physical soft copies to an isolated local directory while storing lightweight metadata and searchable content inside the database.

---

## 🛠️ Tech Stack

- **Frontend / UI:** Streamlit
- **Backend Core:** Python (v3.10+)
- **Data Engineering:** Pandas, NumPy, OpenPyXL
- **Database Engine:** SQLite (Local Relational Database)
- **Computer Vision / OCR:** Tesseract OCR (PyTesseract)

---

## ⚙️ Architecture & Data Flow

```text
[User Web UI] ──────► 1. Run Predefined Query ──────► [Pandas DataFrame] ──► [Excel Download]
              ──────► 2. Upload Scan (Image/PDF) ───► [Tesseract OCR]
                                                             │
                                     ┌───────────────────────┴───────────────────────┐
                                     ▼ (Save File URL & Text)                        ▼ (Save File Binary)
                           [Local SQLite Database]                        [Local Object Storage Folder]
```

---

## 💻 Local Installation & Setup

Follow these steps to set up and run this application on your local computer (`localhost`).

### 1. Prerequisites
- **Python:** Ensure Python 3.10 or higher is installed on your machine.
- **Tesseract OCR Engine:**
  - **Mac:** Run `brew install tesseract` via Homebrew.
  - **Windows:** Download the binary installer from GitHub (e.g., UB-Mannheim) and add Tesseract to your System PATH variables.

### 2. Clone the Repository
```bash
git clone https://github.com[YOUR_GITHUB_USERNAME]/[YOUR_REPOSITORY_NAME].git
cd [YOUR_REPOSITORY_NAME]
```

### 3. Initialize a Virtual Environment
Isolate the project dependencies from your global computer workspace:
```bash
# Windows
python -m venv venv
venv\Scripts\activate

# Mac/Linux
python -m venv venv
source venv/bin/activate
```

### 4. Install Dependencies
```bash
pip install streamlit pandas sqlalchemy openpyxl pytesseract pillow
```

### 5. Boot Up the Application
Launch the local web server:
```bash
streamlit run app.py
```
The browser will automatically open your web app at `http://localhost:8501`.

---

## 📊 Database Schema Design

The application automatically initializes a local relational SQLite database (`local_app.db`) on its first run with the following structures:

- **`sales` Table:** Manages mock business transactions (ID, Item, Amount, Category, Date) for Excel export testing.
- **`documents` Table:** Manages the DMS metadata (ID, Doc_Name, File_Path, Extracted_Text).

---

## 👨‍💻 Developer Profile

Built by **[Your Full Name]**  
- **LinkedIn:# 📂 Local Document Management & Automated Reporting Engine

A full-stack, local web application that automates business reporting and paperless document ingestion. This tool allows users to run complex, predefined database queries to generate downloadable Excel sheets and integrates an OCR pipeline to digitize scanned physical documents into a searchable database.

---

## 🚀 Key Features

- **Automated Reporting:** Execute parameterized database queries via a secure dropdown UI with zero SQL injection risk.
- **Excel Export Engine:** Dynamically processes raw database rows into clean, structured, and native Excel formats (`.xlsx`).
- **Paperless OCR Ingestion:** Uploads scanned images or PDFs, extracts text automatically using Optical Character Recognition, and indexes the text for search.
- **Hybrid Storage Architecture:** Saves physical soft copies to an isolated local directory while storing lightweight metadata and searchable content inside the database.

---

## 🛠️ Tech Stack

- **Frontend / UI:** Streamlit
- **Backend Core:** Python (v3.10+)
- **Data Engineering:** Pandas, NumPy, OpenPyXL
- **Database Engine:** SQLite (Local Relational Database)
- **Computer Vision / OCR:** Tesseract OCR (PyTesseract)

---

## ⚙️ Architecture & Data Flow

```text
[User Web UI] ──────► 1. Run Predefined Query ──────► [Pandas DataFrame] ──► [Excel Download]
              ──────► 2. Upload Scan (Image/PDF) ───► [Tesseract OCR]
                                                             │
                                     ┌───────────────────────┴───────────────────────┐
                                     ▼ (Save File URL & Text)                        ▼ (Save File Binary)
                           [Local SQLite Database]                        [Local Object Storage Folder]
```

---

## 💻 Local Installation & Setup

Follow these steps to set up and run this application on your local computer (`localhost`).

### 1. Prerequisites
- **Python:** Ensure Python 3.10 or higher is installed on your machine.
- **Tesseract OCR Engine:**
  - **Mac:** Run `brew install tesseract` via Homebrew.
  - **Windows:** Download the binary installer from GitHub (e.g., UB-Mannheim) and add Tesseract to your System PATH variables.

### 2. Clone the Repository
```bash
git clone https://github.com[YOUR_GITHUB_USERNAME]/[YOUR_REPOSITORY_NAME].git
cd [YOUR_REPOSITORY_NAME]
```

### 3. Initialize a Virtual Environment
Isolate the project dependencies from your global computer workspace:
```bash
# Windows
python -m venv venv
venv\Scripts\activate

# Mac/Linux
python -m venv venv
source venv/bin/activate
```

### 4. Install Dependencies
```bash
pip install streamlit pandas sqlalchemy openpyxl pytesseract pillow
```

### 5. Boot Up the Application
Launch the local web server:
```bash
streamlit run app.py
```
The browser will automatically open your web app at `http://localhost:8501`.

---

## 📊 Database Schema Design

The application automatically initializes a local relational SQLite database (`local_app.db`) on its first run with the following structures:

- **`sales` Table:** Manages mock business transactions (ID, Item, Amount, Category, Date) for Excel export testing.
- **`documents` Table:** Manages the DMS metadata (ID, Doc_Name, File_Path, Extracted_Text).

---

## 👨‍💻 Developer Profile

Built by: Enoch W.Magero
- LinkedIn: https://www.linkedin.com/in/w-enoch-magero-535a1a256/
- Portfolio / Email: magero833@gmail.com 
