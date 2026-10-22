# Diagnosis Konektivitas (`P1`)

## Tujuan belajar

Menelusuri kendala koneksi secara berurutan dari jaringan lokal hingga aplikasi,
dan membedakan gejala yang menunjuk ke lapisan masalah berbeda.

## Prasyarat

- [Dasar jaringan dan model TCP/IP](00-dasar-jaringan-dan-tcp-ip.md)
- [Client-server dan DNS](01-client-server-dan-dns.md)
- [HTTP dan API](02-http-dan-api.md)

## Urutan diagnosis

Periksa dari komponen paling dekat dengan perangkat menuju aplikasi:

1. Periksa kabel atau koneksi Wi-Fi.
2. Periksa alamat IP dan gateway.
3. Uji konektivitas ke alamat lokal atau gateway.
4. Periksa resolusi DNS.
5. Periksa port dan apakah service berjalan.
6. Periksa log aplikasi.
7. Periksa autentikasi dan payload permintaan.

Urutan ini membantu menghindari kesimpulan terlalu dini. Misalnya, jika koneksi
ke gateway gagal, pemeriksaan API belum menjadi langkah pertama yang tepat.

## Membedakan gejala

| Gejala | Arah pemeriksaan awal |
|---|---|
| Timeout | Konektivitas atau layanan yang tidak merespons |
| Connection refused | Service belum berjalan atau port tidak sesuai |
| DNS gagal | Resolusi nama host |
| HTTP `401` atau `403` | Autentikasi atau izin akses |
| HTTP `404` | Route atau resource |
| HTTP `500` | Log server dan input yang diproses |

## Contoh

`connection refused` pada `localhost:3000` lebih mengarah ke service yang belum
berjalan atau aplikasi menggunakan port berbeda. Jangan langsung menyalahkan
DNS karena koneksi menggunakan `localhost`.

Jika ping ke gateway gagal, periksa koneksi lokal, alamat IP, dan gateway
sebelum menelusuri API.

## Latihan

1. Ping gateway gagal. Apa yang diperiksa lebih dahulu? → **Koneksi lokal,
   alamat IP, dan gateway.**
2. Aplikasi mendapat `connection refused` pada port lokal. Apa dugaan awal? →
   **Service belum berjalan atau port yang digunakan berbeda.**
3. API mengembalikan `500`. Ke mana pemeriksaan diarahkan? → **Log server dan
   input; bukan otomatis kesalahan browser.**

## Checklist

- [ ] Mengurutkan diagnosis dari koneksi lokal ke aplikasi.
- [ ] Membedakan timeout, connection refused, dan DNS gagal.
- [ ] Mengarahkan pemeriksaan `401`/`403`, `404`, dan `500` ke penyebab yang
  sesuai.
