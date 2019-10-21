# tst-api
Repository untuk tugas pembuatan API

ini adalah API dari aplikasi GOJEK dengan menggunakan bantuan GOJEK unofficial API Wrapper in Python.
source GOJEK unofficial API Wrapper in Python : https://github.com/ridho9/pygojek

File pyapi.py pada repo ini akan melakukan hosting server secara lokal.
Anda perlu login terlebih dahulu dengan akun gojek anda.

Cara Menggunakan:

1. curl -X POST https://localhost:9977/login?phone=NOMOR HP
2. Anda akan menerima SMS OTP ke nomor tujuan
3. curl -X POST https://localhost:9977/loginOTP?otp= KODE OTP
4. Kemudian anda berhasil login
5. Method yang dapat digunakan:
   - Untuk melihat Balance anda : curl -X GET https://localhost:9977/balance
   - Untuk melihat History transaksi anda : curl -X GET https://localhost:9977/history
6. Bila sudah selesai, jalankan LOGOUT : curl -X DELETE https://localhost:9977/logout

