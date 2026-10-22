# Client-Server dan DNS (`P1`)

## Tujuan belajar

Menjelaskan pertukaran permintaan dan respons antara client dengan server serta
peran DNS dalam menemukan server.

## Prasyarat

- [Dasar jaringan dan model TCP/IP](00-dasar-jaringan-dan-tcp-ip.md)

## Materi

**Client** adalah pihak yang meminta layanan, misalnya browser atau aplikasi.
**Server** menyediakan layanan: server menunggu komunikasi pada port tertentu,
memproses permintaan, lalu mengirim respons.

Alur sederhananya:

1. Client menentukan layanan yang ingin digunakan.
2. DNS menerjemahkan nama host menjadi alamat IP jika client menggunakan nama.
3. Client menghubungi alamat dan port layanan melalui jaringan.
4. Server memproses permintaan dan mengirim respons.

Nama host memudahkan pengguna mengingat tujuan, sedangkan jaringan menggunakan
alamat IP untuk mengarahkan komunikasi. Port membantu mengarahkan komunikasi
ke layanan yang sesuai pada perangkat tujuan.

## Contoh

Ketika browser meminta sebuah halaman, browser bertindak sebagai client dan
server web menyediakan halaman tersebut. Jika nama host tidak dapat
diterjemahkan, browser tidak dapat menemukan alamat tujuan berdasarkan nama
itu.

## Latihan

1. Siapa yang memulai permintaan layanan? → **Client.**
2. Apa tugas server dalam alur dasar? → **Mendengarkan port, memproses
   permintaan, lalu mengirim respons.**
3. Apa yang dilakukan DNS? → **Menerjemahkan nama host ke alamat IP.**

## Checklist

- [ ] Membedakan peran client dan server.
- [ ] Menjelaskan hubungan nama host, DNS, alamat IP, dan port.
- [ ] Mengurutkan alur permintaan hingga respons.

Lanjutkan ke [HTTP dan API](02-http-dan-api.md).
