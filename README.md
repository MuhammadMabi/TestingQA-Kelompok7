# Financial Accounting Management System - Software Testing & Quality Assurance

![Course](https://img.shields.io/badge/Mata_Kuliah-Testing%20%26%20QA-blue)
![Semester](https://img.shields.io/badge/Semester-7-green)
![Tahun](https://img.shields.io/badge/Tahun-2026-orange)
![Application](https://img.shields.io/badge/Application-FAMS-696CFF)
![Framework](https://img.shields.io/badge/Framework-Laravel-FF2D20)
![Company](https://img.shields.io/badge/Company-PT%20Dinamika%20Solusi%20Informatika-0078D4)

## Tentang Proyek

Repository ini berisi dokumentasi dan kegiatan pengujian perangkat lunak terhadap **Financial Accounting Management System (FAMS)**, yaitu aplikasi akuntansi berbasis web yang dikembangkan menggunakan Laravel untuk mendukung pengelolaan transaksi dan penyusunan laporan keuangan.

Aplikasi digunakan sebagai objek pengujian atas nama **PT Dinamika Solusi Informatika** dan dapat diakses melalui:

**[https://fams.dinamika-si.com](https://fams.dinamika-si.com)**

Proyek pengujian ini dibuat untuk memenuhi tugas mata kuliah **Testing dan QA Perangkat Lunak** pada semester 7, Program Studi Teknik Informatika, Universitas Pamulang.

## Tujuan Proyek

Proyek ini bertujuan untuk:

- Memverifikasi kesesuaian fungsi aplikasi dengan kebutuhan sistem akuntansi.
- Memastikan proses pencatatan transaksi mengikuti prinsip double-entry accounting.
- Memastikan total debit dan kredit pada jurnal selalu seimbang.
- Menguji validasi input, business rules, dan kontrol akses pengguna.
- Memastikan transaksi yang telah diposting menghasilkan informasi keuangan yang sesuai.
- Mengidentifikasi, mencatat, dan mengelola defect yang ditemukan.
- Menyusun dan menjalankan test scenario serta test case.
- Mendokumentasikan hasil pengujian secara terstruktur.
- Melakukan regression testing terhadap fitur yang telah diperbaiki.
- Menerapkan automation testing pada fungsi yang sesuai.
- Menerapkan referensi standar IEEE dan ISO/IEC/IEEE yang relevan.
- Melakukan wawancara dengan profesional yang memiliki pengalaman di bidang Software Testing atau Quality Assurance.

## Objek Pengujian

| Informasi | Keterangan |
|---|---|
| Nama Aplikasi | Financial Accounting Management System |
| Akronim | FAMS |
| Website | [https://fams.dinamika-si.com](https://fams.dinamika-si.com) |
| Perusahaan | PT Dinamika Solusi Informatika |
| Jenis Aplikasi | Web-based Financial Accounting System |
| Framework | Laravel |
| Database | MySQL |
| Platform | Web |
| Metode Utama | Black Box Testing dan Functional Testing |
| Kategori Proyek | Akademik |
| Test Level | System Testing |
| Test Environment | Web Application Testing Environment |

## Deskripsi Aplikasi

**Financial Accounting Management System (FAMS)** merupakan aplikasi berbasis web yang digunakan untuk mengelola proses pencatatan akuntansi, mulai dari pengaturan Chart of Accounts, tahun fiskal, periode akuntansi, pencatatan jurnal, posting transaksi, hingga penyusunan laporan keuangan.

Aplikasi menerapkan prinsip **double-entry accounting**, sehingga setiap jurnal harus memiliki jumlah debit dan kredit yang seimbang sebelum dapat diposting. Transaksi yang telah diposting digunakan sebagai sumber data General Ledger, Trial Balance, Profit and Loss, dan Balance Sheet.

FAMS juga memiliki pengelolaan pengguna berbasis **Role-Based Access Control (RBAC)**, audit trail, pengaturan aplikasi, dan dashboard untuk menyajikan ringkasan aktivitas keuangan.

## Pengguna Aplikasi

FAMS memiliki beberapa kelompok pengguna:

| Role | Tanggung Jawab Utama |
|---|---|
| Administrator | Mengelola pengguna, role, permission, konfigurasi, dan seluruh fungsi aplikasi |
| Finance Staff | Membuat dan mengelola jurnal sebelum diposting |
| Finance Manager | Melakukan review, mengelola periode, dan memposting jurnal |
| Auditor | Melihat transaksi, laporan keuangan, dan audit log |

Hak akses setiap pengguna ditentukan melalui role dan permission yang diberikan oleh Administrator.

## Ruang Lingkup Pengujian

Pengujian difokuskan pada fitur-fitur berikut:

- Authentication dan logout.
- Dashboard dan ringkasan aktivitas keuangan.
- Chart of Accounts.
- Fiscal Year.
- Accounting Period.
- General Journal.
- Journal Entry Lines.
- Validasi keseimbangan debit dan kredit.
- Journal posting.
- General Ledger.
- Trial Balance.
- Profit and Loss.
- Balance Sheet.
- User Management.
- Roles and Permissions.
- Role-Based Access Control.
- Audit Logs.
- Application Settings.
- User Profile.
- Validasi input dan business rules.
- Tampilan responsif pada browser desktop dan mobile.

## Aturan Bisnis Utama yang Diuji

Beberapa aturan bisnis penting dalam FAMS meliputi:

1. Setiap jurnal harus memiliki minimal dua baris transaksi.
2. Setiap baris jurnal hanya dapat memiliki nilai debit atau kredit, bukan keduanya.
3. Total debit dan total kredit harus seimbang sebelum jurnal dapat diposting.
4. Jurnal hanya dapat dibuat pada periode akuntansi yang masih terbuka.
5. Hanya akun aktif dan akun posting yang dapat digunakan pada jurnal.
6. Jurnal berstatus draft masih dapat diubah sesuai permission pengguna.
7. Jurnal yang telah diposting tidak dapat diubah atau dihapus secara langsung.
8. Hanya pengguna dengan permission `journal-post` yang dapat memposting jurnal.
9. Laporan keuangan hanya menggunakan jurnal yang telah diposting.
10. Setiap aktivitas penting harus tercatat pada Audit Logs.
11. Menu, route, dan action harus mengikuti role dan permission pengguna.
12. Pengguna tidak boleh menonaktifkan atau menghapus akun sendiri melalui User Management.

## Metode Pengujian

Metode pengujian yang digunakan meliputi:

- **Black Box Testing**  
  Menguji fungsi aplikasi berdasarkan input dan output tanpa bergantung pada detail implementasi internal.

- **Functional Testing**  
  Memastikan setiap fitur bekerja sesuai kebutuhan dan business rules yang telah ditentukan.

- **Integration Testing**  
  Memastikan integrasi antara jurnal, Chart of Accounts, Accounting Period, General Ledger, dan laporan keuangan berjalan sesuai harapan.

- **System Testing**  
  Menguji FAMS sebagai satu kesatuan sistem dari perspektif pengguna.

- **Equivalence Partitioning**  
  Membagi data input ke dalam kelompok valid dan tidak valid.

- **Boundary Value Analysis**  
  Menguji nilai pada batas minimum, maksimum, sebelum batas, dan setelah batas.

- **Negative Testing**  
  Menguji respons aplikasi terhadap input tidak valid, akses tanpa izin, dan pelanggaran business rules.

- **Role-Based Access Testing**  
  Memastikan setiap role hanya dapat mengakses menu, route, dan action sesuai permission.

- **Regression Testing**  
  Memastikan perbaikan atau perubahan fitur tidak merusak fungsi yang sebelumnya telah berjalan.

- **User Acceptance Testing**  
  Mengevaluasi kesesuaian fungsi aplikasi dengan kebutuhan penggunaan sistem akuntansi.

- **Automation Testing**  
  Mengotomatisasi skenario yang stabil dan berulang menggunakan tools yang dipilih pada tahap automation testing.

## Fokus Pengujian Kritis

Prioritas pengujian diberikan pada area yang berpotensi memengaruhi integritas data keuangan:

| Area | Risiko Utama |
|---|---|
| General Journal | Jurnal tidak seimbang atau baris transaksi tidak valid |
| Journal Posting | Transaksi tidak valid masuk ke laporan keuangan |
| Accounting Period | Transaksi dibuat pada periode yang sudah ditutup |
| General Ledger | Saldo akun tidak sesuai dengan jurnal yang diposting |
| Trial Balance | Total debit dan kredit tidak seimbang |
| Profit and Loss | Pendapatan atau beban tidak dihitung dengan benar |
| Balance Sheet | Persamaan aset, liabilitas, dan ekuitas tidak seimbang |
| RBAC | Pengguna menjalankan action di luar kewenangannya |
| Audit Logs | Aktivitas penting tidak tercatat |
| User Management | Perubahan akses atau status pengguna tidak terkontrol |

## Test Environment

Pengujian **Financial Accounting Management System (FAMS)** dilakukan pada local development environment sebelum aplikasi digunakan pada environment deployment.

| Komponen | Environment |
|---|---|
| Application | Financial Accounting Management System |
| Organization | PT Dinamika Solusi Informatika |
| Deployment URL | https://fams.dinamika-si.com |
| Test Environment | Local Development Environment |
| Test URL | http://127.0.0.1:8000 (localhost)|
| Platform | Web |
| Backend Framework | Laravel |
| Database | MySQL |
| Primary Browser | Google Chrome |
| Additional Browser | Microsoft Edge |
| Network | Localhost / Local Network |
| Access | Testing accounts berdasarkan role |
| Test Data | Data khusus pengujian |

Pengujian utama dilakukan melalui **localhost** menggunakan environment pengembangan lokal. Testing menggunakan data khusus pengujian sehingga proses seperti pembuatan jurnal, posting jurnal, perubahan periode akuntansi, pengujian role dan permission, serta pengujian data keuangan tidak memengaruhi data pada environment deployment.

Detail tambahan seperti versi browser, operating system, versi PHP, Laravel, MySQL, serta build atau commit aplikasi yang diuji akan dicatat pada saat test execution.

## Test Data

Test data yang digunakan antara lain:

- Akun Administrator.
- Akun Finance Staff.
- Akun Finance Manager.
- Akun Auditor.
- Chart of Accounts khusus testing.
- Fiscal Year dan Accounting Period khusus testing.
- Jurnal seimbang.
- Jurnal tidak seimbang.
- Jurnal dengan baris debit dan kredit yang tidak valid.
- Transaksi pada periode terbuka.
- Transaksi pada periode tertutup.
- Input form valid dan tidak valid.
- Data nominal pada batas pengujian.
- Credential valid dan invalid.

Data produksi yang sensitif tidak digunakan sebagai test data. Bukti pengujian harus menyembunyikan password, token, dan informasi rahasia lainnya.

## Referensi

Pengujian menggunakan konsep dan dokumentasi yang relevan dari standar berikut:

- ISO/IEC/IEEE 29119-5 - Keyword-Driven Testing (2024).
- IEEE 730 - Software Quality Assurance Processes (2026).

Tahun edisi, status publikasi, dan penggunaan setiap referensi akan dicatat secara konsisten pada dokumen `ieee-iso-references.md`.

## Struktur Repository

```text
TestingQA-Kelompok7/
│
├── 01-object-under-test/
│   ├── application-overview.md
│   └── feature-list.csv
│
├── 02-standards-and-references/
│   └── ieee-iso-references.md
│
├── 03-test-plan/
│   └── test-plan.md
│
├── 04-test-design/
│   ├── test-scenarios.md
│   ├── test-cases.md
│   ├── test-data.csv
│   └── requirements-traceability-matrix.csv
│
├── 05-test-execution/
│   ├── test-execution-report.md
│   └── screenshots/
│
├── 06-bug-management/
│   ├── bug-report.md
│   └── screenshots/
│
├── 07-testing-types/
│   ├── functional-testing.md
│   ├── integration-testing.md
│   ├── regression-testing.md
│   ├── rbac-testing.md
│   └── user-acceptance-testing.md
│
├── 08-automation-testing/
│   ├── README.md
│   └── tests/
│
├── 09-qa-consultation/
│   ├── question.md
│   ├── qa-consultation.md
│   └── consultation-evidence/
│
├── 10-test-summary/
│   └── test-summary-report.md
│
├── docs/
│   └── screenshots/
│
├── .gitignore
│
└── README.md
```

## Status Pengujian

Status yang digunakan selama test execution:

| Status | Definisi |
|---|---|
| Not Executed | Test case belum dijalankan |
| Pass | Actual Result sesuai dengan Expected Result |
| Fail | Actual Result tidak sesuai dengan Expected Result |
| Blocked | Test case tidak dapat dijalankan karena dependency atau batasan tertentu |
| Not Applicable | Test case tidak relevan terhadap build atau kondisi pengujian |

## Defect Classification

Defect diklasifikasikan berdasarkan severity:

| Severity | Keterangan |
|---|---|
| Critical | Menyebabkan kerusakan data keuangan, akses tidak sah, atau aplikasi tidak dapat digunakan |
| High | Fungsi utama akuntansi gagal dan tidak tersedia workaround yang layak |
| Medium | Fungsi terganggu tetapi masih tersedia workaround |
| Low | Masalah minor pada tampilan, teks, atau usability |

Contoh defect Critical atau High meliputi:

- Jurnal tidak seimbang dapat diposting.
- Jurnal pada periode tertutup dapat dibuat atau diposting.
- Pengguna tanpa permission dapat memposting jurnal.
- Trial Balance menghasilkan debit dan kredit yang tidak seimbang.
- Balance Sheet tidak memenuhi persamaan dasar akuntansi akibat kesalahan perhitungan.
- Jurnal yang telah diposting dapat diubah tanpa kontrol atau audit trail.

## Anggota Kelompok

| No. | Nama | NIM |
|---|---|---|
| 1 | Muhammad Mabi Palaka | 231011401691 |
| 2 | Muhammad Raffi | 231011401441 |
| 3 | Muhammad Gifary Nezar | 231011401241 |
| 4 | Muhammad Fariz | 231011400080 |

---

**Mata Kuliah:** Testing dan QA Perangkat Lunak  
**Program Studi:** Teknik Informatika - Semester 7  
**Universitas:** Universitas Pamulang  
**Tahun Akademik:** 2026  
**Objek Pengujian:** Financial Accounting Management System  
**Perusahaan:** PT Dinamika Solusi Informatika  

Proyek ini dilaksanakan untuk keperluan akademik dan pembelajaran. Pengujian pada environment perusahaan dilakukan menggunakan akun, data, dan akses yang telah diizinkan.