# Feature List

## 1. Tujuan

Dokumen ini berisi hasil identifikasi awal fitur yang tersedia pada Jetprint.id serta
klasifikasi fitur berdasarkan scope pengujian.

Klasifikasi yang digunakan:

- **In Scope**: fitur yang direncanakan untuk diuji oleh kelompok.
- **Need Permission**: fitur yang secara teknis dapat diuji tetapi berpotensi menghasilkan
  transaksi, biaya, pesanan nyata, atau memengaruhi operasional Jetprint sehingga perlu
  izin sebelum dilakukan pengujian.
- **Out of Scope**: fitur yang tidak dijadikan fokus pengujian pada proyek ini.

Status ini dapat diperbarui berdasarkan hasil eksplorasi aplikasi, konsultasi dengan QA
profesional, arahan dosen, dan izin dari pihak Jetprint.

---

## 2. Feature Identification

| ID | Fitur | Deskripsi | Status | Catatan |
|---|---|---|---|---|
| F-01 | Homepage | Menampilkan informasi layanan, kategori, produk pilihan, dan navigasi utama | In Scope | Dapat diuji tanpa transaksi |
| F-02 | Navigation | Navigasi antar halaman dan menu utama website | In Scope | Fokus pada link dan perpindahan halaman |
| F-03 | Product Catalog | Menampilkan daftar produk yang tersedia | In Scope | Termasuk tampilan daftar produk |
| F-04 | Product Category | Menampilkan produk berdasarkan kategori | In Scope | Verifikasi kategori dan produk |
| F-05 | Product Detail | Menampilkan nama, harga, spesifikasi, dan informasi produk | In Scope | Dapat dibandingkan dengan informasi pada katalog |
| F-06 | Product Configuration | Memilih bahan, ukuran, jumlah, atau opsi produk yang tersedia | In Scope | Variasi konfigurasi tergantung produk |
| F-07 | Price Calculation | Menghitung harga berdasarkan konfigurasi dan jumlah produk | In Scope | Cocok untuk Boundary Value Analysis jika tersedia batas jumlah |
| F-08 | Design Upload Validation | Upload file desain sesuai format dan batas ukuran yang diizinkan | In Scope | Gunakan file dummy yang aman, jangan membuat pesanan produksi |
| F-09 | Design Link Input | Memasukkan link desain sebagai alternatif upload file | In Scope | Verifikasi validasi input jika tersedia |
| F-10 | Add to Cart | Memasukkan produk yang telah dikonfigurasi ke keranjang | In Scope | Berhenti sebelum transaksi nyata |
| F-11 | Shopping Cart | Menampilkan dan mengelola produk dalam keranjang | In Scope | Verifikasi item, jumlah, harga, update, dan hapus jika tersedia |
| F-12 | User Registration | Membuat akun pengguna | In Scope | Gunakan akun dan data pengujian yang valid |
| F-13 | User Login | Login menggunakan akun pengguna | In Scope | Positive dan negative testing |
| F-14 | Guest Checkout | Checkout tanpa membuat akun | Need Permission | Proses awal dapat diamati, jangan submit pesanan tanpa izin |
| F-15 | Checkout Validation | Validasi data yang dibutuhkan pada proses checkout | Need Permission | Batasi pada validasi form sebelum pembuatan order |
| F-16 | Promo & Coupon | Menampilkan promo dan menerima kode kupon | In Scope | Penggunaan sampai transaksi final perlu dibatasi |
| F-17 | Payment | Memilih dan melakukan metode pembayaran | Need Permission | Berhubungan dengan transaksi finansial nyata |
| F-18 | Shipping | Memilih pengiriman dan perhitungan biaya kirim | Need Permission | Data ongkir dapat diamati pada checkout jika diizinkan |
| F-19 | Store Pickup | Memilih metode pengambilan pesanan di lokasi | Need Permission | Jangan membuat order nyata tanpa izin |
| F-20 | Order Creation | Membuat pesanan sampai memperoleh nomor/kode order | Need Permission | Dapat masuk sistem operasional Jetprint |
| F-21 | Order Tracking | Melacak status menggunakan kode pesanan | In Scope | Gunakan kode order yang sah dan memang tersedia untuk pengujian |
| F-22 | Order History | Melihat histori transaksi melalui akun pengguna | Need Permission | Membutuhkan akun yang mempunyai data order |
| F-23 | Product Review | Memberikan rating atau ulasan produk | Need Permission | Dapat menambah data publik ke website |
| F-24 | FAQ | Menampilkan informasi pertanyaan dan jawaban layanan | In Scope | Fokus navigasi dan penyajian informasi |
| F-25 | Cara Order | Menampilkan panduan pemesanan | In Scope | Dapat diuji tanpa transaksi |
| F-26 | Blog & Tips | Menampilkan konten artikel | Out of Scope | Bukan fungsi utama proses pemesanan |
| F-27 | Tentang Kami | Menampilkan informasi perusahaan | Out of Scope | Static/informational content |
| F-28 | Karir | Menampilkan informasi rekrutmen | Out of Scope | Tidak berkaitan dengan alur pemesanan |
| F-29 | Kalkulator Potongan | Tool untuk membantu perhitungan potongan | In Scope | Menarik untuk functional dan boundary testing |
| F-30 | WhatsApp / Chat Sales | Menghubungkan pengguna dengan customer service/sales | Out of Scope | Layanan eksternal dan bukan fungsi inti sistem yang diuji |
| F-31 | Admin / Back Office | Pengelolaan produk, pesanan, pembayaran, dan data internal | Out of Scope | Tidak tersedia bagi pengguna publik |
| F-32 | Security / Penetration Testing | Pengujian kerentanan atau eksploitasi keamanan | Out of Scope | Tidak dilakukan tanpa otorisasi khusus |
| F-33 | Performance / Stress Testing | Pengujian beban tinggi terhadap website | Out of Scope | Berpotensi mengganggu layanan publik |

---

## 3. In Scope

Fitur utama yang direkomendasikan sebagai fokus pengujian:

1. Homepage.
2. Navigation.
3. Product Catalog.
4. Product Category.
5. Product Detail.
6. Product Configuration.
7. Price Calculation.
8. Design Upload Validation.
9. Design Link Input.
10. Add to Cart.
11. Shopping Cart.
12. User Registration.
13. User Login.
14. Promo & Coupon.
15. Order Tracking.
16. FAQ.
17. Cara Order.
18. Kalkulator Potongan.

Fitur-fitur tersebut dipilih karena dapat merepresentasikan fungsi utama website dan
sebagian besar dapat diuji tanpa menghasilkan transaksi finansial nyata.

---

## 4. Need Permission

Fitur berikut hanya akan diuji lebih lanjut apabila kelompok memperoleh izin dari pihak
Jetprint:

1. Guest Checkout sampai pembuatan order.
2. Checkout sampai submit pesanan.
3. Pembayaran.
4. Pengiriman dan kalkulasi ongkir dalam proses transaksi.
5. Store Pickup dalam proses transaksi.
6. Pembuatan order nyata.
7. Order History yang membutuhkan order nyata.
8. Product Review atau aktivitas yang menambahkan data publik.

Tanpa izin, pengujian terhadap fitur tersebut dibatasi pada observasi tampilan atau
validasi yang tidak menghasilkan transaksi maupun perubahan data operasional.

---

## 5. Out of Scope

Fitur atau aktivitas berikut tidak menjadi fokus pengujian:

1. Blog & Tips.
2. Tentang Kami.
3. Karir.
4. WhatsApp / Chat Sales.
5. Admin atau Back Office Jetprint.
6. Database dan server internal.
7. API internal yang tidak tersedia secara publik.
8. Penetration testing.
9. Vulnerability exploitation.
10. Brute force testing.
11. Performance, load, dan stress testing.

---

## 6. Catatan Pengujian

Daftar fitur ini disusun berdasarkan hasil identifikasi awal terhadap website Jetprint.id
dan belum merupakan hasil pelaksanaan test case.

Status fitur dapat berubah setelah:

- eksplorasi lebih lanjut terhadap website;
- diskusi dengan QA profesional;
- arahan dari dosen;
- konfirmasi atau izin dari pihak Jetprint.

Penemuan fitur tidak dianggap sebagai bug. Bug hanya akan dicatat setelah suatu test case
dieksekusi dan actual result tidak sesuai dengan expected result.