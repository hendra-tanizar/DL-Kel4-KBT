# Prediksi Indeks Standar Pencemar Udara (ISPU) dengan Metode LSTM (Long Short Term Memory Network) berbasis Website
Oleh kelompok 4:
- Alvinus Yodi (203400010)
- Yulius Dani Eko Saputro (203400012)
- Hendra (203400013)
- Yosef Alfredo Khawarga (19340004)

Kelompok kami membangun aplikasi dengan menerapkan salah satu metode dari deep learning, yakni metode LSTM untuk mengerjakan prediksi indeks kualitas udara berdasarkan lokasi real-time pengguna dan input kota tujuan pengguna.
- Aplikasi menggunakan metode LSTM dan dataset informasi indeks kualitas udara dari 34 provinsi di Indonesia yang memuat sebanyak 98.055 data.
- Menggunakan WEATHERBIT API agar prediksi dapat dilakukan secara real-time dan dikonfigurasi melalui environment variable. API bekerja dengan mengakses data meteorologi untuk memperoleh informasi parameter dalam polutan udara secara real-time, dan data tersebut dibawa ke dalam prediksi dengan model LSTM untuk memperoleh angka indeks kualitas udara beserta kategorinya.
- Menggunakan titik koordinat untuk dapat memprediksi indeks kualitas udara berdasarkan input kota tujuan yang ingin dicari tahu oleh pengguna.
- Variabel parameter terbagi menjadi: PM10, PM2.5, O3, NO2, SO2, dan CO.
- Adapun dependency yang digunakan, yakni library dalam model, scikit-learn, Tensorflow untuk deep learning, dan juga Flask.
- Menggunakan framework Flask Python dalam pengembangan aplikasi berbasis website.

Hasil pada model yang telah di-training:
1. Nilai MAPE pada fitur diperoleh <20% yang menandakan kinerja prediksi pada fitur relatif akurat, kecuali pada fitur O3 (ozon) dengan nilai MAPE >50% yang berarti kinerja pada
   fitur tersebut kurang akurat dibandingkan dengan fitur polutan lain.
2. Fitur polutan CO memiliki nilai RMSE 297.48 yang berarti nilai RMSE yang tinggi.
3. Dari model LSTM yang digunakan untuk prediksi, diperoleh bahwa memungkinkan akan adanya peningkatan pada kinerja beberapa fitur terlebih pada O3, PM2.5, dan PM10 untuk
   meningkatkan akurasi prediksi indeks kualitas udara.
