
# Hasil Eksekusi Pengujian

## TC01 – Login dengan Email dan Password Benar

| Komponen | Hasil |
|---|---|
| Test Case ID | TC01 |
| Fitur yang Diuji | Login |
| Tujuan Pengujian | Memastikan pengguna dapat masuk menggunakan kredensial yang valid. |
| Test Data | Akun pelanggan yang sudah terdaftar. |
| Expected Result | Pengguna berhasil login dan diarahkan ke halaman setelah login. |
| Actual Result | Sistem menerima email dan password yang valid. Pengguna berhasil masuk dan diarahkan ke halaman profil pelanggan. Nama dan email akun ditampilkan pada halaman tersebut. |
| Status | **PASS** |

### Bukti Pengujian

| No. | Nama Screenshot | Keterangan |
|---|---|---|
| 1 | [TC01-01-before-login](screenshots/TC01-01-before-login.png) | Tampilan awal website sebelum login. |
| 2 | [TC01-02-login-form](screenshots/TC01-02-login-form.png) | Form login sebelum diisi. |
| 3 | [TC01-03-password-validation](screenshots/TC01-03-password-validation.png) | Validasi password kurang dari 8 karakter. |
| 4 | [TC01-04-credentials-filled](screenshots/TC01-04-credentials-filled.png) | Form login setelah data dimasukkan. |
| 5 | [TC01-05-login-success](screenshots/TC01-05-login-success.png) | Tampilan profil setelah berhasil login. |

### Kesimpulan Pengujian

Berdasarkan hasil pengujian, fitur login Jetprint.id berhasil menerima kredensial akun pelanggan yang valid. Sistem mengarahkan pengguna ke halaman profil setelah proses login berhasil. Dengan demikian, hasil pengujian TC01 dinyatakan **PASS**.
