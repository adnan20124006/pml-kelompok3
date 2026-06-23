# Prediksi Curah Hujan Kota Bandun

Proyek ini bertujuan untuk membangun model machine learning (Time Series Forecasting atau Regresi) untuk memprediksi jumlah curah hujan bulanan di wilayah Kota Bandung. Proyek ini menggunakan data historis resmi resmi dari Badan Meteorologi, Klimatologi, dan Geofisika (BMKG) yang dirilis secara tahunan.

## 📌 Struktur Proyek

Proyek ini menggunakan struktur standar _Cookiecutter Data Science_:

```text
├── LICENSE
├── Makefile           <- Perintah otomatisasi seperti `make data` atau `make train`
├── README.md          <- Penjelasan utama proyek (File ini)
├── data
│   ├── external       <- Data pihak ketiga pendukung (jika ada)
│   ├── interim        <- Data hasil transformasi awal (misal: encoding nama bulan)
│   ├── processed      <- Data final yang siap dimodelkan (`curah_hujan_bandung_clean.csv`)
│   └── raw            <- File asli: `curah_hujan_di_kota_bandung_2.csv` (immutable)
├── docs               <- Dokumentasi proyek (Sphinx)
├── models             <- File model terlatih (.pkl, .h5) dan metrik evaluasi
├── notebooks          <- Jupyter notebooks untuk eksperimen (Format: [Nomor]-[Inisial]-[Deskripsi])
├── references         <- Dokumen metadata pendukung (`curah_hujan_di_kota_bandung_2_metadata.pdf`)
├── reports            <- Hasil analisis berupa HTML, PDF, atau visualisasi tren hujan
│   └── figures        <- Grafik curah hujan tahunan/bulanan untuk laporan
├── requirements.txt   <- Daftar library Python untuk mereproduksi environment
├── setup.py           <- Membuat modul `src` bisa di-import (pip install -e .)
├── src                <- Source code utama proyek
│   ├── __init__.py
│   ├── data           <- Script pembersihan data (`make_dataset.py`)
│   ├── features       <- Script rekayasa fitur / pembuatan lag features (`build_features.py`)
│   ├── models         <- Script pelatihan dan prediksi (`train_model.py`, `predict_model.py`)
│   └── visualization  <- Script visualisasi tren curah hujan (`visualize.py`)
└── tox.ini            <- Pengaturan otomatisasi pengujian dengan tox
```
