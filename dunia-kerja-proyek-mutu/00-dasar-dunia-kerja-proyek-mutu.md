# Dasar Dunia Kerja, Proyek, dan Mutu PPLG (`P1`)

## Tujuan belajar

Memahami cara kerja tim PPLG, hubungan kebutuhan pengguna dengan tahapan
proyek, serta alasan mutu, HAKI, dan validasi usaha perlu diperhatikan.

## Prasyarat

- [Peta prasyarat PPLG](../00-peta-prasyarat.md)
- Pemahaman dasar tentang kebutuhan pengguna, fitur, bug, dan kualitas.

## Materi

Pengembangan perangkat lunak dan gim adalah kerja tim untuk menghasilkan
solusi yang berguna bagi pengguna. Pekerjaan mencakup memahami masalah,
merancang solusi, membangun dan menguji produk, lalu merilis serta
memeliharanya. Setiap tahap perlu melibatkan komunikasi dan keputusan yang
dapat dipahami oleh anggota tim.

### Peran dan hasil kerja

Anggota tim memiliki tanggung jawab yang berbeda. Analyst membantu memahami
kebutuhan; UI/UX designer merancang alur dan pengalaman pengguna; developer
membangun solusi; QA/tester memeriksa hasil melalui pengujian; peran lain
mendukung pengelolaan produk, proyek, data, operasi, dokumentasi, atau desain
gim.

Peran dapat berkolaborasi dan dalam tim kecil dapat dirangkap, tetapi
tanggung jawab dan hasil kerja tetap perlu jelas. Contoh hasil kerja
(deliverable) adalah dokumen kebutuhan, rancangan, kode, test case, dan catatan
rilis.

### Kebutuhan dan alur proyek

Proses proyek umumnya bergerak melalui:

**Identifikasi masalah → analisis kebutuhan → desain → implementasi →
pengujian → rilis/deployment → pemeliharaan/evaluasi.**

Alur ini membantu tim mengelola pekerjaan, tetapi dapat berulang. Hasil
pengujian atau umpan balik dapat menunjukkan bahwa kebutuhan maupun desain
perlu ditinjau kembali.

Bedakan istilah berikut:

- **Kebutuhan** menjelaskan masalah atau hasil yang diperlukan pengguna.
- **Fitur** adalah kemampuan produk untuk membantu memenuhi kebutuhan.
- **Bug** adalah perilaku yang tidak sesuai dengan yang diharapkan.
- **Kualitas** menunjukkan seberapa baik produk memenuhi kebutuhan dan
  kriteria yang ditetapkan.

Memahami masalah terlebih dahulu membantu tim memilih solusi yang tepat,
menetapkan ruang lingkup, dan menyepakati kriteria penerimaan.

### Mutu, HAKI, dan peluang usaha

Mutu dijaga oleh seluruh tim melalui kriteria selesai yang jelas, perubahan
yang tercatat, code review, pengujian yang dapat diulang, dokumentasi yang
cukup, dan pelaporan masalah berdasarkan bukti. Jika masalah ditemukan,
reproduksi dan prioritaskan, perbaiki, lalu uji kembali termasuk dengan uji
regresi.

Produk dapat menggunakan kode, library, gambar, audio, font, atau aset milik
pihak lain. Tim perlu memeriksa dan mematuhi hak cipta, lisensi, merek, serta
izin penggunaan sebelum menggunakan atau mendistribusikannya.

Peluang technopreneurship sebaiknya dimulai dari masalah pengguna. Tim
merumuskan manfaat dan target pasar, mempertimbangkan pendapatan, biaya, dan
risiko, lalu menguji asumsi inti melalui MVP (minimum viable product). MVP
bertujuan untuk belajar dan memvalidasi nilai, bukan sekadar membuat produk
dengan fitur sesedikit mungkin.

## Contoh

Pengguna kesulitan menyelesaikan checkout. Tim mengumpulkan bukti dan
merumuskan kebutuhan; designer menyusun alur; developer membuat perubahan;
QA menguji skenario berhasil dan gagal. Tim mencatat perubahan, memastikan
aset yang digunakan berizin, merilis solusi, dan memantau hasilnya. Jika
masalah tetap ada, kebutuhan atau desain ditinjau kembali.

## Latihan

1. Urutkan alur proyek dari memahami masalah hingga pemeliharaan. →
   **Identifikasi masalah, analisis kebutuhan, desain, implementasi,
   pengujian, rilis, pemeliharaan/evaluasi.**
2. Apa perbedaan kebutuhan dengan fitur? → **Kebutuhan menyatakan hasil yang
   diperlukan; fitur adalah kemampuan produk yang membantu memenuhinya.**
3. Siapa yang bertanggung jawab atas mutu? → **Seluruh tim, bukan hanya
   QA/tester.**
4. Apa yang perlu dilakukan sebelum mendistribusikan library pihak lain? →
   **Memeriksa dan mematuhi lisensinya.**
5. Apa tujuan MVP? → **Menguji asumsi tentang masalah atau nilai inti dengan
   cara minimum yang sesuai.**

## Checklist

- [ ] Menjelaskan hubungan peran dan hasil kerja dalam tim PPLG.
- [ ] Mengurutkan tahapan umum proyek dan memahami bahwa proses dapat berulang.
- [ ] Membedakan kebutuhan, fitur, bug, dan kualitas.
- [ ] Menyebutkan praktik dasar budaya mutu.
- [ ] Menjelaskan mengapa lisensi dan izin penggunaan harus diperiksa.
- [ ] Menjelaskan hubungan masalah pengguna, proposisi nilai, dan MVP.

Lanjutkan ke [Profesi dan tugas dalam PPLG](01-profesi-pplg.md).
