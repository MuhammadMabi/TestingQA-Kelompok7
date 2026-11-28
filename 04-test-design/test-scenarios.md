
# Test Cases – Jetprint.id

## 1. Test Case Login

### TC01 – Login dengan Data Benar
- Fitur: Login
- Precondition: Pengguna sudah memiliki akun.
- Test Data:
  - Email: tester.jetprint@example.com
  - Password: PasswordValid123
- Steps:
  1. Membuka halaman login.
  2. Memasukkan email yang terdaftar.
  3. Memasukkan password yang benar.
  4. Menekan tombol login.
- Expected Result: Pengguna berhasil masuk ke akun.

### TC02 – Login dengan Password Salah
- Fitur: Login
- Precondition: Pengguna sudah memiliki akun.
- Test Data:
  - Email: Email terdaftar.
  - Password: PasswordSalah123
- Steps:
  1. Membuka halaman login.
  2. Memasukkan email terdaftar.
  3. Memasukkan password yang salah.
  4. Menekan tombol login.
- Expected Result: Sistem menolak login dan menampilkan pesan kesalahan.

### TC03 – Login dengan Kolom Kosong
- Fitur: Login
- Test Data: Email dan password kosong.
- Steps:
  1. Membuka halaman login.
  2. Membiarkan kolom email dan password kosong.
  3. Menekan tombol login.
- Expected Result: Sistem memberikan validasi bahwa kolom harus diisi.

## 2. Test Case Registrasi

### TC04 – Registrasi dengan Data Valid
- Fitur: Registrasi
- Test Data:
  - Nama: Tester Jetprint
  - Email: tester.jetprint@example.com
  - Nomor WhatsApp: 081234567890
  - Password: PasswordValid123
- Steps:
  1. Membuka halaman registrasi.
  2. Mengisi seluruh kolom dengan data yang valid.
  3. Menekan tombol daftar.
- Expected Result: Sistem memproses pendaftaran dan menampilkan konfirmasi sesuai proses registrasi.

### TC05 – Registrasi dengan Email Tidak Valid
- Fitur: Registrasi
- Test Data:
  - Email: farizi123
- Steps:
  1. Membuka halaman registrasi.
  2. Mengisi formulir dengan data yang diperlukan.
  3. Memasukkan email dengan format tidak valid.
  4. Menekan tombol daftar.
- Expected Result: Sistem menolak format email yang tidak valid.

## 3. Test Case Pencarian dan Detail Produk

### TC06 – Mencari Produk
- Fitur: Pencarian Produk
- Test Data: Nama produk yang tersedia di website.
- Steps:
  1. Membuka halaman utama Jetprint.id.
  2. Memasukkan nama produk pada kolom pencarian.
  3. Menjalankan pencarian.
- Expected Result: Sistem menampilkan produk yang sesuai dengan kata kunci.

### TC07 – Melihat Detail Produk
- Fitur: Detail Produk
- Test Data: Salah satu produk yang tersedia.
- Steps:
  1. Membuka halaman produk.
  2. Memilih salah satu produk.
  3. Membuka halaman detail produk.
- Expected Result: Sistem menampilkan informasi produk seperti nama, harga, dan spesifikasi yang tersedia.

## 4. Test Case Pemesanan

### TC08 – Mengisi Detail Pemesanan
- Fitur: Pemesanan
- Test Data:
  - Produk: Produk percetakan yang tersedia.
  - Jumlah: 1.
  - Ukuran: Pilihan yang tersedia.
- Steps:
  1. Memilih produk.
  2. Membuka formulir pemesanan.
  3. Mengisi pilihan produk dan jumlah.
  4. Melengkapi informasi wajib lainnya.
  5. Melanjutkan proses pemesanan.
- Expected Result: Sistem menerima data pesanan yang valid dan menampilkan tahapan pemesanan berikutnya.

### TC09 – Pemesanan dengan Kolom Wajib Kosong
- Fitur: Pemesanan
- Test Data: Salah satu kolom wajib tidak diisi.
- Steps:
  1. Membuka formulir pemesanan.
  2. Membiarkan salah satu kolom wajib kosong.
  3. Menekan tombol lanjut atau pesan.
- Expected Result: Sistem memberikan validasi dan meminta pengguna melengkapi data.

## 5. Test Case Upload Desain

### TC10 – Upload File dengan Format yang Didukung
- Fitur: Upload Desain
- Test Data: File desain dengan format yang tercantum sebagai format yang didukung website.
- Steps:
  1. Membuka bagian upload desain.
  2. Memilih file desain.
  3. Mengunggah file.
- Expected Result: File berhasil diunggah apabila memenuhi ketentuan website.

### TC11 – Upload File dengan Format Tidak Didukung
- Fitur: Upload Desain
- Test Data: File dengan format yang tidak didukung website.
- Steps:
  1. Membuka bagian upload desain.
  2. Memilih file dengan format yang tidak didukung.
  3. Mencoba mengunggah file.
- Expected Result: Sistem menolak file dan menampilkan pesan kesalahan.

## 6. Test Case Keranjang

### TC12 – Menambahkan Produk ke Keranjang
- Fitur: Keranjang
- Precondition: Produk tersedia dan dapat dipesan.
- Test Data: Salah satu produk yang tersedia.
- Steps:
  1. Memilih produk.
  2. Melengkapi pilihan produk yang diwajibkan.
  3. Menekan tombol tambah ke keranjang jika tersedia.
  4. Membuka halaman keranjang.
- Expected Result: Produk tampil di keranjang dengan informasi pesanan yang sesuai.

## 7. Metode Pengujian

### A. Equivalence Partitioning (EP)
Pengujian dilakukan dengan membagi data menjadi kelompok valid dan tidak valid.

Contoh:
- Email dengan format benar.
- Email dengan format salah.
- Email kosong.

### B. Boundary Value Analysis (BVA)
Pengujian dilakukan pada batas nilai input yang ditentukan sistem.

Contoh:
- Jumlah pesanan di bawah batas minimum.
- Jumlah pesanan tepat pada batas minimum.
- Jumlah pesanan di atas batas minimum.

Nilai batas mengikuti ketentuan yang ditampilkan pada website.

### C. Negative Testing
Pengujian dilakukan menggunakan input yang tidak sesuai.

Contoh:
- Password salah.
- Email tidak valid.
- Kolom wajib kosong.
- File dengan format yang tidak didukung.

## 8. Catatan
Actual Result, screenshot evidence, status PASS/FAIL, dan bug report diisi oleh Anggota 3 setelah pengujian dilakukan.
