# BUG REPORT

## 1. Informasi Proyek

| Informasi | Keterangan |
|---|---|
| Project | Jetprint.id - Software Testing & QA |
| Object Under Test | Jetprint.id |
| Testing Method | Black Box Testing |
| Testing Approach | Functional Testing |
| Role | Execution & Defect Coordinator |
| Tester | Muhammad Gifary Nezar |

## 2. Tujuan Bug Report

Dokumen ini digunakan untuk mencatat, mengidentifikasi, dan mendokumentasikan defect yang ditemukan selama proses pengujian website Jetprint.id.

Setiap defect harus berdasarkan hasil pengujian aktual, dianalisis, dan didukung oleh evidence yang relevan.

## 3. Defect Summary

| Keterangan | Jumlah |
|---|---:|
| Total Defect Terverifikasi | 0 |
| Critical | 0 |
| High | 0 |
| Medium | 0 |
| Low | 0 |
| Open | 0 |
| Fixed | 0 |
| Retest | 0 |
| Closed | 0 |
| Reopened | 0 |

**Catatan:** Belum terdapat defect yang terverifikasi berdasarkan hasil pengujian yang telah dilakukan. Jumlah ini dapat diperbarui apabila ditemukan defect pada pengujian berikutnya.

## 4. Hasil Analisis Pengujian

### TC09 – Validasi Jumlah Pesanan Kosong

| Informasi | Keterangan |
|---|---|
| Test Case ID | TC09 |
| Fitur | Pemesanan / Jumlah Pesanan |
| Status Pengujian | BLOCKED |
| Hasil Pengamatan | Kolom jumlah pesanan tidak dapat dikosongkan atau diubah menjadi 0 melalui antarmuka website. |
| Analisis | Skenario pengujian tidak dapat dilanjutkan sesuai langkah yang ditentukan. |
| Status Defect | Belum ditetapkan sebagai defect terverifikasi. |

**Kesimpulan:**

TC09 belum dapat diselesaikan sesuai skenario pengujian karena nilai jumlah pesanan tetap berada pada angka 1. Kondisi ini perlu dikonfirmasi lebih lanjut sebelum dinyatakan sebagai defect.

## 5. Format Dokumentasi Defect

Apabila ditemukan defect yang telah diverifikasi, gunakan format berikut:

### BUG-XXX

| Informasi | Keterangan |
|---|---|
| Bug ID | BUG-XXX |
| Bug Title | Diisi sesuai masalah yang ditemukan |
| Related Test Case | ID test case terkait |
| Module / Feature | Fitur yang mengalami masalah |
| Environment | Browser dan sistem operasi |
| Severity | Critical / High / Medium / Low |
| Priority | Diisi berdasarkan urgensi perbaikan |
| Status | Open |

#### Precondition
Kondisi awal sebelum pengujian dilakukan.

#### Steps to Reproduce
1. Langkah pertama.
2. Langkah kedua.
3. Langkah ketiga.

#### Expected Result
Hasil yang seharusnya terjadi.

#### Actual Result
Hasil aktual yang ditemukan.

#### Evidence
Screenshot pendukung yang menunjukkan defect.

#### Recommendation
Saran perbaikan berdasarkan hasil analisis.

---

## 6. Defect Status

| Status | Description |
|---|---|
| Open | Defect telah dilaporkan dan belum diperbaiki. |
| Fixed | Developer menyatakan defect telah diperbaiki. |
| Retest | Defect sedang diuji ulang. |
| Closed | Defect telah diverifikasi dan dinyatakan selesai. |
| Reopened | Defect masih terjadi setelah perbaikan. |

## 7. Severity Classification

| Severity | Description |
|---|---|
| Critical | Masalah sangat serius yang menghambat fungsi utama website. |
| High | Masalah besar yang mengganggu fungsi penting. |
| Medium | Masalah yang mengganggu sebagian fungsi. |
| Low | Masalah kecil dengan dampak terbatas. |

## 8. Evidence Documentation

Screenshot defect yang ditemukan akan disimpan pada folder:

`06-bug-reports/screenshots/`

Contoh penamaan file:
- BUG-001-before.png
- BUG-001-actual.png
- BUG-001-after.png

Setiap screenshot harus memiliki keterkaitan dengan Bug ID yang dicatat.

## 9. Kesimpulan

Berdasarkan pengujian yang telah dilakukan, belum terdapat defect yang dapat ditetapkan sebagai bug terverifikasi.

TC09 masih berstatus BLOCKED karena skenario pengujian tidak dapat dilakukan sesuai test case. Kondisi tersebut akan dianalisis lebih lanjut sebelum ditetapkan sebagai defect.

Dokumen bug report akan diperbarui apabila ditemukan masalah baru atau terdapat hasil retesting dari tim pengembang.
