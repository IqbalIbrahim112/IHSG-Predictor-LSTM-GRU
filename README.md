# Prediksi IHSG dengan LSTM dan GRU

Repositori ini berisi proyek prediksi **Indeks Harga Saham Gabungan (IHSG)** menggunakan dua arsitektur deep learning: **Long Short-Term Memory (LSTM)** dan **Gated Recurrent Unit (GRU)**. Proyek ini merupakan bagian dari penelitian yang dipresentasikan dalam **Seminar Nasional**.

## 📊 Dataset

Dataset yang digunakan adalah data historis harian IHSG dari **1 Januari 2015 hingga 16 Mei 2025**, terdiri atas:
- `Date` – Tanggal perdagangan
- `Price` – Harga penutupan IHSG

Data telah diurutkan berdasarkan waktu dan dinormalisasi sebelum digunakan untuk pelatihan model.

## 🧠 Tujuan Penelitian

Penelitian ini bertujuan untuk membandingkan performa model **LSTM dan GRU** dalam memprediksi harga IHSG berdasarkan pergerakan 60 hari sebelumnya. Evaluasi performa dilakukan menggunakan metrik:
- **Mean Absolute Percentage Error (MAPE)**

## 🔍 Hasil Ringkas

| Model | Konfigurasi Neuron | Batch Size | MAPE    |
|-------|--------------------|------------|---------|
| LSTM  | 64–64              | 32         | 1.81%   |
| GRU   | 32–32              | 32         | **1.68%** |

Model GRU dengan konfigurasi 32–32 neuron dan batch size 32 menghasilkan akurasi terbaik dengan MAPE terendah.

## 📁 Struktur Folder

- `artikel/` – Artikel ilmiah dalam format PDF
- `data/` – Dataset historis IHSG (`ihsg.csv`)
- `src/` – Script Python untuk preprocessing, pelatihan model, dan evaluasi

## ⚙️ Cara Menjalankan

1. Clone repositori:
   ```bash
   git clone https://github.com/username/ihsg-prediction-lstm-gru.git
   cd ihsg-prediction-lstm-gru
