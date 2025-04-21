# 📚 Journal Search Program

Program ini memungkinkan pencarian jurnal akademik menggunakan algoritma **Linear Search** dan **Binary Search**. Dirancang sebagai proyek mata kuliah Struktur Data, aplikasi ini menyediakan antarmuka baris perintah untuk mencari jurnal berdasarkan **judul**, **tahun terbit**, atau **nama penulis**.

---

## 📝 Deskripsi

Journal Search Program mengambil data dari file CSV yang ditentukan melalui variabel lingkungan (`.env`) dan menyediakan pilihan metode pencarian:

### 🔍 Metode Pencarian
1. **Linear Search**  
   Mencari secara berurutan dari awal hingga akhir.
2. **Binary Search**  
   Menggunakan algoritma pencarian biner — membutuhkan data yang sudah terurut.

---

## ⚙️ Kebutuhan Sistem

- Python 3.8 atau lebih baru
- Paket yang dibutuhkan:
  - `pandas` (versi 2.2.3)
  - `python-dotenv` (versi 1.0.0)

---

## 🛠️ Instalasi

1. Clone repository:
   ```bash
   git clone <repository-url>
   cd search-program
   ```

2. Install dependensi:
   ```bash
   pip install -r requirements.txt
   ```

3. Salin file `.env.example` menjadi `.env`:
   ```bash
   cp .env.example .env
   ```

---

## 🚀 Penggunaan

Jalankan program dengan:
```bash
python main.py
```

Ikuti petunjuk di terminal:

1. Pilih metode pencarian (Linear atau Binary)
2. Pilih kriteria pencarian (Judul, Tahun, atau Penulis)
3. Masukkan kata kunci yang ingin dicari

---

## 📄 Format CSV yang Didukung

CSV yang digunakan harus memiliki struktur kolom sebagai berikut:

| Nama Kolom | Deskripsi | Tipe |
|------------|-----------|------|
| No | Nomor urut | Integer |
| NIM | NIM Mahasiswa | String |
| Nama Mahasiswa | Nama Mahasiswa | String |
| Sumber Database | Nama database | String |
| Fokus Kata Kunci | Fokus kata kunci (No. 1/2/3 sesuai soal) | String |
| Judul Paper | Judul Jurnal | String |
| Tahun Terbit | Tahun terbit | String/Integer |
| Nama Penulis | Nama penulis | String |
| Abstrak | Abstrak jurnal | Text |
| Kesimpulan | Kesimpulan jurnal | Text |
| Link Paper | URL ke jurnal | String |

---

## ✨ Fitur

- Animasi loading saat mengambil data
- Formatting teks untuk tampilan yang lebih rapi
- Penanganan error saat pengambilan data
- Dukungan untuk pencarian linear dan biner
- Tampilan hasil pencarian yang bersih

---

## ⚠️ Catatan

- Binary search hanya mendukung pencarian dengan kata kunci **tepat (exact match)** dan sebaiknya digunakan untuk **kata tunggal**
- Linear search mendukung pencarian **parsial** pada kolom yang dipilih
- Pastikan URL CSV dapat diakses dari jaringan Anda
