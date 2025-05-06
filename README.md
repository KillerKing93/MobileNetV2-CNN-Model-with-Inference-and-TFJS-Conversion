# MobileNetV2-CNN-Model-with-Inference-and-TFJS-Conversion

Repositori ini berisi implementasi model Convolutional Neural Network (CNN)
berbasis MobileNetV2 untuk deteksi makanan Padang, beserta skrip inferensi
dan konversi model ke TensorFlow.js.

## Fitur

- Pelatihan model CNN menggunakan TensorFlow/Keras
- Skrip inferensi di Python (`DeteksiMakananCNN.ipynb`)
- Konversi model ke format TensorFlow.js (folder `model_tfjs`)
- Hasil inference dalam bentuk gambar (`inference_results.png`)
- Visualisasi proses pelatihan (`initial_training_results.png`)

## Struktur Direktori

```

├── model_keras
│ ├── final_padangfood_model.h5
│ └── final_padangfood_model.keras
├── model_tfjs
│ ├── group1-shard1of3.bin
│ ├── group1-shard2of3.bin
│ ├── group1-shard3of3.bin
│ └── model.json
├── padangfood_split
│ ├── train
│ ├── val
│ └── test
├── padangfood_staged
│ ├── ayam_goreng
│ ├── ayam_pop
│ ├── daging_rendang
│ ├── ... (kelas lainnya)
├── class_names.txt
├── DeteksiMakananCNN.ipynb
├── inference_results.png
└── initial_training_results.png

```

## Instalasi

1. **Clone repositori**
   ```bash
   git clone https://github.com/KillerKing93/MobileNetV2-CNN-Model-with-Inference-and-TFJS-Conversion.git
   cd MobileNetV2-CNN-Model-with-Inference-and-TFJS-Conversion
   ```

````

2. **Buat virtual environment & install dependencies**

   ```bash
   python3 -m venv venv
   source venv/bin/activate
   pip install -r requirements.txt
   ```

3. **Siapkan dataset**

   - Download dataset PadangFood dari Kaggle
     [https://www.kaggle.com/datasets/faldoae/padangfood](https://www.kaggle.com/datasets/faldoae/padangfood)
   - Ekstrak ke folder `padangfood_staged`

## Penggunaan

- **Training**
  Jalankan skrip training di notebook `DeteksiMakananCNN.ipynb`.

- **Inference (Python)**
  Buka dan jalankan sel pada `DeteksiMakananCNN.ipynb` untuk melihat
  hasil deteksi pada gambar contoh.

- **Inference (Web/TFJS)**

  - Buka folder `model_tfjs`, lalu integrasikan ke aplikasi web
    menggunakan TensorFlow\.js.
  - Contoh kode di `example_web_inference.html` (jika tersedia).

## Dataset

Dataset `padangfood_staged` berasal dari:

> Faldoae / PadangFood
> [https://www.kaggle.com/datasets/faldoae/padangfood](https://www.kaggle.com/datasets/faldoae/padangfood)

## Kontribusi

Selamat datang!

- Fork repositori ini
- Buat branch fitur baru (`git checkout -b feature/…`)
- Commit perubahan Anda (`git commit -m "…”`)
- Push ke branch (`git push origin feature/…`)
- Buka Pull Request

## Lisensi

Proyek ini dilisensikan di bawah **Apache License 2.0** dengan ketentuan
tambahan royalti untuk penggunaan komersial.
Lihat file [LICENSE](LICENSE) untuk detail.

## Kontak

- **Penulis**: Alif Nurhidayat
- **Email**: [alifnurhidayatwork@gmail.com](mailto:alifnurhidayatwork@gmail.com)
- **GitHub**: [https://github.com/KillerKing93/MobileNetV2-CNN-Model-with-Inference-and-TFJS-Conversion](https://github.com/KillerKing93/MobileNetV2-CNN-Model-with-Inference-and-TFJS-Conversion)

````
