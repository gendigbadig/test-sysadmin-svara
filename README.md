# Soal Tes Administrasi Server SVARA

## SSH
- Hostname: **nomorurut**-test.awscloud.svara.fm
- Username: ubuntu
- Login tanpa password, menggunakan PEM key yang sudah disediakan

## OS: 
Ubuntu 18.04

---

## Tugas: 
**Goal**: Berhasil melakukan deployment aplikasi web berbasis php dan mysql sederhana yang bisa diakses melalui alamat _**nomorurut**-test.awscloud.svara.fm_

**Batas Pengerjaan**: 90 menit

**Langkah**: 
1. Install web server (pilihan: apache webserver/nginx) 
2. Install php 7. Jika pilihan 1 memilih untuk menggunakan nginx, maka perlu juga menginstall php-fpm
3. Install database MariaDB 
4. Buat user di MariaDB dengan ketentuan berikut:
   - username: `svara`
   - password: `testadminserversvara`
5. Buat database `svaraapp` dan beri akses ke user `svara` supaya bisa baca/tulis ke database tersebut
6. Simpan direktori `app` di folder ini kedalam root directory web server yang dipilih (bisa menggunakan `scp` atau menggunakan cara lain)
7. Didalam direktori `app` terdapat file `config.php`. Konfigurasi parameter username dan password sesuai dengan user yang dibuat di MariaDB sebelumnya
8. Lakukan instalasi/inisiasi database aplikasi dengan cara akses ke alamat _http://**nomorurut**-test.awscloud.svara.fm/install.php_. Pastikan di langkah ini tidak ada pesan error seperti `General error: ` dan sebagainya. Jika muncul error, pastikan kembali langkah-langkah sebelumnya sudah dilakukan dengan benar.
9. Jika sudah selesai, akses alamat _http://**nomorurut**-test.awscloud.svara.fm/public_ dan coba membuat user baru sesuai dengan data diri. 
10. Melapor bahwa sudah selesai mengerjakan 

**Tugas Tambahan**: 
1. Implementasikan HTTPS di web server pilihan anda menggunakan Let's Encrypt SSL dengan cara yang sesuai dengan web server yang dipilih, supaya alamat url menjadi _https://**nomorurut**-test.awscloud.svara.fm_

**Catatan**: 
- Jika memilih nginx, mampu mengimplementasikan https menggunakan let's encrypt, dan mampu mengerjakan dengan cepat sesuai target waktu akan mendapat nilai plus, tapi goalnya adalah keberhasilan
- Diperkenankan untuk mencari referensi di google, diperkenankan pula untuk memberitahu keyword yang digunakan untuk mencari referensi di google, namun **tidak diperkenankan** untuk melihat pekerjaan ataupun membantu pekerjaan orang lain. 

---

## Soal: 

**Batas Pengerjaan**: 15 menit

**Langkah**:
1. Buat direktori /home/ubuntu/soal
2. Masuk ke direktori tersebut, lalu buat shell script dengan nama **nomorurut**.sh
3. Isi shell script dengan fungsi yang menghasilkan output yang diharapkan:
   - Terbentuk 10 file txt yang diberi nama: **nomorurut** * 10 + {0-9}
     
     Contoh: Nomor Urut 1, maka terbentuk file: 10.txt, 11.txt, 12.txt, 13.txt, 14.txt, 15.txt, 16.txt, 17.txt, 18.txt, 19.txt

   - Terbentuk 10 direktori yang diberi nama **nomorurut** * 100 + {0-9}
  
     Contoh: Nomor Urut 1, maka terbentuk direktori: 100, 101, 102, 103, 104, 105, 106, 107, 108, 109

4. Pada shell script harus mengandung unsur looping
5. Untuk ujicoba, silahkan eksekusi shell script. Namun sebelum melapor selesai mengerjakan, hapus semua hasil output terlebih dahulu.

**Catatan**: 
- Jika mengerjakan dengan cepat sesuai target waktu akan mendapat nilai plus, tapi goalnya adalah keberhasilan
- Diperkenankan untuk mencari referensi di google, diperkenankan pula untuk memberitahu orang lain keyword yang digunakan untuk mencari referensi di google, namun **tidak diperkenankan** untuk melihat pekerjaan ataupun membantu pekerjaan orang lain. 
