# Dasar Jaringan dan Model TCP/IP (`P1`)

## Tujuan belajar

Memahami peran alamat jaringan dan fungsi setiap lapisan TCP/IP dalam
komunikasi antarkomputer.

## Prasyarat

- [Sistem operasi, berkas, dan direktori](../k3lh-aset-os/04-sistem-operasi-file.md)
- Pemahaman dasar tentang perangkat yang terhubung ke jaringan.

## Materi

Jaringan menghubungkan perangkat agar dapat bertukar data dan menggunakan
layanan. Beberapa istilah dasar yang perlu dikenali:

- **Alamat IP** mengidentifikasi perangkat pada jaringan.
- **Subnet** membagi alamat ke dalam kelompok jaringan. Pada tingkat dasar,
  subnet membantu menentukan apakah tujuan berada di jaringan lokal.
- **Gateway** menjadi jalur keluar dari jaringan lokal menuju jaringan lain.
- **DNS** menerjemahkan nama host menjadi alamat IP.
- **Port** mengarahkan komunikasi ke layanan tertentu pada sebuah perangkat.

Model TCP/IP menjelaskan komunikasi melalui lapisan berdasarkan fungsinya:

| Lapisan | Fungsi |
|---|---|
| Akses jaringan/link | Mengirim data melalui media dan jaringan lokal |
| Internet | Pengalamatan IP dan routing ant jaringan |
| Transport | Komunikasi ant proses menggunakan TCP atau UDP dan port |
| Aplikasi | Protokol layanan seperti HTTP dan DNS |

TCP dan UDP memiliki kegunaan berbeda. **TCP** menyediakan pengiriman yang
andal dan berurutan. **UDP** tidak menjamin pengiriman dan urutan dengan cara
yang sama, sehingga dapat dipilih ketika karakteristik tersebut sesuai dengan
kebutuhan aplikasi.

## Contoh

Saat membuka situs dengan nama domain, perangkat meminta DNS mencari alamat IP
tujuan. Data kemudian dikirim melalui jaringan menuju server; gateway membantu
jika server berada di luar jaringan lokal.

## Latihan

1. Apa fungsi DNS? → **Memetakan nama host ke alamat IP.**
2. Apa peran gateway? → **Menghubungkan jaringan lokal ke jaringan lain.**
3. Kapan TCP tepat dipilih? → **Saat pengiriman yang andal dan berurutan
   diperlukan.**

## Checklist

- [ ] Menjelaskan fungsi IP, subnet, gateway, DNS, dan port.
- [ ] Menyebutkan fungsi empat lapisan TCP/IP.
- [ ] Membedakan kebutuhan umum TCP dan UDP.

Lanjutkan ke [Client-server dan DNS](01-client-server-dan-dns.md).
