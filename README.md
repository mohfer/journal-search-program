# 📚 Journal Search Program

This program enables searching for academic journals using **Linear Search** and **Binary Search** algorithms. Designed as a Data Structures course project, the application provides a command-line interface to search for journals by **title**, **publication year**, or **author name**.

---

## 📝 Description

The Journal Search Program retrieves data from a CSV file specified through environment variables (`.env`) and offers the following search methods:

### 🔍 Search Methods
1. **Linear Search**  
    Searches sequentially from beginning to end.
2. **Binary Search**  
    Uses binary search algorithm — requires pre-sorted data.

---

## ⚙️ System Requirements

- Python 3.8 or newer
- Required packages:
  - `pandas` (version 2.2.3)
  - `python-dotenv` (version 1.0.0)

---

## 🛠️ Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/mohfer/journal-search-program.git
    cd journal-search-program
    ```

2. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Copy `.env.example` to `.env`:
    ```bash
    cp .env.example .env
    ```

4. Update the Google Sheets ID in the `.env` file:
    ```
    URL=https://docs.google.com/spreadsheets/d/{id}/export?format=csv
    ```
    Replace `{id}` with your actual Google Sheet ID.

---

## 🚀 Usage

Run the program with:
```bash
python main.py
```

Follow the terminal prompts:

1. Select search method (Linear or Binary)
2. Choose search criteria (Title, Year, or Author)
3. Enter your search keyword

---

## 📄 Supported CSV Format

The CSV file must have the following column structure:

| Column Name |
|-------------|
| No |
| NIM |
| Nama Mahasiswa |
| Sumber Database |
| Fokus kata kunci (No. 1/2/3 sesuai soal) |
| Judul Paper |
| Tahun Terbit |
| Nama Penulis |
| Abstrak |
| Kesimpulan |
| Link Paper |

---

## ✨ Features

- Loading animation when retrieving data
- Text formatting for cleaner display
- Error handling during data retrieval
- Support for linear and binary search
- Clean search results display

---

## ⚠️ Notes

- Binary search only supports **exact match** keywords and is best used for **single words**
- Linear search supports **partial** matches in the selected column
- Ensure the CSV URL is accessible from your network
