# Project 1: Komparasi Arsitektur CNN

Perbandingan lima model untuk klasifikasi Female/Male menggunakan [dataset CelebA dari Kaggle](https://www.kaggle.com/datasets/ashishjangra27/gender-recognition-200k-images-celeba).

Data yang digunakan: 20.000 training, 5.000 validasi, dan 5.000 test. Konfigurasi bersama: seed 42, 8 epoch, batch size 64, learning rate 0,0001, Adam, CrossEntropyLoss, input 224 × 224 piksel, dan bobot awal ImageNet. Output runtime mencatat GPU Tesla T4.

| Model | Notebook | Akurasi test | Macro F1 | Training (menit) |
|---|---|---:|---:|---:|
| AlexNet | [Buka](notebooks/AlexNet.ipynb) | 97,36% | 97,29% | 13,0 |
| VGG16 | [Buka](notebooks/VGG16.ipynb) | 98,52% | 98,48% | 25,7 |
| VGG19 | [Buka](notebooks/VGG19.ipynb) | 98,42% | 98,38% | 30,0 |
| GoogLeNet | [Buka](notebooks/GoogLeNet.ipynb) | 97,94% | 97,89% | 15,3 |
| ResNet18 | [Buka](notebooks/ResNet18.ipynb) | 98,18% | 98,13% | 14,5 |

Evaluasi test memakai checkpoint dengan akurasi validasi tertinggi, confusion matrix, dan classification report. VGG16 unggul pada akurasi test dalam run ini. ResNet18 mencapai 98,18% dengan waktu training 14,5 menit. Hasil berasal dari satu run per model.

## Laporan

- [Google Sheets komparasi](https://docs.google.com/spreadsheets/d/1U9UvMD9tMa8L96QBRixhuX88JTluqr22j_ciP7C4yEc/edit) / [XLSX](reports/Komparasi_CNN_CelebA.xlsx)
- [Google Slides presentasi](https://docs.google.com/presentation/d/1MvVJFpfq--ksOoStYSwD1KPhrXRRtPiTfCH3ylXyhvA/edit) / [PPTX](reports/Presentasi_Komparasi_CNN_CelebA.pptx)
- [Spreadsheet tambahan dari tahap sebelumnya](reports/CNN_Experiment_Comparison.xlsx)

Notebook menyertakan hasil training, confusion matrix, dan contoh prediksi. Bobot model dan dataset tidak disertakan. Token Kaggle pada salinan notebook disamarkan.
