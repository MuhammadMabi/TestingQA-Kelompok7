# TEST SUMMARY REPORT

## 1. Informasi Proyek

| Informasi | Keterangan |
|---|---|
| Project | Jetprint.id - Software Testing & QA |
| Object Under Test | Jetprint.id |
| Application Type | Web Application / E-Commerce Digital Printing |
| Testing Method | Black Box Testing |
| Testing Approach | Functional Testing |
| Role | Execution & Defect Coordinator |
| Tester | Muhammad Gifary Nezar |

## 2. Tujuan Pengujian

Test Summary Report ini dibuat untuk merangkum hasil pelaksanaan pengujian fungsional pada website Jetprint.id.

Pengujian dilakukan berdasarkan test scenario dan test case yang telah disusun oleh tim Test Design.

Tujuan pengujian adalah:
- Memastikan fitur website berjalan sesuai Expected Result.
- Mencatat hasil aktual dari setiap test case.
- Mengidentifikasi kendala selama pengujian.
- Mendokumentasikan evidence pengujian.
- Memberikan kesimpulan berdasarkan hasil pengujian.

## 3. Ringkasan Hasil Pengujian

| Keterangan | Jumlah |
|---|---:|
| Total Test Case | 10 |
| PASS | 9 |
| FAIL | 0 |
| BLOCKED | 1 |
| NOT EXECUTED | 0 |

## 4. Detail Hasil Pengujian

| Test Case ID | Fitur yang Diuji | Status |
|---|---|---|
| TC01 | Login dengan Email dan Password Benar | PASS |
| TC02 | Login dengan Password Salah | PASS |
| TC03 | Login dengan Kolom Kosong | PASS |
| TC04 | Registrasi dengan Data Lengkap | PASS |
| TC05 | Registrasi dengan Email Tidak Valid | PASS |
| TC06 | Registrasi dengan Password Kurang dari 8 Karakter | PASS |
| TC07 | Pencarian Produk | PASS |
| TC08 | Menambahkan Produk ke Keranjang | PASS |
| TC09 | Validasi Jumlah Pesanan Kosong | BLOCKED |
| TC10 | Validasi Ukuran File Upload | PASS |

## 5. Hasil dan Temuan Pengujian

Berdasarkan pelaksanaan pengujian, sebagian besar fitur yang diuji memberikan hasil sesuai dengan Expected Result.

Beberapa hasil pengujian yang diperoleh:

1. **Login:** Sistem berhasil menerima kredensial yang benar dan menolak password yang salah.
2. **Registrasi:** Sistem berhasil memproses pendaftaran dengan data lengkap serta memberikan validasi terhadap format email dan panjang password.
3. **Pencarian Produk:** Sistem menampilkan produk yang sesuai dengan kata kunci pencarian.
4. **Keranjang:** Produk berhasil ditambahkan ke keranjang dan detail pesanan ditampilkan.
5. **Validasi Jumlah Pesanan:** Pengujian belum dapat diselesaikan karena jumlah pesanan tidak dapat dikosongkan atau diubah menjadi 0 melalui antarmuka website.
6. **Upload Desain:** Website menampilkan pesan "Ukuran maksimal 50MB untuk produk ini" ketika file yang dipilih melebihi batas ukuran yang ditentukan.

## 6. Kendala Pengujian

Kendala ditemukan pada TC09, yaitu pengujian validasi jumlah pesanan kosong.

Saat pengujian dilakukan, nilai jumlah pesanan tetap berada pada angka 1 dan tidak dapat dikosongkan atau diubah menjadi 0.

Akibatnya, langkah pengujian tidak dapat dijalankan sesuai skenario yang telah ditentukan.

Oleh karena itu, TC09 diberikan status **BLOCKED** dan tidak langsung dikategorikan sebagai defect.

## 7. Defect Summary

Berdasarkan hasil pengujian yang telah dilakukan:

| Keterangan | Jumlah |
|---|---:|
| Defect Terverifikasi | 0 |
| Defect Belum Diverifikasi | 0 |

Tidak terdapat defect yang ditetapkan sebagai bug terverifikasi selama pengujian ini.

Kendala pada TC09 dicatat sebagai pengujian BLOCKED dan memerlukan pemeriksaan lebih lanjut.

## 8. Kesimpulan

Berdasarkan hasil pengujian terhadap 10 test case pada website Jetprint.id, diperoleh 9 test case berstatus PASS dan 1 test case berstatus BLOCKED.

Secara umum, fitur login, registrasi, pencarian produk, penambahan produk ke keranjang, dan validasi upload desain telah memberikan hasil sesuai dengan Expected Result.

Namun, pengujian validasi jumlah pesanan kosong pada TC09 belum dapat diselesaikan karena keterbatasan interaksi pada kolom jumlah pesanan.

Dengan demikian, pengujian menunjukkan bahwa sebagian besar fitur yang diuji telah berjalan sesuai dengan skenario pengujian, dengan satu skenario yang masih memerlukan pemeriksaan lebih lanjut.

## 9. Rekomendasi

- Melakukan pemeriksaan lebih lanjut terhadap skenario TC09.
- Melakukan pengujian ulang apabila kendala pada TC09 telah dapat ditangani.
- Mempertahankan dokumentasi screenshot sebagai evidence pengujian.
- Memperbarui laporan apabila terdapat pengujian lanjutan atau perubahan hasil.

