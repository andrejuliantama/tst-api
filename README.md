# tst-api
Repository untuk tugas pembuatan API

ini adalah API dari aplikasi GOJEK dengan menggunakan bantuan GOJEK unofficial API Wrapper in Python.
source GOJEK unofficial API Wrapper in Python : https://github.com/ridho9/pygojek

File pyapi.py pada repo ini akan melakukan hosting server secara lokal.
Anda perlu login terlebih dahulu dengan akun gojek anda.

Cara Menggunakan:

1. jalankan program pyapi.py di command prompt dengan cara >python pyapi.py
2. curl -X POST https://localhost:9977/login?phone=nomorHP --insecure
3. Anda akan menerima SMS OTP ke nomor tujuan
4. curl -X POST https://localhost:9977/loginOTP?otp=kodeOTP --insecure
5. Kemudian anda berhasil login
6. Method yang dapat digunakan:
   - Untuk melihat Balance anda : curl -X GET https://localhost:9977/balance --insecure
   - Untuk melihat History transaksi anda : curl -X GET https://localhost:9977/history --insecure
7. Bila sudah selesai, jalankan LOGOUT : curl -X DELETE https://localhost:9977/logout --insecure
. 
