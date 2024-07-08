# Prediksi Indeks Standar Pencemar Udara (ISPU) dengan Metode LSTM berbasis Website
Anggota kelompok:
1. Hendra (203400013)
2. Alvinus Yodi (203400010)
3. Yulius Dani Eko Saputro (203400012)
4. Yosef Alfredo Khawarga (19340004)

Deskripsi Project:
- Project dibangun berbasis website.
- Aplikasi bertujuan untuk memberi hasil prediksi mengenai indeks kualitas udara, dan sekaligus menguji metode LSTM (Long Short Term Memory Network) yang merupakan salah satu metode deep learning dalam memberi prediksi.
- Data yang digunakan adalah dataset AQI (indeks kualitas udara) untuk 34 provinsi di Indonesia.
- Penerapan AI yakni dalam prediksi indeks kualitas udara melalui parameter yang diintegrasikan secara real-time berdasarkan lokasi, tanggal, dan waktu prediksi user.
- Parameter yang digunakan terdiri dari 6 kategori, diantaranya: PM10, PM2.5, O3 (ozon),  SO2 (sulfur dioksida), NO2 (nitrogen dioksida), CO (karbon monoksida).
- Kualitas Udara yang digunakan mengacu pada skor ISPU yang diperoleh dari konversi nilai konsentrasi dan terbagi menjadi 4 kategori, yakni: Baik, Sedang, Tidak sehat, Sangat tidak sehat
- Menggunakan framework deep learning yakni Tensorflow.
- Membaca dataset dari repository ini.

Hasil Training Model:
- Diukur melalui beberapa metrik, yakni RMSE, MSE, MAE, dan MAPE pada setiap fitur.
- RMSE (Root Mean Squared Error) digunakan untuk menghitung rata-rata dari kesalahan prediksi.
- MSE (Mean Squared Error) digunakan untuk menghitung rata-rata kuadrat dari kesalahan prediksi.
- MAE (Mean Absolute Error) digunakan untuk menghitung rata-rata nilai absolut dari kesalahan prediksi.
- MAPE (Mean Absolute Percentage Error) digunakan untuk menghitung rata-rata persentase dari kesalahan absolut.
1. Nilai MAPE pada fitur diperoleh <20% yang menandakan kinerja prediksi pada fitur relatif akurat, kecuali pada fitur O3 (ozon) dengan nilai MAPE >50% yang berarti kinerja pada fitur tersebut kurang akurat dibandingkan dengan fitur polutan lain.
2. Fitur polutan CO memiliki nilai RMSE 297.48 yang berarti nilai RMSE yang tinggi.
3. Dari model LSTM yang digunakan untuk prediksi, diperoleh bahwa memungkinkan akan adanya peningkatan pada kinerja beberapa fitur terlebih pada O3, PM2.5, dan PM10 untuk meningkatkan akurasi prediksi indeks kualitas udara.

Referensi tambahan:
https://silika.jakarta.go.id/udara
