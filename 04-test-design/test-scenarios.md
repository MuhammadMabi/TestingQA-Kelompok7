
# Test Scenarios – Jetprint.id

## 1. Tujuan Pengujian
Pengujian dilakukan untuk mengetahui apakah fitur utama pada website Jetprint.id dapat berjalan sesuai dengan fungsi yang diharapkan.

## 2. Daftar Skenario Pengujian

| ID | Fitur | Skenario Pengujian | Tujuan |
|---|---|---|---|
| TS01 | Login | Login menggunakan email dan password yang benar | Memastikan pengguna berhasil masuk ke akun |
| TS02 | Login | Login menggunakan password yang salah | Memastikan sistem menolak data login yang salah |
| TS03 | Login | Login dengan kolom email dan password kosong | Memastikan sistem memberikan validasi |
| TS04 | Registrasi | Mendaftar menggunakan data yang valid | Memastikan proses pendaftaran dapat dilakukan |
| TS05 | Registrasi | Mendaftar menggunakan format email yang tidak valid | Memastikan sistem memvalidasi format email |
| TS06 | Pencarian Produk | Mencari produk menggunakan nama produk | Memastikan produk dapat ditemukan melalui pencarian |
| TS07 | Detail Produk | Membuka salah satu produk yang tersedia | Memastikan informasi produk dapat ditampilkan |
| TS08 | Pemesanan | Mengisi detail pesanan dan jumlah produk | Memastikan pengguna dapat mengisi kebutuhan pesanan |
| TS09 | Pemesanan | Melanjutkan pesanan tanpa mengisi kolom wajib | Memastikan sistem memberikan validasi |
| TS10 | Upload Desain | Mengunggah file desain dengan format yang didukung | Memastikan file desain dapat diunggah |
| TS11 | Upload Desain | Mengunggah file dengan format yang tidak didukung | Memastikan sistem menolak file yang tidak sesuai |
| TS12 | Keranjang | Menambahkan produk ke keranjang | Memastikan produk dapat ditambahkan ke keranjang |

## 3. Metode Pengujian

Metode yang digunakan:

1. Equivalence Partitioning (EP), yaitu membagi data input menjadi kelompok valid dan tidak valid.
2. Boundary Value Analysis (BVA), yaitu menguji nilai pada batas minimum dan maksimum yang ditentukan sistem.
3. Negative Testing, yaitu menguji sistem menggunakan input yang salah atau tidak sesuai.

## 4. Kesimpulan

Skenario pengujian ini dibuat sebagai pedoman untuk menguji fitur utama website Jetprint.id. Setiap skenario akan digunakan oleh Anggota 3 untuk melakukan pengujian secara langsung dan mencatat hasil pengujian.
