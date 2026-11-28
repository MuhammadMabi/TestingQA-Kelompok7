# Application Overview

## 1. Informasi Aplikasi

| Informasi | Keterangan |
|---|---|
| Nama Aplikasi | Financial Accounting Management System (FAMS) |
| Organisasi | PT Dinamika Solusi Informatika |
| Deployment URL | https://fams.dinamika-si.com |
| Test Environment | Local Development Environment |
| Platform | Web |
| Framework | Laravel |
| Database | MySQL |
| Jenis Aplikasi | Financial Accounting Management System |

## 2. Deskripsi Aplikasi

**Financial Accounting Management System (FAMS)** merupakan aplikasi berbasis web untuk membantu proses pencatatan dan pengelolaan transaksi keuangan sampai dengan penyusunan laporan keuangan.

Sistem menerapkan prinsip **double-entry accounting**, sehingga transaksi jurnal harus memiliki total debit dan kredit yang seimbang sebelum dapat diposting.

## 3. Pengguna Aplikasi

FAMS memiliki beberapa role pengguna:

- **Administrator** – mengelola pengguna, role, permission, dan konfigurasi aplikasi.
- **Finance Staff** – melakukan pencatatan dan pengelolaan transaksi jurnal.
- **Finance Manager** – melakukan review serta posting transaksi.
- **Auditor** – melakukan pemeriksaan transaksi, laporan, dan audit log.

Hak akses fitur dan tindakan pada aplikasi dikendalikan menggunakan **Role-Based Access Control (RBAC)**.

## 4. Fitur Utama

Fitur utama FAMS meliputi:

- Dashboard
- Chart of Accounts
- Fiscal Year
- Accounting Period
- General Journal
- General Ledger
- Trial Balance
- Profit and Loss
- Balance Sheet
- User Management
- Roles and Permissions
- Audit Logs
- Application Settings
- User Profile

## 5. Alur Utama Sistem

Proses akuntansi dimulai dari pengaturan **Chart of Accounts**, Fiscal Year, dan Accounting Period. Pengguna kemudian membuat Journal Entry dengan menentukan akun serta nilai debit dan kredit.

Jurnal yang valid dan seimbang dapat diposting. Transaksi yang telah diposting menjadi dasar pembentukan **General Ledger, Trial Balance, Profit and Loss, dan Balance Sheet**.

## 6. Tujuan Pengujian

Pengujian dilakukan untuk memastikan fungsi FAMS berjalan sesuai kebutuhan, business rules akuntansi diterapkan dengan benar, serta akses terhadap fitur sesuai dengan role dan permission pengguna.

Pengujian utama dilakukan pada **local development environment** menggunakan data khusus pengujian agar tidak memengaruhi data pada deployment aplikasi.