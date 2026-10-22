# Jaringan, TCP/IP, HTTP, dan API (`P1`)

## Target TKA

Menerapkan konfigurasi jaringan dasar, memahami client-server dan layer TCP/IP,
serta menganalisis kendala koneksi yang memengaruhi pengembangan/pengujian/
distribusi aplikasi.

## Required Knowledge

- [K3LH, aset, dan OS](02-k3lh-aset-os.md).
- Alamat IP, subnet sederhana, gateway, DNS, port, dan konektivitas.
- Permintaan/respons serta format data JSON.

## Inti materi

Model TCP/IP dipahami berdasarkan fungsi: akses jaringan/link, internet (IP dan
routing), transport (TCP/UDP, port, reliabilitas), dan aplikasi (HTTP, DNS,
protokol lain). Client meminta layanan; server mendengar port dan mengirim
respons. DNS menerjemahkan nama ke alamat; gateway menghubungkan jaringan.

HTTP request memiliki method, URL, header, dan body. Respons memakai status:
`2xx` berhasil, `3xx` pengalihan, `4xx` masalah permintaan/otorisasi client,
`5xx` masalah server. API database tidak boleh langsung membuka kredensial ke
client; gunakan server/API dengan validasi.

Urutan diagnosis: cek kabel/Wi-Fi → IP dan gateway → ping alamat lokal/gateway
→ DNS → port/service → log aplikasi → autentikasi dan payload. Bedakan timeout,
connection refused, DNS gagal, status 401/403, 404, dan 500.

## Contoh

Browser mendapat `404`: jaringan dan server mungkin hidup, tetapi resource/route
tidak ditemukan. `connection refused` pada localhost:3000 lebih mengarah ke
service yang belum berjalan atau port berbeda; jangan langsung menyalahkan DNS.

## Latihan

1. DNS berfungsi → **memetakan nama host ke alamat IP**.
2. TCP dipilih saat → **perlu pengiriman andal dan berurutan**.
3. HTTP 401 → **butuh autentikasi yang valid**.
4. Ping gateway gagal → **periksa koneksi lokal/IP/gateway sebelum API**.
5. API mengembalikan 500 → **analisis log server dan input; bukan otomatis kesalahan browser**.

## Checklist

- [ ] Mengurutkan diagnosis konektivitas dari lokal ke aplikasi.
- [ ] Menjelaskan IP, DNS, port, TCP, HTTP, dan API.
- [ ] Membedakan makna status 401/403/404/500.
