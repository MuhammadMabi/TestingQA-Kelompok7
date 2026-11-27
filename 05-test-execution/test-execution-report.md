# TEST EXECUTION REPORT
## Jetprint.id – Software Testing & Quality Assurance

---

## 1. Informasi Pengujian

| Informasi | Keterangan |
|---|---|
| Project | Jetprint.id – Software Testing & QA |
| Object Under Test | Jetprint.id |
| Application Type | Web Application / E-Commerce Digital Printing |
| Testing Method | Black Box Testing |
| Testing Approach | Functional Testing |
| Role | Execution & Defect Coordinator |
| Tester | Muhammad Gifary Nezar |
| Browser | Google Chrome |
| Operating System | Windows |
| Device | Desktop / Laptop |
| Testing Status | Execution Completed with Blocked Case |

## 2. Tujuan Pengujian

Dokumen ini digunakan untuk mencatat proses dan hasil pelaksanaan pengujian terhadap website Jetprint.id.

Pengujian dilakukan berdasarkan test case yang telah disusun oleh tim Test Design.

Tujuan pengujian:

- Memastikan fungsi website berjalan sesuai harapan.
- Membandingkan Expected Result dan Actual Result.
- Mengidentifikasi kemungkinan defect.
- Mengumpulkan evidence pengujian.
- Mendokumentasikan hasil Pass, Fail, dan Blocked.

## 3. Ruang Lingkup Pengujian

Pengujian dilakukan terhadap beberapa fungsi utama website Jetprint.id, meliputi:

1. Login pengguna.
2. Registrasi akun.
3. Pencarian produk.
4. Penambahan produk ke keranjang.
5. Validasi jumlah pesanan.
6. Validasi ukuran file upload desain.

Pengujian dilakukan melalui tampilan website sebagai pengguna tanpa mengakses source code maupun database aplikasi.

## 4. Test Execution Summary

| Keterangan | Jumlah |
|---|---:|
| Total Test Cases | 10 |
| PASS | 9 |
| FAIL | 0 |
| BLOCKED | 1 |
| NOT EXECUTED | 0 |

### Ringkasan Status

- **PASS:** Fungsi memberikan hasil sesuai dengan expected result.
- **FAIL:** Fungsi memberikan hasil yang tidak sesuai dengan expected result.
- **BLOCKED:** Pengujian tidak dapat dilaksanakan sesuai skenario karena terdapat keterbatasan atau kondisi tertentu.
- **NOT EXECUTED:** Test case belum dijalankan.

## 5. Detail Hasil Pengujian

### TC01 – Login dengan Email dan Password Benar

| Komponen | Hasil |
|---|---|
| Test Case ID | TC01 |
| Fitur yang Diuji | Login |
| Tujuan Pengujian | Memastikan pengguna dapat masuk menggunakan kredensial valid. |
| Test Data | Akun pelanggan yang sudah terdaftar. |
| Expected Result | Pengguna berhasil login dan diarahkan ke halaman setelah login. |
| Actual Result | Sistem menerima email dan password yang valid. Pengguna berhasil masuk dan diarahkan ke halaman profil pelanggan. Nama dan email akun ditampilkan pada halaman tersebut. |
| Status | **PASS** |

**Bukti Pengujian:**

1. [TC01-01-before-login.jpg](screenshots/TC01%20-%20Login%20Valid/TC01-01-before-login.jpg) – Tampilan awal website sebelum login.
2. [TC01-02-login-form.jpg](screenshots/TC01%20-%20Login%20Valid/TC01-02-login-form.jpg) – Form login sebelum diisi.
3. [TC01-03-password-validation.jpg](screenshots/TC01%20-%20Login%20Valid/TC01-03-password-validation.jpg) – Validasi password kurang dari 8 karakter.
4. [TC01-04-credentials-filled.jpg](screenshots/TC01%20-%20Login%20Valid/TC01-04-credentials-filled.jpg) – Form login setelah data dimasukkan.
5. [TC01-05-login-success.jpg](screenshots/TC01%20-%20Login%20Valid/TC01-05-login-success.jpg) – Tampilan profil setelah berhasil login.

### TC02 – Login dengan Password Salah

| Komponen | Hasil |
|---|---|
| Test Case ID | TC02 |
| Fitur yang Diuji | Login |
| Tujuan Pengujian | Memastikan sistem menolak kredensial yang salah. |
| Test Data | Email terdaftar dan password salah. |
| Expected Result | Sistem menolak login dan menampilkan pesan kesalahan yang sesuai. |
| Actual Result | Sistem menampilkan pesan "Email atau password salah" dan pengguna tidak berhasil masuk. |
| Status | **PASS** |

**Bukti Pengujian:**

1. [TC02-01-login-form.jpg](screenshots/TC02%20-%20Login%20dengan%20Password%20Salah/TC02-01-login-form.jpg) – Form login dengan data pengujian.
2. [TC02-02-login-rejected.jpg](screenshots/TC02%20-%20Login%20dengan%20Password%20Salah/TC02-02-login-rejected.jpg) – Sistem menolak login dengan password salah.

### TC03 – Login dengan Kolom Kosong

| Komponen | Hasil |
|---|---|
| Test Case ID | TC03 |
| Fitur yang Diuji | Login |
| Tujuan Pengujian | Memastikan sistem memberikan validasi untuk input wajib. |
| Test Data | Email dan password kosong. |
| Expected Result | Sistem meminta pengguna mengisi kolom wajib. |
| Actual Result | Sistem menampilkan validasi bahwa kolom email wajib diisi ketika pengguna mencoba mengirim formulir dalam keadaan kosong. |
| Status | **PASS** |

**Bukti Pengujian:**

1. [TC03-01-empty-login-form.jpg](screenshots/TC03%20-%20Login%20dengan%20Kolom%20Kosong/TC03-01-empty-login-form.jpg) – Form login sebelum diisi.
2. [TC03-02-empty-fields-validation.jpg](screenshots/TC03%20-%20Login%20dengan%20Kolom%20Kosong/TC03-02-empty-fields-validation.jpg) – Validasi ketika kolom login kosong.

### TC04 – Registrasi dengan Data Lengkap

| Komponen | Hasil |
|---|---|
| Test Case ID | TC04 |
| Fitur yang Diuji | Registrasi |
| Tujuan Pengujian | Memastikan formulir menerima data yang valid. |
| Test Data | Nama, nomor WhatsApp, email, dan password sesuai aturan. |
| Expected Result | Sistem memproses pendaftaran dan memberikan konfirmasi yang sesuai. |
| Actual Result | Sistem berhasil memproses pendaftaran akun dan mengarahkan pengguna ke halaman profil pelanggan. |
| Status | **PASS** |

**Bukti Pengujian:**

1. [TC04-01-registration-form.jpg](screenshots/TC04%20-%20Registrasi%20dengan%20Data%20Lengkap/TC04-01-registration-form.jpg) – Form registrasi sebelum diisi.
2. [TC04-02-registration-filled.jpg](screenshots/TC04%20-%20Registrasi%20dengan%20Data%20Lengkap/TC04-02-registration-filled.jpg) – Form registrasi setelah diisi.
3. [TC04-03-registration-result.jpg](screenshots/TC04%20-%20Registrasi%20dengan%20Data%20Lengkap/TC04-03-registration-result.jpg) – Hasil proses registrasi.

### TC05 – Registrasi dengan Email Tidak Valid

| Komponen | Hasil |
|---|---|
| Test Case ID | TC05 |
| Fitur yang Diuji | Registrasi |
| Tujuan Pengujian | Memastikan format email divalidasi. |
| Test Data | Email tidak valid: `fariz123` |
| Expected Result | Sistem menolak format email yang tidak valid. |
| Actual Result | Browser menampilkan validasi format email yang tidak sesuai dan formulir tidak dapat dikirim. |
| Status | **PASS** |

**Bukti Pengujian:**

1. [TC05-01-registration-invalid-email.jpg](screenshots/TC05%20-%20Registrasi%20dengan%20Email%20Tidak%20Valid/TC05-01-registration-invalid-email.jpg) – Form registrasi dengan email tidak valid.
2. [TC05-02-registration-invalid-email-rejected.jpg](screenshots/TC05%20-%20Registrasi%20dengan%20Email%20Tidak%20Valid/TC05-02-registration-invalid-email-rejected.jpg) – Validasi penolakan format email.

### TC06 – Registrasi dengan Password Kurang dari 8 Karakter

| Komponen | Hasil |
|---|---|
| Test Case ID | TC06 |
| Fitur yang Diuji | Registrasi |
| Tujuan Pengujian | Memeriksa validasi panjang password. |
| Test Data | Password `abc123` |
| Expected Result | Sistem menolak password dan menampilkan validasi. |
| Actual Result | Browser menampilkan pesan bahwa password harus memiliki minimal 8 karakter. |
| Status | **PASS** |

**Bukti Pengujian:**

1. [TC06-01-registration-short-password.jpg](screenshots/TC06%20-%20Registrasi%20dengan%20Password%20Kurang%20dari%208%20Karakter/TC06-01-registration-short-password.jpg) – Form registrasi dengan password kurang dari 8 karakter.
2. [TC06-02-registration-short-password-rejected.jpg](screenshots/TC06%20-%20Registrasi%20dengan%20Password%20Kurang%20dari%208%20Karakter/TC06-02-registration-short-password-rejected.jpg) – Validasi penolakan password.

### TC07 – Mencari Produk Spanduk Flexy

| Komponen | Hasil |
|---|---|
| Test Case ID | TC07 |
| Fitur yang Diuji | Pencarian Produk |
| Tujuan Pengujian | Memastikan fitur pencarian menampilkan hasil yang relevan. |
| Test Data | Kata kunci "Spanduk Flexy" |
| Expected Result | Sistem menampilkan produk yang sesuai dengan kata kunci. |
| Actual Result | Sistem menampilkan satu produk Spanduk Flexy yang sesuai dengan kata kunci pencarian. |
| Status | **PASS** |

**Bukti Pengujian:**

1. [TC07-01-search-keyword.jpg](screenshots/TC07%20-%20Pencarian%20Produk/TC07-01-search-keyword.jpg) – Kata kunci pencarian produk.
2. [TC07-02-search-result.jpg](screenshots/TC07%20-%20Pencarian%20Produk/TC07-02-search-result.jpg) – Hasil pencarian produk Spanduk Flexy.

### TC08 – Menambahkan Produk ke Keranjang

| Komponen | Hasil |
|---|---|
| Test Case ID | TC08 |
| Fitur yang Diuji | Keranjang |
| Tujuan Pengujian | Memastikan produk dapat ditambahkan ke keranjang. |
| Test Data | Produk Spanduk Flexy, jumlah 1. |
| Expected Result | Produk masuk ke keranjang dan detailnya ditampilkan dengan benar. |
| Actual Result | Produk Spanduk Flexy berhasil ditambahkan ke keranjang. Informasi produk, konfigurasi, jumlah, dan harga ditampilkan pada halaman keranjang. |
| Status | **PASS** |

**Bukti Pengujian:**

1. [TC08-01-product-detail.jpg](screenshots/TC08%20-%20Menambahkan%20Produk%20ke%20Keranjang/TC08-01-product-detail.jpg) – Halaman detail dan konfigurasi produk.
2. [TC08-02-product-added-to-cart.jpg](screenshots/TC08%20-%20Menambahkan%20Produk%20ke%20Keranjang/TC08-02-product-added-to-cart.jpg) – Produk berhasil ditambahkan ke keranjang.
3. [TC08-03-cart-verification.jpg](screenshots/TC08%20-%20Menambahkan%20Produk%20ke%20Keranjang/TC08-03-cart-verification.jpg) – Verifikasi produk pada keranjang belanja.

### TC09 – Melanjutkan Pemesanan Tanpa Mengisi Jumlah

| Komponen | Hasil |
|---|---|
| Test Case ID | TC09 |
| Fitur yang Diuji | Pemesanan |
| Tujuan Pengujian | Memastikan jumlah pesanan yang wajib diisi divalidasi. |
| Test Data | Jumlah kosong. |
| Expected Result | Sistem meminta pengguna mengisi jumlah pesanan. |
| Actual Result | Kolom jumlah memiliki nilai awal 1. Nilai tersebut tidak dapat dikosongkan melalui input biasa maupun diturunkan menjadi 0 menggunakan tombol minus. |
| Status | **BLOCKED** |

**Bukti Pengujian:**

1. [TC09-01-quantity-field-default.jpg](screenshots/TC09%20-%20Validasi%20Jumlah%20Pesanan%20Kosong/TC09-01-quantity-field-default.jpg) – Kolom jumlah memiliki nilai awal 1 dan tidak dapat dikosongkan.

**Catatan Pengujian:**

Skenario tidak dapat dilaksanakan sesuai test case karena antarmuka website membatasi jumlah pesanan dengan nilai minimum 1. Pengujian ditetapkan BLOCKED dan belum dapat digunakan untuk menyimpulkan adanya defect.

### TC10 – Mengunggah File Desain Berukuran 51 MB

| Komponen | Hasil |
|---|---|
| Test Case ID | TC10 |
| Fitur yang Diuji | Upload Desain |
| Tujuan Pengujian | Memeriksa batas ukuran file yang dapat diunggah. |
| Test Data | File desain berukuran lebih dari 50 MB. |
| Expected Result | Sistem menolak file dan menampilkan pesan yang sesuai. |
| Actual Result | Setelah pengguna memilih file berukuran lebih dari 50 MB melalui jendela File Explorer, sistem menampilkan pesan "Ukuran maksimal 50MB untuk produk ini." pada bagian upload desain. |
| Status | **PASS** |

**Bukti Pengujian:**

1. [TC10-01-upload-design-section.jpg](screenshots/TC10%20-%20Validasi%20Ukuran%20File%20Upload/TC10-01-upload-design-section.jpg) – Tampilan area upload desain dan batas maksimal 50 MB.
2. [TC10-02-upload-file-size-validation.jpg](screenshots/TC10%20-%20Validasi%20Ukuran%20File%20Upload/TC10-02-upload-file-size-validation.jpg) – Pesan validasi ketika memilih file lebih dari 50 MB.

## 6. Evidence Documentation Summary

Seluruh bukti pengujian disimpan pada:

`05-test-execution/screenshots/`

Dokumentasi terdiri dari 24 screenshot yang dikelompokkan ke dalam 10 folder berdasarkan Test Case ID.

Setiap screenshot pada bagian hasil pengujian di atas dapat dibuka melalui tautan Markdown.

## 7. Defect Documentation

Setiap hasil pengujian yang tidak sesuai dengan Expected Result akan dianalisis terlebih dahulu.

Defect yang telah diverifikasi akan didokumentasikan pada:

`06-bug-management/bug-report.md`

Catatan:

- Belum ada defect yang dinyatakan terverifikasi berdasarkan hasil pengujian yang dicatat dalam laporan ini.
- TC09 berstatus BLOCKED dan tidak otomatis dikategorikan sebagai defect.
- Hasil pengujian yang berstatus PASS tidak memerlukan bug report.

## 8. Testing Notes

- Pengujian dilakukan melalui tampilan website Jetprint.id sebagai pengguna.
- Pengujian menggunakan data dummy untuk kebutuhan registrasi dan pengujian.
- Tidak dilakukan transaksi pembayaran sungguhan.
- TC09 belum dapat dijalankan sesuai skenario karena jumlah pesanan memiliki nilai minimum 1.
- TC10 menunjukkan pesan validasi ketika file yang dipilih melebihi batas maksimal 50 MB.
- Hasil pengujian dicatat berdasarkan kondisi aktual website yang diamati.

## 9. Kesimpulan

Berdasarkan pelaksanaan pengujian terhadap 10 test case pada website Jetprint.id, diperoleh hasil:

- 9 test case berstatus PASS.
- 0 test case berstatus FAIL.
- 1 test case berstatus BLOCKED.
- 0 test case berstatus NOT EXECUTED.

Secara umum, fungsi login, registrasi, pencarian produk, penambahan produk ke keranjang, dan validasi upload desain memberikan hasil sesuai dengan Expected Result.

Sementara itu, TC09 belum dapat dilaksanakan sesuai skenario karena kolom jumlah pesanan tidak dapat dikosongkan atau diubah menjadi 0 melalui antarmuka website.

Dengan demikian, hasil pengujian ini menunjukkan bahwa sebagian besar skenario pengujian berhasil dijalankan sesuai harapan, dengan satu skenario yang masih berstatus BLOCKED.

Laporan ini dapat diperbarui apabila terdapat pengujian lanjutan, retesting, atau perubahan hasil dari tim QA.
