# Proses Bisnis dan Tahapan Proyek (`P1`)

## Target belajar

Menjelaskan alur umum pengembangan perangkat lunak/gim dan memahami bahwa
proses proyek dapat berulang mengikuti umpan balik.

## Materi

Proses bisnis menjelaskan cara pekerjaan dilakukan untuk menghasilkan nilai
bagi pengguna atau organisasi. Dalam pengembangan perangkat lunak dan gim,
alur umum proyek adalah:

1. **Identifikasi masalah** — memahami masalah atau kebutuhan yang ingin
   diselesaikan.
2. **Analisis kebutuhan** — mengumpulkan dan memperjelas kebutuhan pengguna.
3. **Desain** — merancang solusi, alur, tampilan, atau struktur sistem.
4. **Implementasi** — membangun solusi berdasarkan desain.
5. **Pengujian** — memeriksa apakah hasil bekerja sesuai kebutuhan dan
   menemukan masalah.
6. **Rilis/deployment** — menyediakan hasil kepada pengguna.
7. **Pemeliharaan/evaluasi** — memantau hasil, menangani masalah, dan menilai
   kebutuhan perubahan berikutnya.

Urutan ini membantu tim mengelola pekerjaan, tetapi bukan berarti setiap tahap
hanya terjadi satu kali. Pada proses iteratif, hasil pengujian atau umpan balik
pengguna dapat membawa tim kembali ke analisis atau desain.

Kebutuhan pengguna, fitur, bug, dan kualitas adalah hal yang berbeda:

- **Kebutuhan pengguna** menyatakan masalah atau hasil yang diperlukan.
- **Fitur** adalah kemampuan produk yang dibuat untuk memenuhi kebutuhan.
- **Bug** adalah perilaku atau hasil yang tidak sesuai dengan yang diharapkan.
- **Kualitas** menggambarkan seberapa baik produk memenuhi kriteria yang
  ditetapkan.

Memahami masalah sebelum memilih solusi mencegah tim menambahkan fitur yang
tidak menjawab kebutuhan sebenarnya.

### Proses bisnis, tujuan, dan ruang lingkup

Proses bisnis menggambarkan kegiatan nyata yang dilakukan orang atau
organisasi untuk mencapai tujuan. Sebelum membuat aplikasi, tim perlu
memahami pelaku, urutan aktivitas, keputusan, informasi yang digunakan, dan
masalah pada proses tersebut. Aplikasi adalah salah satu cara mendukung atau
memperbaiki proses, bukan tujuan yang harus dibuat tanpa alasan.

Proyek menerjemahkan kebutuhan menjadi pekerjaan yang dapat dikelola. Tim
menetapkan tujuan, ruang lingkup, prioritas, pemilik tugas, sumber daya,
ketergantungan, serta risiko. Ruang lingkup membantu menghindari pekerjaan
yang terus bertambah tanpa kesepakatan (scope creep). Perubahan kebutuhan
masih dapat diterima, tetapi dampak terhadap waktu, biaya, kualitas, dan
pekerjaan lain perlu dibahas.

Kebutuhan fungsional menjelaskan kemampuan atau perilaku yang harus disediakan,
misalnya sistem menghitung total belanja. Kebutuhan nonfungsional menjelaskan
kualitas atau batasan, misalnya mudah digunakan, dapat diakses, aman, atau
memenuhi sasaran kinerja yang disepakati. Kriteria penerimaan membuat kebutuhan
lebih dapat diperiksa: kondisi awal, tindakan pengguna, dan hasil yang
diharapkan ditulis dengan cukup jelas.

### Tahapan proyek secara lebih terperinci

1. **Identifikasi masalah:** kumpulkan gejala, pengguna terdampak, konteks,
   frekuensi, dan dampak. Jangan langsung menganggap solusi yang pertama
   terpikir sebagai kebutuhan.
2. **Analisis kebutuhan:** wawancarai pemangku kepentingan, amati proses,
   klarifikasi aturan, dan catat kebutuhan serta hal yang belum diketahui.
3. **Perencanaan:** tentukan ruang lingkup awal, prioritas, tanggung jawab,
   jadwal, sumber daya, risiko, dan cara mengukur kemajuan.
4. **Desain:** rancang alur pengguna, tampilan, struktur sistem, dan data.
   Prototipe dapat dipakai untuk mendapat umpan balik sebelum implementasi.
5. **Implementasi:** bangun perubahan, tinjau kode, dan catat keputusan
   penting agar pekerjaan dapat dipahami serta dilanjutkan orang lain.
6. **Pengujian:** uji terhadap kebutuhan dan kriteria penerimaan. Catat
   perbedaan antara hasil yang diharapkan dan hasil aktual.
7. **Rilis/deployment:** siapkan versi, lingkungan, komunikasi perubahan, dan
   cara memantau atau mengembalikan rilis bila terjadi masalah.
8. **Pemeliharaan/evaluasi:** tangani masalah, perbarui dependensi bila perlu,
   pantau hasil, dan gunakan umpan balik untuk menentukan perubahan selanjutnya.

Dalam pendekatan berurutan, tahapan direncanakan lebih dahulu dan banyak
pekerjaan diselesaikan sesuai urutan; pendekatan ini dapat berguna ketika
kebutuhan stabil atau proses formal dibutuhkan. Dalam pendekatan
iteratif/inkremental, tim membangun dan mengevaluasi bagian produk secara
bertahap; cara ini memberi ruang untuk belajar dari umpan balik. Keduanya
memerlukan perencanaan dan pengujian, dan tidak ada satu pendekatan yang
selalu cocok untuk semua proyek.

### Istilah yang sering tertukar

- **Kebutuhan:** masalah, tujuan, atau hasil yang diperlukan pengguna.
- **Fitur:** kemampuan produk yang dibuat untuk memenuhi suatu kebutuhan.
- **Bug:** perilaku aktual berbeda dari perilaku yang diharapkan atau
  disepakati.
- **Kualitas:** seberapa baik produk memenuhi kebutuhan dan kriteria, termasuk
  aspek seperti ketepatan, keandalan, keamanan, dan kemudahan penggunaan.
- **Umpan balik:** informasi dari pengguna atau tim yang dapat mengonfirmasi
  hasil atau menunjukkan perlunya perubahan.

Fitur baru bukan otomatis perbaikan bug. Contohnya, permintaan menambahkan
metode pembayaran baru adalah perubahan kemampuan; tombol bayar yang tidak
bekerja sesuai kriteria adalah bug.

## Contoh

Pengguna tidak berhasil menyelesaikan checkout. Tim mengumpulkan informasi
tentang kendala tersebut, merumuskan kebutuhan, merancang alur, membuat
perubahan, menguji kasus checkout, lalu merilis dan memantau hasilnya. Jika
umpan balik menunjukkan alur masih membingungkan, tim dapat kembali memperbaiki
desain.

## Latihan

1. Susun tahapan setelah desain: implementasi → pengujian → rilis → pemeliharaan.
2. Apa yang dapat dilakukan tim jika umpan balik menunjukkan solusi belum
   memenuhi kebutuhan? **Kembali meninjau kebutuhan atau desain dan
   memperbaikinya.**
3. Mengapa sebaiknya tim memahami kendala checkout sebelum menambah fitur?
   **Agar solusi yang dibuat benar-benar menjawab masalah pengguna.**
4. Apa beda kebutuhan fungsional dan nonfungsional? **Fungsional menjelaskan
   kemampuan/perilaku; nonfungsional menjelaskan kualitas atau batasan sistem.**
5. Apa yang perlu dilakukan jika ruang lingkup berubah? **Bahas kebutuhan dan
   prioritas, lalu nilai serta sepakati dampak perubahan pada sumber daya,
   jadwal, kualitas, dan pekerjaan lain.**
6. Apakah pendekatan iteratif berarti tidak perlu perencanaan? **Tidak; tim
   tetap merencanakan tujuan dan pekerjaan, lalu memperbarui rencana saat
   memperoleh informasi baru.**

## Checklist

- [ ] Dapat menyusun tahapan umum proyek.
- [ ] Dapat membedakan kebutuhan, fitur, bug, dan kualitas.
- [ ] Memahami bahwa umpan balik dapat mengulang atau mengubah tahapan proyek.
- [ ] Dapat menjelaskan ruang lingkup, kriteria penerimaan, dan kebutuhan nonfungsional.
- [ ] Dapat membandingkan pendekatan berurutan dan iteratif.
