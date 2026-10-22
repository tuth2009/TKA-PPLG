# Budaya Mutu dalam Proyek PPLG (`P1`)

## Target belajar

Menjelaskan praktik kerja yang membantu tim menjaga kualitas hasil dan
menangani masalah secara terukur.

## Materi

Budaya mutu adalah kebiasaan tim untuk menetapkan kualitas yang diharapkan,
memeriksa hasil kerja, dan belajar dari masalah. Mutu bukan hanya tanggung
jawab QA; semua anggota tim berkontribusi pada prosesnya.

Praktik budaya mutu meliputi:

- Menentukan kriteria selesai agar tim memiliki pemahaman yang sama tentang
  hasil yang dapat diterima.
- Mencatat perubahan agar keputusan dan riwayat pekerjaan dapat ditelusuri.
- Melakukan code review untuk memeriksa perubahan sebelum diterapkan.
- Menulis dan menjalankan pengujian yang dapat diulang.
- Menyediakan dokumentasi yang cukup untuk menjelaskan penggunaan atau
  keputusan penting.
- Melaporkan masalah berdasarkan bukti tanpa menyalahkan orang.

Jika bug kritis ditemukan setelah rilis, tim perlu mencatat dan mereproduksi
masalah, menentukan prioritas, memperbaikinya, lalu menjalankan uji regresi.
Uji regresi memastikan perbaikan tidak merusak fungsi yang sebelumnya sudah
berjalan.

### Praktik mutu sebelum dan selama implementasi

Mutu lebih mudah dijaga jika diperhatikan sejak awal, bukan hanya diperiksa
setelah semua kode selesai. Tim dapat:

- menyepakati **kriteria penerimaan** untuk fitur tertentu dan **kriteria
  selesai** untuk pekerjaan secara umum;
- membagi pekerjaan menjadi perubahan yang cukup kecil agar mudah ditinjau;
- memakai standar penamaan, struktur, dan gaya kode yang konsisten;
- meminta rekan melakukan **code review** untuk memeriksa kesesuaian kebutuhan,
  keterbacaan, dampak perubahan, dan potensi kesalahan;
- membuat pengujian yang dapat dijalankan kembali, serta mencatat hasilnya;
- memperbarui dokumentasi, catatan versi, atau panduan penggunaan jika
  perubahan memengaruhi pembaca atau pengguna.

Kriteria selesai bukan hanya "kode sudah ditulis". Contohnya, suatu perubahan
baru dinyatakan selesai setelah memenuhi kriteria penerimaan, diperiksa oleh
rekan sesuai aturan tim, diuji, dan dokumentasi yang terpengaruh diperbarui.
Definisi ini perlu proporsional: pekerjaan berisiko tinggi mungkin memerlukan
peninjauan dan pengujian lebih ketat.

### Menulis laporan bug yang dapat ditindaklanjuti

Laporan yang baik membantu orang lain memahami dan mengulang masalahnya.
Cantumkan ringkasan, versi atau lingkungan, prasyarat, langkah reproduksi,
hasil yang diharapkan, hasil aktual, dampak, dan bukti yang relevan. Hindari
laporan seperti "aplikasi rusak" tanpa rincian yang dapat diuji.

Tim dapat membedakan **severity** (seberapa besar dampak masalah) dan
**priority** (seberapa segera masalah ditangani dibanding pekerjaan lain).
Bug berdampak besar sering mendapat prioritas tinggi, tetapi prioritas juga
dipengaruhi jumlah pengguna terdampak, kemungkinan terjadi, solusi sementara,
risiko, dan komitmen rilis. Prioritas ditentukan dengan konteks tim, bukan
hanya angka.

### Perbaikan dan pembelajaran

Setelah masalah dikonfirmasi, tim menentukan pemilik dan langkah penanganan,
membuat perbaikan, menjalankan pengujian yang relevan, dan mengecek dampak
samping. Uji regresi mencakup fungsi yang sudah berjalan dan berpotensi
terpengaruh oleh perubahan. Setelah rilis, pemantauan membantu memastikan
perbaikan efektif di lingkungan nyata.

Jika masalah berulang, tinjau penyebab pada proses maupun sistem: apakah
kebutuhan kurang jelas, skenario uji terlewat, komunikasi tidak sampai, atau
mekanisme pemantauan kurang. Tujuannya memperbaiki cara kerja agar kejadian
serupa lebih kecil kemungkinannya, bukan mencari siapa yang patut disalahkan.
Perubahan dan keputusan dicatat agar pembelajaran tidak hilang.

## Contoh

QA menemukan checkout gagal pada kondisi tertentu. Tim mencatat langkah untuk
mengulangi kegagalan, memprioritaskan dampaknya, memperbaiki penyebabnya, lalu
menguji kembali checkout serta fungsi terkait. Hasil dan perubahan dicatat agar
anggota tim lain dapat menelusurinya.

## Latihan

1. Bukti praktik budaya mutu yang dapat ditelusuri adalah **test case, code
   review, dan changelog**.
2. Apa langkah yang tepat untuk menangani bug kritis setelah rilis?
   **Catat, reproduksi, prioritaskan, perbaiki, lalu uji regresi.**
3. Mengapa masalah dilaporkan tanpa menyalahkan orang? **Agar tim berfokus pada
   bukti dan perbaikan.**
4. Informasi apa yang membantu QA mengulang suatu bug? **Lingkungan/versi,
   prasyarat, langkah reproduksi, hasil aktual, dan hasil yang diharapkan.**
5. Apa beda severity dan priority? **Severity menggambarkan dampak; priority
   menentukan urutan atau kesegeraan penanganan berdasarkan konteks.**
6. Mengapa perlu uji regresi setelah perbaikan? **Untuk memastikan perubahan
   memperbaiki masalah tanpa merusak fungsi lain yang sudah berjalan.**

## Checklist

- [ ] Dapat menyebutkan contoh praktik budaya mutu.
- [ ] Dapat menjelaskan fungsi kriteria selesai dan pencatatan perubahan.
- [ ] Dapat mengurutkan penanganan bug kritis setelah rilis.
- [ ] Dapat membuat laporan bug yang dapat direproduksi.
- [ ] Dapat membedakan severity dan priority.
