# **Masalah yang Diketahui**

Versi Aplikasi Pemungutan Suara Catalyst:

- 4.3 Android dan iOS (versi produksi 0.1.28 #2223)
- 4.4 iOS (versi produksi 0.1.30 #2241)
- Versi Backend: 4.3

Masalah | Dampak
:-: | :--
Pembulatan data skor ComRev | Data penilaian Ulasan Komunitas menggunakan logika sistem peringkat bintang untuk membulatkan skor agregat untuk masing-masing dari 3 kriteria tanpa titik desimal, kecuali untuk skor 4,5
Pemformatan | Beberapa pengguna mungkin mengalami format yang tidak konsisten atau aneh pada halaman tertentu, seperti bagian pengalaman tim yang relevan
Navigasi pengurutan acak | Ketika pengguna menerapkan opsi pengurutan “acak” (default), maka mengklik tanda panah untuk menavigasi antar proposal akan menyebabkan angka berubah secara acak, bukannya bertambah 1
Item bilah navigasi | Item bilah navigasi mungkin tampak salah tempat bagi pengguna iPhone
Pesan pemungutan suara telah berakhir | Setelah pemungutan suara berakhir, beberapa pengguna mungkin melihat hak suara mereka diganti dengan tanda bintang (“***”) daripada diganti dengan pesan yang sesuai
