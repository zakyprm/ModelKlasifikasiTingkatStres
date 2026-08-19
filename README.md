# Model Klasifikasi Tingkat Stres

Repository ini berisi source code dan sumber daya untuk model klasifikasi tingkat stres berbasis AI (bagian dari penelitian skripsi). Model ini dikembangkan menggunakan dataset kuesioner dengan pendekatan _Natural Language Processing_ (NLP) memanfaatkan IndoBERT untuk analisis dan klasifikasi.

## Struktur File Utama

- `klasifikasi.ipynb`: Jupyter Notebook utama yang berisi seluruh _pipeline_ sistem, mulai dari preprocessing data, training model, hingga evaluasi.
- `data_kusioner.csv`: Dataset utama yang berisi hasil kuesioner untuk melatih model.
- `hasil_evaluasi_final.csv` & `hasil_per_kelas.csv`: Ringkasan metrik evaluasi model akhir.
- `grafik_training_lengkap.png` & `confusion_matrix_final.png`: Visualisasi kurva training dan confusion matrix dari evaluasi akhir.
- `log_training_per_epoch.csv`: Catatan performa (loss dan accuracy) per iterasi epoch.
- `.gitignore`: Mengabaikan folder model berukuran besar (`indobert_hasil_skripsi/`, `model_final_skripsi/`) dan folder environment (`.venv/`) agar tidak melampaui batas kapasitas GitHub.

## Prasyarat

Pastikan beberapa library Python berikut telah terinstal sebelum menjalankan file notebook:
- `pandas`
- `numpy`
- `scikit-learn`
- `torch` (PyTorch)
- `transformers` (Hugging Face)
- `matplotlib` & `seaborn` (untuk visualisasi)

*(Sangat disarankan menggunakan virtual environment seperti `.venv` atau `conda`)*.

## Cara Penggunaan

1. Clone repository ini ke perangkat Anda:
   ```bash
   git clone https://github.com/zakyprm/ModelKlasifikasiTingkatStres.git
   cd ModelKlasifikasiTingkatStres
   ```
2. Jalankan jupyter notebook:
   ```bash
   jupyter notebook
   ```
3. Buka file `klasifikasi.ipynb` dan eksekusi setiap cell (Run All) secara berurutan untuk melihat langkah-langkah preprocessing dan hasil pelatihannya.
