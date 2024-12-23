
# About 🌐
### Tugas Mata Kuliah Riset Informatika
#### Nama : Andini Fitriyah Salsabilah  
#### NPM  : 21081010217

1. Tugas ini mencakup review beberapa penelitian berdasarkan jenisnya. Setiap review terdapat dalam folder berupa file dengan format PDF.
2. Tugas ini mencakup review 1 jurnal acuan yang ingin dijadikan paper.

## Review Jurnal Berdasarkan Jenisnya

### Jenis Penelitian Menurut Penggunaannya:

| No | Jenis Penelitian       | Link Jurnal                                          |
|----|-----------------------|-----------------------------------------------------|
| 1  | Pure Research         | [Link Jurnal](https://doi.org/10.1038/s41377-024-01451-z) |
| 2  | Applied Research      | [Link Jurnal](https://doi.org/10.1007/s00170-023-12864-2)  |

### Jenis Penelitian Menurut Metodenya:

| No | Jenis Penelitian       | Link Jurnal                                          |
|----|-----------------------|-----------------------------------------------------|
| 1  | Penelitian Historis   | [Link Jurnal](https://ojs.bonviewpress.com/index.php/AIA/article/view/689/580)                                     |
| 2  | Penelitian Filosofis   | [Link Jurnal](https://link.springer.com/article/10.1007/s11229-022-03999-y)                                     |
| 3  | Penelitian Observasional| [Link Jurnal](https://formative.jmir.org/2024/1/e54044/PDF)                                     |
| 4  | Penelitian Eksperimental| [Link Jurnal](https://arxiv.org/abs/2403.07183)                                     |

### Jenis Penelitian Menurut Sifat Permasalahannya:

| No | Jenis Penelitian           | Link Jurnal                                          |
|----|---------------------------|-----------------------------------------------------|
| 1  | Penelitian Historis       | [Link Jurnal](https://link.springer.com/article/10.1007/s13347-020-00405-8)                                     |
| 2  | Penelitian Deskriptif     | [Link Jurnal](https://doi.org/10.54373/imeij.v4i3.641)                                     |
| 3  | Penelitian Perkembangan   | [Link Jurnal](https://www.oarepo.org/index.php/oa/article/view/1870)                                     |
| 4  | Penelitian Korelasional   | [Link Jurnal](https://media.proquest.com/media/hms/PFT/1/KtoNW?_s=9Pu%2FkWuwB%2FVJvkKKo64rjTRNxxw%3D)                                     |
| 5  | Penelitian Kausal-Komparatif | [Link Jurnal](https://pubs.acs.org/doi/epdf/10.1021/acs.est.1c02204?ref=article_openPDF)                                  |
| 6  | Penelitian Eksperimental   | [Link Jurnal](https://doi.org/10.24929/jars.v2i1.2983)                                     |
| 7  | Penelitian Tindakan       | [Link Jurnal](https://dl.acm.org/doi/pdf/10.1145/3551624.3555285)                                     |

## 🟦 Review Jurnal Acuan

| No | Link Jurnal              |
|----|--------------------------|
| 1  | [Link Jurnal UTS](https://ieeexplore.ieee.org/document/10127792)          |

## ❓ Analisis Gap
#### Penelitian ini terbatas pada satu jenis model deep learning, yaitu CNN scratch dari awal, untuk mendeteksi hama pada tanaman caisim. Sedangkan bisa ditingkatkan akurasi prediksinya dengan mencoba metode yang lebih kompleks dan terbaru seperti VGG16, dll sehingga akurasinya lebih meningkat

### 🟦alternatif agar mendapatkan nilai akurasi yang lebih baik
1. Penerapan Transfer Learning dengan Model Pre-trained
Alih-alih membangun CNN dari awal, gunakan model yang telah dilatih sebelumnya seperti VGG16, ResNet, atau EfficientNet. Transfer learning memungkinkan model menggunakan pengetahuan yang telah dipelajari dari dataset besar seperti ImageNet, yang dapat meningkatkan akurasi dan generalisasi meskipun dataset terbatas.
Dengan fine-tuning model pre-trained ini, Anda bisa memanfaatkan fitur-fitur yang telah diekstraksi dan sesuaikan pada data hama caisim, sehingga tetap mencapai performa yang baik meskipun data terbatas.
2. Augmentasi Data untuk Memperbanyak Variasi Data
Terapkan augmentasi data untuk meningkatkan jumlah data latih secara virtual. Teknik augmentasi seperti rotasi, flipping, zooming, dan perubahan kontras atau kecerahan pada gambar dapat membantu model memahami variasi yang lebih luas dari data yang sama, sehingga membantu generalisasi.
Dengan augmentasi, Anda bisa meningkatkan jumlah sampel tanpa mengumpulkan data baru, yang dapat meningkatkan performa model dan meminimalkan overfitting pada dataset kecil.
3. Menggabungkan CNN dengan Algoritma Deteksi Objek seperti Faster R-CNN
Menggabungkan CNN dengan Faster R-CNN dapat meningkatkan deteksi yang lebih spesifik, yaitu dengan memberikan bounding box pada area yang terinfeksi hama. Ini tidak memerlukan data tambahan tetapi akan menambah kemampuan model untuk mendeteksi dan menunjukkan lokasi yang terinfeksi secara langsung.
Faster R-CNN dengan backbone seperti VGG16 dapat diterapkan pada dataset caisim untuk memberikan informasi lebih lanjut tentang area spesifik yang terkena hama, yang sangat berguna dalam aplikasi lapangan.
4. Penerapan Metode Ensemble untuk Meningkatkan Akurasi
Anda dapat menggunakan metode ensemble yang menggabungkan hasil dari beberapa model (misalnya CNN, VGG16, dan Faster R-CNN). Dengan cara ini, prediksi akhir bisa didasarkan pada voting atau rata-rata dari output berbagai model, yang sering kali meningkatkan akurasi dan ketahanan terhadap kesalahan pada data yang terbatas.
Metode ensemble ini tidak mengharuskan Anda memiliki dataset yang lebih besar, tetapi dapat memaksimalkan pemanfaatan dataset yang ada dengan memanfaatkan kekuatan berbagai model sekaligus.
5. Penggunaan Teknik Regularisasi untuk Mengurangi Overfitting
Pada dataset kecil, overfitting menjadi masalah yang umum. Anda bisa menerapkan dropout, early stopping, atau regularisasi L2 untuk meningkatkan kemampuan generalisasi model. Teknik ini akan membantu model untuk tidak terlalu terpaku pada data latih yang terbatas dan dapat menghasilkan performa yang lebih baik saat diuji pada data baru.
6. Validasi Silang (Cross-Validation) untuk Optimasi Model
Gunakan teknik k-fold cross-validation untuk mengoptimalkan model pada dataset kecil. Dengan membagi dataset menjadi beberapa fold dan melatih model secara bergantian, Anda dapat memastikan bahwa model tidak hanya terbatas pada satu subset data dan lebih tahan terhadap variasi.

### 🔸Judul Paper dari alternatif paper acuan
"Comparative Analysis of CNN with VGG16, and Xception Models for Pest Detection and Harvest Readiness Prediction in Caisim Leaves"
### 🔸Link Presentasi 
[Link presentasil]([https://dl.acm.org/doi/pdf/10.1145/3551624.3555285](https://drive.google.com/file/d/1fs4C5DDiw9XPvKXg28yA5k59HXhT7Tdq/view?usp=sharing))                                     |


