# Klasifikasi-Kertas-Gunting-Batu-dengan-VGG19
1. Business Understanding
Dalam tahap ini, tujuan bisnis dari proyek adalah untuk mengklasifikasikan gambar-gambar tangan yang menggambarkan gunting, batu, atau kertas. Ini dapat digunakan dalam aplikasi permainan sederhana atau pengenalan gestur tangan untuk kontrol perangkat. Dataset telah dipersiapkan dengan membagi gambar-gambar ke dalam folder train dan validation, masing-masing dengan proporsi 60% dan 40%. Totalnya, ada 1314 gambar untuk pelatihan dan 874 gambar untuk validasi.

2. Data Collecting
Kode ini digunakan untuk mengunduh dataset yang diperlukan untuk proyek dari repositori GitHub. Dataset ini berisi gambar-gambar tangan yang digunakan untuk klasifikasi.

3. Data Understanding:
Proses ini melibatkan ekstraksi dataset dari file zip yang telah diunduh sebelumnya. Dataset terdiri dari gambar-gambar tangan yang mewakili gunting, batu, dan kertas. Gambar-gambar ini kemudian dibagi menjadi folder train dan validation untuk keperluan pelatihan dan evaluasi model.

4. Data Preprocessing:
Pada tahap ini, gambar-gambar yang telah dimuat diolah menggunakan augmentasi data untuk meningkatkan variasi dataset pelatihan. Augmentasi ini termasuk rotasi, pergeseran horizontal dan vertikal, pemotongan, dan pembalikan. Ini membantu model untuk belajar dari berbagai variasi gambar.

5. Modelling:
Arsitektur model yang digunakan adalah VGG19, yang telah dilatih sebelumnya pada dataset ImageNet. Transfer learning dilakukan dengan memanfaatkan bobot yang sudah dilatih pada VGG19 dan mengganti lapisan terakhir untuk sesuai dengan tugas klasifikasi tangan. Model diikuti dengan beberapa lapisan Dense untuk pembelajaran lebih lanjut.

6. Evaluation:
Model dievaluasi menggunakan dataset validasi untuk memperkirakan kinerja model. Metric yang digunakan adalah akurasi. Selain itu, visualisasi grafik akurasi dan loss dari pelatihan dan validasi juga disajikan untuk memahami tren performa model.

7. Test:
Terakhir, pengguna dapat mengunggah gambar tangan yang ingin diklasifikasikan oleh model. Model akan memproses gambar tersebut dan memberikan prediksi kelas yang sesuai (scissors, rock, atau paper). Ini memungkinkan pengguna untuk menguji model secara langsung dengan gambar-gambar baru.
