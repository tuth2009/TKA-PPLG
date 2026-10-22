# Skenario Dunia Kerja, Proyek, dan Mutu (`P1`)

## Tujuan belajar

Menerapkan pemahaman peran tim, tahapan proyek, budaya mutu, HAKI, dan
technopreneurship dalam situasi pengembangan produk.

## Prasyarat

- [Dasar dunia kerja, proyek, dan mutu PPLG](../dunia-kerja-proyek-mutu/00-dasar-dunia-kerja-proyek-mutu.md)
- [Profesi dan tugas dalam PPLG](../dunia-kerja-proyek-mutu/01-profesi-pplg.md)
- [Proses bisnis dan tahapan proyek](../dunia-kerja-proyek-mutu/02-proses-bisnis-dan-proyek.md)
- [Budaya mutu](../dunia-kerja-proyek-mutu/03-budaya-mutu.md)
- [HAKI dan lisensi](../dunia-kerja-proyek-mutu/04-haki-dan-lisensi.md)
- [Technopreneurship](../dunia-kerja-proyek-mutu/05-technopreneurship.md)

## Skenario: checkout gagal

Pengguna melaporkan bahwa sebagian pesanan gagal dibayar. Tim langsung meminta
developer menambah metode pembayaran baru.

Sebelum mengubah produk, tim perlu mengumpulkan bukti: siapa yang terdampak,
langkah untuk mengulangi masalah, hasil yang diharapkan, dan hasil aktual.
Analyst memperjelas kebutuhan dan kriteria penerimaan; UI/UX meninjau alur;
developer menyelidiki implementasi; QA menyiapkan kasus reproduksi serta
regresi. Project manager membantu koordinasi prioritas dan risiko, sedangkan
product manager menjaga fokus pada masalah dan nilai produk. Peran dapat
dirangkap, tetapi tanggung jawab tetap harus jelas.

Urutan kerja dapat bergerak dari identifikasi masalah dan analisis kebutuhan
ke desain, implementasi, pengujian, rilis, dan pemeliharaan. Hasil pengujian
atau umpan balik dapat membawa tim kembali ke analisis atau desain.

## Latihan

1. Tim ingin menambah metode baru sebelum mengetahui penyebab kegagalan.
   Mengapa perlu menahan perubahan itu? → **Fitur baru belum tentu menjawab
   kebutuhan atau memperbaiki bug; kumpulkan bukti dan pahami masalah dahulu.**
2. Bug kritis muncul setelah rilis. Urutkan respons yang tepat. →
   **Catat dan reproduksi, nilai dampak/prioritas, perbaiki, jalankan uji
   regresi, lalu pantau hasil rilis.**
3. QA menemukan bug; siapa yang bertanggung jawab atas mutu? →
   **Seluruh tim; QA membantu memberi bukti melalui pengujian.**
4. Tim ingin memakai library pihak ketiga dalam produk komersial. Apa yang
   perlu dilakukan? → **Periksa lisensi versi yang digunakan, cocokkan
   ketentuannya dengan cara penggunaan/distribusi, dan penuhi kewajibannya.**
5. Tim punya ide aplikasi tetapi belum membuktikan masalahnya. Apa langkah
   MVP yang tepat? → **Nyatakan asumsi, tentukan bukti/ukuran keberhasilan,
   lalu uji solusi minimum dengan pengguna yang sesuai.**
6. Tim akan menguji MVP kepada pemilik toko kecil. Apa yang perlu dirumuskan
   selain fitur prototipe? → **Target pengguna dan masalahnya, proposisi
   nilai, asumsi/ukuran validasi, biaya dan risiko, serta model pendapatan
   yang masuk akal; lindungi data peserta dan gunakan aset berizin.**
7. Bagaimana membedakan tingkat dampak bug dengan kesegeraan penanganannya?
   → **Severity menggambarkan dampak; priority menentukan urutan/kesegeraan
   berdasarkan konteks, pengguna terdampak, risiko, dan rencana rilis.**

## Checklist

- [ ] Memilih peran berdasarkan tugas dan hasil kerja yang diperlukan.
- [ ] Mengurutkan tahapan proyek serta mengenali proses iteratif.
- [ ] Membedakan kebutuhan, fitur, bug, dan kualitas.
- [ ] Menangani masalah dengan bukti, prioritas, uji regresi, dan pemantauan.
- [ ] Memeriksa lisensi dan membedakan asumsi produk dari bukti pengguna.
- [ ] Mempertimbangkan target pasar, proposisi nilai, model pendapatan, biaya,
  dan risiko saat mengevaluasi peluang teknologi.
