# Classification of Grapevine Leaves using CNN for Identification Disease on Grapevine Leaves
Pada program ini mengimplementasikan arsitektur CNN (Convolutional Neural Network) dan transfer learning MobileNetV2 (pre-trained model) untuk melakukan klasifikasi gambar.

![General-CNN-layout-architecture-diagram](https://github.com/ndnfzr/visi-komputer-UAS/assets/148251636/c1ff4b3d-0405-4985-932a-a3759e00015f) 

**Data Preparation**

- Membuat dataset yang berisi gambar daun anggur yang mencakup berbagai kondisi dan variasinya. 
  Pada dataset ini menggunakan kondisi sebagai classnya yaitu *healthy* dan *unhealthy* sehingga terdapat 2 class.
- Bagi dataset menjadi 2 bagian antara lain untuk data pelatihan (*training*) dan data pengujian (*testing*).
- Menganotasikan gambar dengan memberikan bercak-bercak coklat untuk gambar daun *unhealthy* sebagai label yang nantinya akan menggambarkan
  apakah daun tersebut *healthy* atau *unhealthy*.

**Data Augmentation**

- Melakukan augmentasi data pada data pelatihan menggunakan beberapa teknik untuk membantu model lebih baik
  dalam generalisasi dan mengurangi overfitting.

**Model CNN**

- Mengklasifikasi gambar menggunakan rancang model CNN dengan menyesuaikan ukuran input model dengan gambar daun anggur.
- Menambahkan layer konvolusi, pooling, normalization, dan dense layer untuk membangun arsitektur model.

**Transfer Learning**

- Pre-trained model MobileNetV2 sebagai base model dan menambahkan layer kustom untuk proses klasifikasi secara spesifik.

**Compile Model**

- Memilih fungsi loss yang sesuai untuk klasifikasi multi-kelas.
- Menentukan optimizer seperti Adam atau SGD.
- Memilih metrik evaluasi seperti akurasi.

**Training Model**

- Melatih model pada data pelatihan menggunakan fungsi `fit` pada TensorFlow atau Keras.
- Memonitor performa model pada data validasi untuk memastikan tidak terjadi overfitting.

**Evaluasi dan Prediksi Model**

- Evaluasi model pada data pengujian untuk mengukur performa sebenarnya pada dataset.
- Menganalisis hasil evaluasi, termasuk akurasi dan metrik lainnya.
- Menggunakan model yang telah dilatih untuk membuat prediksi pada gambar daun anggur baru.

**Interpretasi Hasil**

- Menganalisis kelas sesuai hasil akurasi tiap gambar yang ditampilkan.
- Memvisualisasikan aktivasi layer untuk memahami bagian dari gambar yang penting bagi model dalam pengambilan keputusan.

Hasil dari data training

![download (1)](https://github.com/ndnfzr/visi-komputer-UAS/assets/148251636/538bd6c8-7d49-440e-8e6f-0acee3fc1dcb)


Hasil dari data test

![download (2)](https://github.com/ndnfzr/visi-komputer-UAS/assets/148251636/45f64757-5733-4ca9-9d76-53675666f8ad)



