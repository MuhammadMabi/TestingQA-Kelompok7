# Test Plan

## 1. Tujuan

Pengujian dilakukan untuk memastikan **Financial Accounting Management System (FAMS)** berjalan sesuai fungsi dan business rules yang ditetapkan, serta dapat menghasilkan proses pencatatan dan laporan keuangan yang sesuai.

## 2. Ruang Lingkup

Pengujian mencakup fitur utama FAMS:

- Authentication dan Dashboard
- Chart of Accounts
- Fiscal Year dan Accounting Period
- General Journal dan Journal Posting
- General Ledger
- Trial Balance
- Profit and Loss
- Balance Sheet
- User Management
- Roles and Permissions
- Audit Logs
- Application Settings dan User Profile

## 3. Metode Pengujian

Metode yang digunakan meliputi:

- **Black Box Testing**
- **Functional Testing**
- **Integration Testing**
- **Negative Testing**
- **Regression Testing**
- **Role-Based Access Testing**
- **Automation Testing**

Teknik seperti **Equivalence Partitioning** dan **Boundary Value Analysis** digunakan pada fitur yang memiliki input dan batas nilai yang sesuai.

## 4. Test Environment

| Komponen | Environment |
|---|---|
| Application | Financial Accounting Management System |
| Environment | Local Development |
| Platform | Web |
| Backend | Laravel |
| Database | MySQL |
| Browser | Google Chrome dan Microsoft Edge |
| Test Data | Data khusus pengujian |

## 5. Kriteria Pengujian

Test case dinyatakan:

- **Pass** apabila actual result sesuai dengan expected result.
- **Fail** apabila actual result tidak sesuai dengan expected result.
- **Blocked** apabila pengujian tidak dapat dilakukan karena dependency atau kondisi tertentu.
- **Not Executed** apabila test case belum dijalankan.

## 6. Fokus Pengujian

Pengujian diprioritaskan pada:

- Validasi input dan business rules.
- Keseimbangan debit dan kredit jurnal.
- Validasi proses posting jurnal.
- Perhitungan dan penyajian laporan keuangan.
- Pembatasan akses berdasarkan role dan permission.
- Pencatatan aktivitas pada Audit Logs.

## 7. Hasil Pengujian

Hasil pengujian akan didokumentasikan dalam bentuk:

- Test Scenario dan Test Case.
- Test Execution Report.
- Screenshot atau evidence pengujian.
- Bug Report.
- Automation Test Result.
- Test Summary Report.