# IEEE/ISO References

## 1. Tujuan

Dokumen ini berisi standar IEEE/ISO yang digunakan sebagai referensi dalam perencanaan dan pelaksanaan pengujian website Jetprint.id.

Referensi dibatasi pada standar yang diterbitkan dalam rentang tahun 2023–2026 sesuai ketentuan tugas. Standar dipilih berdasarkan relevansinya terhadap software quality, quality assurance, evaluasi kualitas aplikasi, dan software testing.

## 2. Daftar Standar

| No. | Standar | Tahun | Topik | Penerapan pada Proyek |
|---:|---|---:|---|---|
| 1 | ISO/IEC 25010 | 2023 | Product Quality Model | Menentukan karakteristik kualitas produk yang relevan untuk diuji |
| 2 | ISO/IEC 25019 | 2023 | Quality-in-Use Model | Mengevaluasi kualitas aplikasi dari perspektif pengguna |
| 3 | ISO/IEC 25002 | 2024 | Quality Model Overview and Usage | Memberikan panduan penggunaan quality model dalam evaluasi aplikasi |
| 4 | ISO/IEC/IEEE 29119-5 | 2024 | Keyword-Driven Testing | Referensi tambahan untuk pengorganisasian test case berbasis keyword |

## 3. ISO/IEC 25010:2023

**Judul resmi:**

*Systems and software engineering — Systems and software Quality Requirements and Evaluation (SQuaRE) — Product quality model*

ISO/IEC 25010:2023 mendefinisikan model kualitas produk yang dapat digunakan untuk menentukan, mengukur, dan mengevaluasi kualitas produk ICT dan perangkat lunak.

Standar ini digunakan sebagai referensi utama dalam menentukan aspek kualitas yang relevan terhadap pengujian Jetprint.id.

Karakteristik yang diprioritaskan dalam proyek ini adalah:

### 3.1 Functional Suitability

Functional Suitability digunakan untuk mengevaluasi apakah fungsi yang tersedia mampu memenuhi kebutuhan pengguna.

Penerapannya mencakup:

- Kesesuaian fungsi navigasi.
- Kesesuaian informasi pada katalog dan detail produk.
- Fungsi konfigurasi produk.
- Fungsi perhitungan harga.
- Fungsi registrasi dan login.
- Fungsi upload desain.
- Fungsi keranjang belanja.
- Fungsi pelacakan pesanan.

### 3.2 Interaction Capability

Interaction Capability digunakan untuk mengevaluasi kemudahan pengguna dalam berinteraksi dengan website.

Penerapannya mencakup:

- Kejelasan menu dan navigasi.
- Kemudahan memahami informasi produk.
- Kejelasan label dan pesan validasi.
- Kemudahan mengisi form.
- Kemudahan menyelesaikan alur penggunaan yang diuji.

### 3.3 Compatibility

Compatibility dipertimbangkan secara terbatas untuk melihat apakah fungsi utama dapat digunakan pada environment pengujian yang ditentukan.

Pengujian compatibility hanya dilakukan jika kelompok menggunakan lebih dari satu browser atau perangkat. Detail browser dan perangkat akan dicatat pada saat test execution.

### 3.4 Reliability

Reliability dipertimbangkan secara terbatas berdasarkan konsistensi fungsi ketika test case dijalankan.

Proyek ini tidak mencakup reliability testing yang membutuhkan akses server, monitoring internal, pengujian dalam jangka panjang, atau pemberian beban tinggi terhadap sistem.

**Referensi resmi:**

https://www.iso.org/standard/78176.html

## 4. ISO/IEC 25019:2023

**Judul resmi:**

*Systems and software engineering — Systems and software Quality Requirements and Evaluation (SQuaRE) — Quality-in-use model*

ISO/IEC 25019:2023 mendefinisikan model quality-in-use untuk menentukan, mengukur, mengevaluasi, dan meningkatkan kualitas ketika suatu produk atau sistem digunakan dalam konteks penggunaan tertentu.

Dalam proyek ini, konteks penggunaannya adalah pengguna website layanan digital printing yang melakukan aktivitas melalui browser, seperti:

- Mencari produk.
- Membuka kategori produk.
- Melihat detail produk.
- Mengatur spesifikasi produk.
- Mengunggah desain.
- Menambahkan produk ke keranjang.
- Melakukan registrasi atau login.
- Mengakses informasi pemesanan.

Penerapan standar ini dibatasi pada pengamatan dari sisi pengguna. Kelompok tidak melakukan pengukuran terhadap proses internal, server, database, atau infrastruktur Jetprint.

**Referensi resmi:**

https://www.iso.org/standard/78177.html

## 5. ISO/IEC 25002:2024

**Judul resmi:**

*Systems and software engineering — Systems and software Quality Requirements and Evaluation (SQuaRE) — Quality model overview and usage*

ISO/IEC 25002:2024 memberikan kerangka untuk mendefinisikan dan menggunakan quality model yang terdiri dari karakteristik dan subkarakteristik kualitas.

Standar ini digunakan untuk membantu kelompok dalam:

- Memilih karakteristik kualitas yang sesuai dengan scope proyek.
- Menghubungkan karakteristik kualitas dengan fitur yang diuji.
- Menentukan tujuan evaluasi.
- Menyusun expected result berdasarkan perilaku aplikasi yang diharapkan.
- Menghindari pengujian aspek kualitas yang tidak dapat dievaluasi dengan akses yang tersedia.

Proyek tidak menggunakan seluruh karakteristik secara sekaligus. Karakteristik dipilih berdasarkan relevansinya dengan website Jetprint.id, jenis pengujian, akses kelompok, serta batasan pengujian pada production/public website.

**Referensi resmi:**

https://www.iso.org/standard/78175.html

## 6. ISO/IEC/IEEE 29119-5:2024

**Judul resmi:**

*Software and systems engineering — Software testing — Part 5: Keyword-driven testing*

ISO/IEC/IEEE 29119-5:2024 membahas pendekatan Keyword-Driven Testing, termasuk penggunaan keyword untuk menyusun spesifikasi pengujian secara modular dan konsisten.

Standar ini digunakan sebagai referensi tambahan, bukan sebagai pendekatan utama proyek.

Jika pendekatan keyword-driven diterapkan, contoh keyword yang dapat digunakan antara lain:

- `OPEN_PAGE`
- `CLICK_MENU`
- `SELECT_PRODUCT`
- `INPUT_DATA`
- `UPLOAD_FILE`
- `ADD_TO_CART`
- `CHECK_VALUE`
- `VERIFY_MESSAGE`

Penggunaan keyword dapat membantu menjaga konsistensi penulisan action dan expected result pada test case. Namun, implementasinya bersifat opsional dan disesuaikan dengan kebutuhan kelompok.

Proyek ini tidak mengklaim menerapkan seluruh requirement, framework, tool integration, maupun automation yang dibahas dalam ISO/IEC/IEEE 29119-5:2024.

**Referensi resmi:**

https://www.iso.org/standard/87233.html

https://standards.ieee.org/ieee/29119-5/11042/

## 7. Penerapan Standar pada Proyek

| Area Proyek | Referensi | Penerapan |
|---|---|---|
| Penentuan aspek kualitas | ISO/IEC 25010:2023 | Memilih karakteristik kualitas yang relevan untuk Jetprint.id |
| Evaluasi fungsi aplikasi | ISO/IEC 25010:2023 | Fokus pada Functional Suitability |
| Evaluasi dari sisi pengguna | ISO/IEC 25019:2023 | Menentukan konteks penggunaan website |
| Penyusunan tujuan evaluasi | ISO/IEC 25002:2024 | Menghubungkan quality model, fitur, dan tujuan pengujian |
| Penyusunan test scenario | ISO/IEC 25002:2024 | Mengelompokkan pengujian berdasarkan fitur dan kualitas |
| Penulisan langkah pengujian | ISO/IEC/IEEE 29119-5:2024 | Referensi opsional penggunaan keyword yang konsisten |
| Pelaksanaan pengujian | ISO/IEC 25010:2023 dan ISO/IEC 25019:2023 | Membandingkan expected result dengan actual result |
| Test summary | ISO/IEC 25010:2023 | Merangkum kualitas berdasarkan hasil pengujian yang benar-benar dilakukan |

## 8. Hubungan dengan Dokumen Repository

| Dokumen | Hubungan dengan Referensi |
|---|---|
| `application-overview.md` | Menjelaskan aplikasi dan konteks penggunaannya |
| `feature-list.md` | Menentukan fitur yang dapat dievaluasi |
| `test-plan.md` | Menetapkan tujuan, scope, quality characteristics, metode, dan batasan |
| `test-scenarios.md` | Menghubungkan fitur dengan kondisi yang perlu diuji |
| `test-cases.md` | Mendokumentasikan langkah, data, dan expected result |
| `test-execution-report.md` | Mencatat actual result dan status pelaksanaan |
| `bug-report.md` | Mendokumentasikan ketidaksesuaian yang telah diverifikasi |
| `test-summary-report.md` | Merangkum hasil pengujian dan evaluasi kualitas |

## 9. Batasan Penerapan

Penerapan standar pada proyek ini disesuaikan dengan ruang lingkup tugas akademik dan kondisi objek pengujian.

Batasan penerapannya meliputi:

1. Kelompok hanya memiliki akses dari sisi pengguna.
2. Pengujian dilakukan terhadap production/public website.
3. Kelompok tidak memiliki akses terhadap source code, database, server, log internal, dan dashboard administrator.
4. Tidak semua karakteristik kualitas dapat dievaluasi.
5. Pengujian tidak mencakup penetration testing, load testing, dan stress testing.
6. ISO/IEC/IEEE 29119-5:2024 hanya digunakan apabila pendekatan Keyword-Driven Testing diterapkan.
7. Proyek tidak mengklaim menerapkan seluruh requirement pada setiap standar.

## 10. Catatan Tahun Referensi

Seluruh standar yang dicantumkan dalam dokumen ini diterbitkan dalam rentang tahun 2023–2026.

Dokumen ini tidak mencantumkan ISO/IEC/IEEE 29119 Part 1 sampai Part 4 karena edisi aktif yang sebelumnya ditemukan berada di luar batas tahun referensi tugas.

Pembatasan tahun tersebut menyebabkan referensi untuk proses, dokumentasi, dan teknik pengujian tidak menggunakan Part 1 sampai Part 4. Struktur dokumen proyek disusun sesuai kebutuhan tugas dan diperkuat menggunakan model kualitas SQuaRE serta ISO/IEC/IEEE 29119-5:2024 sebagai referensi tambahan.

## 11. Official References

1. ISO/IEC 25010:2023  
   https://www.iso.org/standard/78176.html

2. ISO/IEC 25019:2023  
   https://www.iso.org/standard/78177.html

3. ISO/IEC 25002:2024  
   https://www.iso.org/standard/78175.html

4. ISO/IEC/IEEE 29119-5:2024  
   https://www.iso.org/standard/87233.html

5. IEEE Standards Association — IEEE/ISO/IEC 29119-5-2024  
   https://standards.ieee.org/ieee/29119-5/11042/