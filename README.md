# Project Sistem Terdistribusi: Pemrosesan Video Terdistribusi Berbasis Cloud untuk Deteksi Objek
---
### Ansyarullah
### 1217050017
---

Proyek ini dilakukan sebagai bagian dari mata kuliah CSCI 5253: Komputasi Skala Pusat Data yang ditawarkan di CU Boulder. Tujuan dari Proyek ini adalah untuk membuat pemrosesan frame video terdistribusi untuk deteksi objek menggunakan DNN yang telah dilatih sebelumnya. Dengan memasukkan video ke dalam sistem, kami
pada dasarnya akan mendapatkan kembali video yang sama dengan objek yang berbeda yang disorot dan juga jumlah mereka dalam a
bingkai tertentu. Objek-objek ini bisa berupa mobil, orang, atau objek lain yang didukung oleh
DNN yang telah dilatih sebelumnya. Ini akan terjadi dengan memecah video menjadi beberapa frame dan memproses
masing-masing frame tersebut. Setelah pemrosesan selesai pada frame, mereka digabungkan
kembali dengan cara mempertahankan urutan bingkai asli. Dengan demikian, kami mendapatkan video yang diperlukan dengan
semua objek dan jumlahnya disorot.

# Laporan dan Video Demo
Laporan yang lebih rinci tentang Proyek (On Process)

Video penjelasan tentang Proyek bersama dengan Demo. (On process)

# Langkah-langkah untuk menjalankan Proyek

Proyek ini berisi

--server.py - menjalankan server untuk distribusi dan manajemen. Berikan alamat ip server sebagai argumen baris perintah.

--worker.py - jalankan node klien pada perangkat pengguna. Berikan alamat ip server dan klien sebagai argumen baris perintah dalam urutan tersebut.

Setiap klien dimulai sebagai pekerja. Ketika pengguna perlu meminta pemrosesan, ketik request di terminal. Ketika Anda ingin menyelesaikan pemrosesan (dalam kasus streaming langsung), ketik end di terminal. Ketik quit untuk keluar.

Perintah-perintah pada node klien:

1. request live --> untuk meminta pemrosesan streaming langsung
2. request path-to-video --> untuk meminta pemrosesan streaming video
3. end --> untuk menghentikan pemrosesan
4. quit --> untuk keluar

Perintah-perintah pada node server:

1. quit --> untuk keluar

Translated with DeepL.com (free version)
