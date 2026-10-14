# Computer Vision Projects

Kumpulan tugas project mata kuliah Computer Vision.

## Project 1: Komparasi Arsitektur CNN

Klasifikasi label Female/Male pada dataset CelebA menggunakan AlexNet, VGG16, VGG19, GoogLeNet, dan ResNet18. Setiap model memakai 20.000 gambar training, 5.000 validasi, dan 5.000 test, dengan 8 epoch, batch size 64, serta learning rate 0,0001.

| Model | Akurasi test | Macro F1 |
|---|---:|---:|
| AlexNet | 97,36% | 97,29% |
| VGG16 | 98,52% | 98,48% |
| VGG19 | 98,42% | 98,38% |
| GoogLeNet | 97,94% | 97,89% |
| ResNet18 | 98,18% | 98,13% |

Evaluasi menggunakan confusion matrix, precision, recall, dan F1-score. VGG16 menghasilkan akurasi tertinggi pada run ini.

[Notebook dan laporan](Tugas-Project-1/README.md) · [Google Sheets](https://docs.google.com/spreadsheets/d/1U9UvMD9tMa8L96QBRixhuX88JTluqr22j_ciP7C4yEc/edit) · [Presentasi](https://docs.google.com/presentation/d/1MvVJFpfq--ksOoStYSwD1KPhrXRRtPiTfCH3ylXyhvA/edit)

Notebook memuat output eksperimen. Dataset dan bobot model tidak disertakan.
