# Test Plan

## 1. Informasi Pengujian

| Informasi | Keterangan |
|---|---|
| Project | UMKM Software Testing |
| Object Under Test | Jetprint.id |
| Application Type | Web Application / E-Commerce Digital Printing |
| Test Level | System Testing dari perspektif pengguna |
| Testing Approach | Black Box & Functional Testing |
| Primary Standard Reference | ISO/IEC/IEEE 29119 |
| Repository | UMKM-Software-Testing |

## 2. Tujuan Pengujian

Pengujian dilakukan untuk mengevaluasi fungsi utama website Jetprint.id dari sisi pengguna dan memastikan fitur yang termasuk dalam ruang lingkup pengujian dapat memberikan hasil sesuai dengan perilaku yang diharapkan.

Tujuan pengujian meliputi:

- Memverifikasi fungsi utama website.
- Memastikan navigasi dan alur penggunaan berjalan dengan benar.
- Memeriksa validasi terhadap input pengguna.
- Memeriksa fungsi konfigurasi produk dan perhitungan harga.
- Membandingkan expected result dengan actual result.
- Mengidentifikasi defect apabila ditemukan selama proses pengujian.
- Mendokumentasikan proses dan hasil pengujian secara terstruktur.

## 3. Object Under Test

Objek pengujian adalah website **Jetprint.id**:

https://jetprint.id

Pengujian dilakukan terhadap website publik dari perspektif pengguna tanpa mengakses source code, database, server, dashboard administrator, atau sistem internal Jetprint.

Detail objek pengujian:

- `../01-object-under-test/application-overview.md`
- `../01-object-under-test/feature-list.md`

## 4. Test Scope

### 4.1 In Scope

| ID | Fitur |
|---|---|
| F-01 | Homepage |
| F-02 | Navigation |
| F-03 | Product Catalog |
| F-04 | Product Category |
| F-05 | Product Detail |
| F-06 | Product Configuration |
| F-07 | Price Calculation |
| F-08 | Design Upload Validation |
| F-09 | Design Link Input |
| F-10 | Add to Cart |
| F-11 | Shopping Cart |
| F-12 | User Registration |
| F-13 | User Login |
| F-16 | Promo & Coupon |
| F-21 | Order Tracking |
| F-24 | FAQ |
| F-25 | Cara Order |
| F-29 | Kalkulator Potongan |

### 4.2 Need Permission

| ID | Fitur | Batasan |
|---|---|---|
| F-14 | Guest Checkout | Jangan submit pesanan tanpa izin |
| F-15 | Checkout Validation | Batasi sebelum pembuatan order |
| F-17 | Payment | Berhubungan dengan transaksi finansial |
| F-18 | Shipping | Dapat berkaitan dengan transaksi nyata |
| F-19 | Store Pickup | Jangan membuat order tanpa izin |
| F-20 | Order Creation | Dapat menghasilkan pesanan nyata |
| F-22 | Order History | Membutuhkan order/account yang sesuai |
| F-23 | Product Review | Dapat menghasilkan data publik |

Tanpa izin dari pihak Jetprint, pengujian fitur tersebut dibatasi pada observasi atau validasi yang tidak menghasilkan transaksi dan tidak memengaruhi data operasional.

### 4.3 Out of Scope

| ID | Fitur |
|---|---|
| F-26 | Blog & Tips |
| F-27 | Tentang Kami |
| F-28 | Karir |
| F-30 | WhatsApp / Chat Sales |
| F-31 | Admin / Back Office |
| F-32 | Security / Penetration Testing |
| F-33 | Performance / Stress Testing |

Selain fitur tersebut, database, server, API internal, source code, dan infrastruktur internal Jetprint juga tidak termasuk dalam ruang lingkup pengujian.

## 5. Test Approach

### 5.1 Black Box Testing

Pengujian dilakukan dari perspektif pengguna tanpa mengetahui implementasi atau struktur source code Jetprint.id.

Tester memberikan input melalui antarmuka website kemudian membandingkan actual result dengan expected result yang telah ditentukan pada test case.

### 5.2 Functional Testing

Functional Testing digunakan untuk memeriksa apakah fungsi aplikasi bekerja sesuai dengan perilaku yang diharapkan.

Contoh fungsi yang diuji:

- Navigasi halaman.
- Katalog dan kategori produk.
- Detail produk.
- Konfigurasi produk.
- Perhitungan harga.
- Registrasi dan login.
- Upload desain.
- Keranjang belanja.
- Pelacakan pesanan.

### 5.3 Equivalence Partitioning

Equivalence Partitioning digunakan pada input yang dapat dikelompokkan menjadi kelas data valid dan invalid.

Kandidat penerapan antara lain:

- Format file desain.
- Input login.
- Input registrasi.
- Link desain.
- Quantity produk.

Test data final ditentukan berdasarkan rule yang benar-benar ditemukan pada website.

### 5.4 Boundary Value Analysis

Boundary Value Analysis digunakan pada input yang memiliki batas minimum atau maksimum.

Kandidat penerapan:

- Batas ukuran file upload.
- Minimum dan maksimum quantity produk.
- Batas panjang input apabila tersedia.

Teknik hanya diterapkan jika batas nilai dapat diidentifikasi.

### 5.5 Negative Testing

Negative Testing digunakan untuk memverifikasi respons aplikasi ketika menerima input yang tidak sesuai.

Contohnya:

- Login dengan credential yang salah.
- Required field dikosongkan.
- Format input tidak valid.
- Upload file yang tidak didukung.
- Input di luar batas yang diperbolehkan.

Negative Testing tidak digunakan untuk eksploitasi keamanan atau aktivitas yang dapat mengganggu layanan.

### 5.6 Regression Testing

Regression Testing dilakukan apabila terdapat kondisi yang memungkinkan dilakukannya retest terhadap fungsi yang sebelumnya telah diuji.

Karena kelompok tidak memiliki akses terhadap deployment Jetprint.id, Regression Testing hanya dilakukan apabila terdapat perubahan aplikasi yang dapat diamati selama periode pengujian.

## 6. Test Environment

| Komponen | Environment |
|---|---|
| Application | Jetprint.id |
| Environment | Production / Public Website |
| Platform | Web |
| Primary Browser | Google Chrome |
| Network | Public Internet Connection |

Versi browser, operating system, perangkat, dan detail environment lainnya akan dicatat saat test execution dilakukan.

## 7. Test Data

Test data disiapkan berdasarkan kebutuhan masing-masing test case.

Data yang dapat digunakan antara lain:

- Akun khusus testing.
- Credential valid dan invalid.
- File dummy untuk pengujian upload.
- Link dummy yang aman.
- Quantity produk.
- Konfigurasi produk.
- Data form valid dan invalid.
- Kode promo yang tersedia secara publik.
- Kode pesanan yang diperoleh secara sah.

Test data disimpan pada:

`../04-test-cases/test-data.csv`

Data pribadi pengguna lain tidak digunakan sebagai test data.

## 8. Entry Criteria

Testing dapat dimulai apabila:

- Website Jetprint.id dapat diakses.
- Scope testing telah ditentukan.
- Feature list tersedia.
- Test scenario telah dibuat.
- Test case untuk fitur yang akan diuji tersedia.
- Test data yang diperlukan tersedia.
- Fitur yang membutuhkan izin tidak dieksekusi tanpa izin.

## 9. Exit Criteria

Siklus testing dapat diselesaikan apabila:

- Seluruh test case yang termasuk dalam scope telah dieksekusi atau diberikan status yang sesuai.
- Actual result telah dicatat.
- Status setiap test case telah ditentukan.
- Evidence yang diperlukan telah tersedia.
- Defect yang ditemukan telah didokumentasikan.
- Test summary report telah dibuat.

Test case yang tidak dapat dieksekusi karena izin, dependency, atau kondisi environment dicatat sebagai `Blocked` beserta alasannya.

## 10. Test Execution Status

| Status | Definisi |
|---|---|
| Not Executed | Test case belum dijalankan |
| Pass | Actual result sesuai expected result |
| Fail | Actual result tidak sesuai expected result |
| Blocked | Test case tidak dapat dieksekusi karena batasan tertentu |

## 11. Defect Management

Test case dengan status `Fail` akan dianalisis sebelum dicatat sebagai defect.

Defect yang telah diverifikasi akan didokumentasikan pada:

`../06-bug-reports/bug-report.md`

Informasi defect minimal meliputi:

- Bug ID.
- Title.
- Related Feature.
- Environment.
- Precondition.
- Steps to Reproduce.
- Expected Result.
- Actual Result.
- Severity.
- Evidence.
- Status.

Status `Fail` pada test case tidak otomatis dianggap sebagai bug sebelum hasilnya diverifikasi.

## 12. Evidence

Evidence digunakan untuk mendokumentasikan pelaksanaan pengujian.

Screenshot hasil testing akan disimpan pada:

`../05-test-execution/screenshots/`

Evidence hanya dibuat berdasarkan hasil test execution yang benar-benar dilakukan.

## 13. Risks and Limitations

Beberapa risiko dan batasan dalam proses pengujian:

1. Jetprint.id merupakan sistem milik pihak eksternal.
2. Kelompok tidak memiliki akses terhadap source code dan sistem internal.
3. Website produksi dapat berubah selama periode testing.
4. Beberapa fitur dapat menghasilkan transaksi nyata.
5. Beberapa test case mungkin membutuhkan izin dari Jetprint.
6. Ketersediaan website dan koneksi internet dapat memengaruhi testing.
7. Kelompok tidak memiliki kontrol terhadap deployment atau perubahan aplikasi.

## 14. Test Deliverables

Dokumentasi yang dihasilkan dalam proses pengujian:

| Deliverable | Lokasi |
|---|---|
| Application Overview | `01-object-under-test/application-overview.md` |
| Feature List | `01-object-under-test/feature-list.md` |
| IEEE/ISO References | `02-standards-and-references/ieee-iso-references.md` |
| Supporting Journals | `02-standards-and-references/supporting-journals.md` |
| Test Plan | `03-test-plan/test-plan.md` |
| Test Scenarios | `04-test-cases/test-scenarios.md` |
| Test Cases | `04-test-cases/test-cases.md` |
| Test Data | `04-test-cases/test-data.csv` |
| Test Execution | `05-test-execution/test-execution-report.md` |
| Bug Report | `06-bug-reports/bug-report.md` |
| QA Consultation | `07-qa-consultation/hasil-wawancara-qa.md` |
| Test Summary | `08-test-summary/test-summary-report.md` |

## 15. References

Test plan disusun dengan mempertimbangkan konsep yang relevan dari ISO/IEC/IEEE 29119 Series.

Referensi utama yang termasuk rentang tahun tugas:

- ISO/IEC/IEEE 29119-5:2024 — Keyword-Driven Testing.

Referensi dasar tambahan:

- ISO/IEC/IEEE 29119-1:2022 — General Concepts.
- ISO/IEC/IEEE 29119-2:2021 — Test Processes.
- ISO/IEC/IEEE 29119-3:2021 — Test Documentation.
- ISO/IEC/IEEE 29119-4:2021 — Test Techniques.

Penerapan standar disesuaikan dengan kebutuhan proyek akademik dan tidak dimaksudkan sebagai implementasi penuh seluruh proses ISO/IEC/IEEE 29119.