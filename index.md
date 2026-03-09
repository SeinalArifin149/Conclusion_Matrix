# Conclusion Matrix

Ini adalah buku tentang **Confusion Matrix** dalam Machine Learning. 
Sering kali evaluasi model hanya berfokus pada nilai **akurasi**, padahal akurasi saja tidak selalu cukup untuk memahami performa model secara menyeluruh. 

Dengan menggunakan Confusion Matrix, kita dapat melihat bagaimana model melakukan klasifikasi secara lebih detail, seperti berapa banyak prediksi yang benar maupun yang salah pada setiap kelas.

## Pengertian

Confusion Matrix adalah metode evaluasi yang digunakan untuk mengukur kinerja model klasifikasi. 
Metode ini menampilkan perbandingan antara **label sebenarnya (actual)** dengan **label hasil prediksi model (predicted)**.

Komponen utama dalam Confusion Matrix meliputi:

- **True Positive (TP)** → Model memprediksi positif dan hasilnya memang positif.
- **True Negative (TN)** → Model memprediksi negatif dan hasilnya memang negatif.
- **False Positive (FP)** → Model memprediksi positif tetapi sebenarnya negatif.
- **False Negative (FN)** → Model memprediksi negatif tetapi sebenarnya positif.

Dengan melihat nilai-nilai tersebut, kita dapat menghitung berbagai metrik evaluasi seperti **accuracy, precision, recall, dan F1-score**.

---

## Pengecekan Akurasi dengan 2 Fitur

Pada percobaan pertama, model klasifikasi menggunakan **2 fitur** dari dataset sebagai variabel input. 
Fitur ini digunakan untuk melatih model agar dapat memprediksi kelas target.

Dengan jumlah fitur yang terbatas, model mungkin belum mampu menangkap pola data secara maksimal. 
Hal ini dapat menyebabkan nilai akurasi yang diperoleh masih relatif rendah atau model melakukan kesalahan prediksi pada beberapa data.

Namun, percobaan ini penting untuk melihat **baseline performa model** sebelum menambahkan fitur lain.

---

## Pengecekan Akurasi dengan 3 Fitur

Pada percobaan kedua, jumlah fitur yang digunakan ditingkatkan menjadi **3 fitur**. 
Penambahan fitur ini bertujuan untuk memberikan lebih banyak informasi kepada model sehingga model dapat mempelajari pola data dengan lebih baik.

Dengan adanya tambahan fitur, model biasanya akan menunjukkan peningkatan performa. 
Nilai akurasi dapat meningkat karena model memiliki lebih banyak variabel yang dapat digunakan untuk membedakan antar kelas.

Namun, peningkatan fitur juga harus diperhatikan agar tidak menyebabkan **overfitting**, yaitu kondisi di mana model terlalu menyesuaikan diri dengan data training.

---

## Pengecekan Akurasi dengan 4 Fitur

Pada percobaan ketiga, model menggunakan **4 fitur** sebagai variabel input. 
Dengan semakin banyak fitur yang digunakan, model memiliki lebih banyak informasi untuk melakukan proses klasifikasi.

Jika fitur yang ditambahkan memang relevan terhadap target klasifikasi, maka performa model dapat meningkat dan hasil Confusion Matrix akan menunjukkan lebih banyak prediksi yang benar.

Namun, tidak semua penambahan fitur selalu meningkatkan performa model. 
Beberapa fitur mungkin tidak memberikan kontribusi yang signifikan atau bahkan dapat menurunkan akurasi jika mengandung noise.

Oleh karena itu, analisis menggunakan Confusion Matrix sangat penting untuk melihat bagaimana perubahan jumlah fitur mempengaruhi hasil prediksi model.