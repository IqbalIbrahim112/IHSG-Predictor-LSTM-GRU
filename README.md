# Prediksi IHSG dengan LSTM vs GRU

Proyek ini merupakan bagian dari artikel ilmiah berjudul **"Perbandingan Algoritma Long Short-Term Memory (LSTM) dan Gated Recurrent Unit (GRU) untuk Prediksi IHSG"** yang dipresentasikan dalam Seminar Nasional.

## 📄 Deskripsi Singkat

Penelitian ini membandingkan dua arsitektur deep learning, LSTM dan GRU, untuk memprediksi **Indeks Harga Saham Gabungan (IHSG)** berdasarkan data historis dari tahun 2015 hingga 2025. Evaluasi dilakukan menggunakan metrik **Mean Absolute Percentage Error (MAPE)**.

**Hasil utama:**
- GRU memberikan performa prediksi terbaik dengan MAPE **1.68%**
- LSTM terbaik mencetak MAPE **1.81%**

## 📁 Struktur Folder

- `artikel/`: File PDF artikel ilmiah
- `data/`: Dataset historis IHSG (jika tersedia)
- `src/`: Kode Python untuk preprocessing, training, dan evaluasi model
- `requirements.txt`: (Opsional) Library Python yang dibutuhkan

## ⚙️ Cara Menjalankan

1. Clone repo:
    ```bash
    git clone https://github.com/username/prediksi-ihsg-lstm-vs-gru.git
    cd prediksi-ihsg-lstm-vs-gru
    ```

2. Install library:
    ```bash
    pip install -r requirements.txt
    ```

3. Jalankan kode:
    ```bash
    python src/prediksi_ihsg.py
    ```

## 📚 Artikel

PDF lengkap bisa dilihat di folder [`/artikel`](./artikel).

## 📊 Hasil Singkat

| Model | Konfigurasi Neuron | Batch Size | MAPE    |
|-------|--------------------|------------|---------|
| LSTM  | 64–64              | 32         | 1.81%   |
| GRU   | 32–32              | 32         | **1.68%** |

## 📬 Kontak

Jika ada pertanyaan, silakan hubungi melalui email: [emailmu@domain.com]

