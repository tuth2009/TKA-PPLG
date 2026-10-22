# Dasar K3LH, Budaya Kerja, Aset, dan Sistem Operasi (`P1`)

## Tujuan belajar

Memahami cara menyiapkan lingkungan kerja PPLG yang aman dan profesional,
serta mengelola perangkat dan berkas proyek agar terlindungi dan mudah
ditelusuri.

## Prasyarat

- [Peta prasyarat PPLG](../00-peta-prasyarat.md)
- Pemahaman dasar tentang perangkat komputer dan berkas digital.

## Materi

Pekerjaan PPLG tidak hanya melibatkan penulisan kode. Tim juga perlu menjaga
keselamatan dan kesehatan, berkomunikasi secara profesional, melindungi
informasi, serta mengatur aset proyek dan berkas kerja. Kebiasaan ini
mendukung pekerjaan yang aman, kolaboratif, dan dapat dilanjutkan oleh anggota
tim lain.

### Keselamatan dan kesehatan kerja

Bahaya di ruang kerja dapat berasal dari perangkat listrik yang rusak, kabel
melintang, ventilasi yang terhalang, posisi kerja yang tidak ergonomis, atau
paparan layar terlalu lama. Untuk menangani risiko:

1. Identifikasi bahaya.
2. Nilai kemungkinan dan dampak yang dapat terjadi.
3. Pilih pengendalian yang sesuai, mulai dari eliminasi, substitusi, rekayasa,
   administratif, lalu alat pelindung diri (APD) bila diperlukan.
4. Laporkan insiden atau kondisi berbahaya agar ditindaklanjuti.

Jangan menangani perangkat listrik atau peralatan berbahaya di luar
kewenangan dan kompetensi. Atur posisi kerja, ambil jeda, dan pastikan
ventilasi perangkat tidak terhalang.

### Budaya kerja profesional

Budaya kerja profesional mencakup disiplin terhadap kesepakatan, komunikasi
yang jelas dan saling menghormati, serta tanggung jawab atas pekerjaan.
Lindungi privasi pengguna dan rekan kerja: periksa log, tangkapan layar, dan
berkas sebelum dibagikan. Password, token, dan kredensial lain harus tetap
rahasia dan tidak dimasukkan ke repository. Kode dan aset digital juga harus
digunakan sesuai sumber, izin, dan lisensinya.

### Aset dan berkas proyek

Aset proyek meliputi perangkat fisik serta sumber kode, konfigurasi, konten,
dokumentasi, database, dan hasil build. Gunakan struktur folder dan penamaan
yang konsisten agar aset mudah ditemukan. Version control membantu menelusuri
perubahan; backup membantu pemulihan dan perlu diuji agar dapat diandalkan.

Berikan hak akses secukupnya (**least privilege**) dan jangan menyimpan secret
di repository. Catat sumber serta izin aset konten, dan periksa path serta
backup sebelum menghapus atau memindahkan berkas.

Sistem operasi menyediakan cara untuk menjalankan aplikasi dan mengelola
berkas. File menyimpan data, sedangkan folder/direktori mengelompokkan file.
Path absolut menunjukkan lokasi dari titik awal sistem berkas; path relatif
menunjukkan lokasi berdasarkan direktori kerja. Permission menentukan apakah
file dapat dibaca, diubah, atau dijalankan. Pastikan direktori kerja dan path
benar sebelum melakukan perubahan.

## Contoh

Sebelum mengirim laporan bug ke tim, pastikan kabel dan perangkat di area
kerja aman, lalu hapus data pribadi atau token dari tangkapan layar dan log.
Simpan laporan di direktori dokumentasi yang disepakati, gunakan path yang
benar, dan atur akses hanya untuk pihak yang memerlukannya. Jika laporan
memakai gambar dari luar proyek, pastikan sumber dan izinnya jelas.

## Latihan

1. Kabel melintang di jalur berjalan. Apa langkah yang tepat? →
   **Amankan area dan rapikan atau minta penanganan sesuai prosedur, lalu
   laporkan bila diperlukan.**
2. Berkas konfigurasi berisi token akan dikirim ke repository. Apa yang harus
   dilakukan? → **Jangan commit token; gunakan mekanisme pengelolaan secret
   yang disetujui.**
3. Apa fungsi backup dan version control? → **Backup membantu pemulihan;
   version control menelusuri perubahan.**
4. Apa beda path absolut dan path relatif? → **Absolut merujuk dari titik
   awal sistem berkas; relatif bergantung pada direktori kerja.**
5. Sebelum menghapus aset, apa yang perlu diperiksa? → **Path, riwayat atau
   perubahan, hak akses, dan ketersediaan backup.**

## Checklist

- [ ] Mengidentifikasi bahaya umum di ruang kerja dan memilih pengendalian
  sesuai risiko.
- [ ] Menjaga komunikasi, privasi, kredensial, dan kepatuhan lisensi.
- [ ] Membedakan aset fisik dan digital serta menata berkas proyek.
- [ ] Menjelaskan peran version control, backup, dan least privilege.
- [ ] Membedakan path absolut dan relatif serta memahami permission.
- [ ] Memastikan path dan backup sebelum memindahkan atau menghapus berkas.

Lanjutkan ke [K3LH di lingkungan kerja PPLG](01-k3lh.md).
