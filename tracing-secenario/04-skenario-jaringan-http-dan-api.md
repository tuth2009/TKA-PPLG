# Skenario Jaringan, HTTP, dan API (`P1`)

## Tujuan belajar

Memilih langkah diagnosis jaringan dari gejala, membedakan status HTTP, serta
memahami batas akses client ke data server.

## Prasyarat

- [Dasar jaringan dan model TCP/IP](../jaringan-tcpip/00-dasar-jaringan-dan-tcp-ip.md)
- [Client-server dan DNS](../jaringan-tcpip/01-client-server-dan-dns.md)
- [HTTP dan API](../jaringan-tcpip/02-http-dan-api.md)
- [Diagnosis konektivitas](../jaringan-tcpip/03-diagnosis-konektivitas.md)

## Skenario: aplikasi tidak dapat memuat data

Browser gagal memuat halaman API. Mulai dari koneksi lokal dan IP/gateway,
lanjutkan ke DNS, port/service, lalu log aplikasi, autentikasi, dan payload.
Jika gateway tidak dapat dijangkau, jangan mulai dengan mengubah kode API.
Jika API memberi status HTTP, gunakan status itu sebagai bukti untuk
menentukan lapisan pemeriksaan berikutnya.

## Latihan

1. Ping gateway gagal. Apa yang diperiksa lebih dahulu? →
   **Koneksi Wi-Fi/kabel, alamat IP, dan gateway.**
2. `localhost:3000` memberi `connection refused`. Apa dugaan awal? →
   **Service belum berjalan atau port yang dituju berbeda.**
3. DNS tidak dapat menerjemahkan nama host. Apa bagian yang perlu diperiksa? →
   **Resolusi nama DNS dan konfigurasi nama host, bukan langsung route API.**
4. API mengembalikan `403` untuk `/admin/users`. Apa arah pemeriksaan yang
   tepat? → **Autentikasi/role dan kebijakan izin; jangan mematikan
   autentikasi.**
5. Server memberi `404` setelah deployment. Apakah itu membuktikan koneksi
   jaringan putus? → **Tidak; periksa URL, route, base path, dan log server.**
6. API memberi `500`. Di mana mencari bukti awal? → **Log server dan input
   yang diproses; bukan otomatis kesalahan browser.**
7. Di mana kredensial database seharusnya berada? → **Di sisi server/API
   dengan validasi dan pengendalian akses, bukan dibuka di client.**
8. Bagian transport perlu pengiriman andal dan berurutan. Protokol mana yang
   umumnya dipilih? → **TCP; pemilihan tetap mengikuti kebutuhan aplikasi.**
9. Apa fungsi lapisan internet pada model TCP/IP? → **Pengalamatan IP dan
   routing ant jaringan.**

## Checklist

- [ ] Mengurutkan diagnosis dari koneksi lokal ke aplikasi.
- [ ] Membedakan timeout, connection refused, dan DNS gagal.
- [ ] Membedakan masalah autentikasi/izin (`401`/`403`), route/resource
  (`404`), dan server (`500`).
- [ ] Menjelaskan peran server/API dalam melindungi akses database.
- [ ] Menghubungkan fungsi lapisan internet dan transport dengan diagnosis.
