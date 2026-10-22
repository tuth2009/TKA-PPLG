# Latihan Integratif PPLG (`P1`)

## Tujuan belajar

Menggabungkan penalaran proyek, tracing kode, desain modular/OOP, K3LH,
pengelolaan aset, dan diagnosis jaringan/API dalam satu skenario.

## Prasyarat

- Menyelesaikan [Tracing data dan struktur kontrol](01-tracing-data-dan-kontrol.md)
- Menyelesaikan [Skenario dunia kerja, proyek, dan mutu](02-skenario-dunia-kerja-dan-mutu.md)
- Menyelesaikan [Skenario K3LH, aset, dan OS](03-skenario-k3lh-aset-dan-os.md)
- Menyelesaikan [Skenario jaringan, HTTP, dan API](04-skenario-jaringan-http-dan-api.md)
- Menyelesaikan [Skenario fungsi dan modularisasi](05-skenario-fungsi-dan-modularisasi.md)
- Menyelesaikan [Skenario OOP](06-skenario-oop.md)

## Studi kasus: checkout aplikasi toko

Tim merilis checkout baru. Sebagian pengguna melaporkan tombol bayar tidak
berhasil. Di log terlihat bahwa beberapa permintaan mendapat `403`, sementara
pengguna lain membuka URL lama dan menerima `404`. Fungsi `processOrder`
menghitung pajak, menyimpan pesanan, dan mengirim notifikasi. Class
`Payment` memiliki atribut `amount` yang public; ada subclass `QRPayment`.
Log yang dibagikan ke kanal tim menampilkan email pengguna. Saat pemeriksaan
di ruang kerja, ditemukan kabel melintang di jalur berjalan.

## Tugas

1. Urutkan langkah awal diagnosis laporan, bedakan `403` dan `404`, dan
   jelaskan bukti apa yang perlu dikumpulkan.
2. Uraikan tanggung jawab tim dari analisis kebutuhan sampai rilis perbaikan
   dan uji regresi.
3. Usulkan cara memecah `processOrder` agar hasil perhitungan dapat diuji dan
   efek samping terlihat.
4. Jelaskan perubahan desain untuk melindungi `amount`, dan tentukan kapan
   `QRPayment` memakai inheritance serta implementasi `pay` yang dijalankan.
5. Sebutkan tindakan untuk melindungi email dalam log, mengelola kredensial,
   dan mengamankan kabel.
6. Tulis kriteria penerimaan sederhana yang dapat diuji untuk checkout.

## Kunci jawaban ringkas

1. Periksa kondisi reproduksi, URL, autentikasi/role, dan bukti permintaan.
   `403` mengarah ke izin/role; `404` mengarah ke URL, route, atau resource
   yang tidak ditemukan. Keduanya bukan bukti otomatis bahwa jaringan putus.
   Jika konektivitas dasar bermasalah, diagnosis tetap dimulai dari lokal,
   IP/gateway, DNS, service/port, lalu aplikasi.
2. Analyst memperjelas kebutuhan dan kriteria; developer mengimplementasikan
   perubahan; QA menguji kasus gagal dan berhasil; tim meninjau, mencatat,
   merilis, lalu memantau. Bug harus direproduksi, diprioritaskan, diperbaiki,
   dan diuji regresi tanpa menyalahkan individu.
3. Pisahkan validasi, perhitungan total/pajak yang mengembalikan nilai,
   penyimpanan pesanan, dan pengiriman notifikasi. Uji fungsi hitung dengan
   kasus normal dan batas; uji tindakan melalui hasil atau kolaborator yang
   sesuai.
4. Jadikan `amount` tidak terbuka sembarangan dan validasi nilainya pada
   method yang mengubahnya. `QRPayment` dapat mewarisi `Payment` jika benar
   merupakan jenis pembayaran; pemanggilan `pay` memakai override
   `QRPayment` saat object aktual adalah `QRPayment`.
5. Samarkan atau hapus email sebelum log dibagikan, batasi akses, dan jangan
   menyimpan token di repository. Amankan jalur kabel sesuai prosedur dan
   laporkan bahaya; tangani perangkat listrik hanya sesuai kewenangan.
6. Contoh: "Jika pengguna dengan role yang berwenang memilih metode QR dan
   mengonfirmasi pembayaran valid, sistem menyimpan satu pesanan dengan total
   yang benar dan menampilkan status hasil pembayaran; permintaan tanpa izin
   ditolak tanpa membocorkan data." Kriteria perlu disesuaikan dengan
   kebutuhan produk dan dapat direproduksi oleh QA.

## Checklist akhir

- [ ] Menelusuri bukti dan memilih diagnosis sebelum mengubah kode.
- [ ] Menghubungkan kebutuhan, peran tim, pengujian, rilis, dan mutu.
- [ ] Menjelaskan batas tanggung jawab fungsi serta efek samping.
- [ ] Menjaga state object dan memilih inheritance/komposisi secara tepat.
- [ ] Menangani privasi, kredensial, dan bahaya kerja dengan aman.
- [ ] Menulis kriteria penerimaan yang dapat diuji.
