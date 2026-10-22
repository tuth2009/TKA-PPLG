# Sumber resmi Pusmendik untuk TKA SMK (PPLG + Matematika Tingkat Lanjut)

Dokumen ini adalah catatan bukti dan batas cakupan untuk paket belajar TKA di
repositori ini. Seluruh halaman di bawah dibaca melalui `agent-browser` pada
29 Agustus 2026 (WIB). Periksa kembali indeks Unduhan bila Pusmendik menerbitkan
revisi baru.

Fase ini sengaja memprioritaskan Markdown dan halaman HTML interaktif. PDF
tidak dijadikan input isi modul; bila nanti perlu mengekstrak PDF, gunakan
Python melalui `uv` sesuai aturan kerja proyek.

## 1. Sumber utama dan format asesmen

### Sumber yang harus diprioritaskan

1. [Beranda TKA Pusmendik](https://pusmendik.kemendikdasmen.go.id/tka/) —
   menjelaskan tujuan TKA, daftar mata pelajaran, FAQ bentuk soal, dan prinsip
   bahwa soal mengukur kompetensi mata pelajaran serta tetap menekankan
   penalaran dan pemecahan masalah.
2. [Indeks Kerangka Asesmen SMA/MA/SMK/MAK/Sederajat](https://pusmendik.kemendikdasmen.go.id/tka/tka/view/mata-pelajaran-wajib/sma)
   — halaman indeks dinamis yang memuat tautan mata pelajaran wajib dan
   pilihan. Halaman ini juga dapat dibuka dari URL pilihan yang diberikan pada
   permintaan awal.
3. [Indeks Unduhan Pusmendik](https://pusmendik.kemendikdasmen.go.id/tka/page/download)
   — daftar dokumen hukum/kerangka asesmen resmi. Pada tanggal akses,
   indeks menampilkan antara lain:

   - *Salinan Peraturan Kepala BKPDM Nomor 1 Tahun 2026 tentang Kerangka
     Asesmen Tes Kemampuan Akademik pada Sekolah Menengah Kejuruan/Madrasah
     Aliyah Kejuruan*;
   - *Kepmendikdasmen Nomor 56 Tahun 2026 tentang Pedoman Penyelenggaraan
     TKA-AN*;
   - *Petunjuk Teknis TKA-AN 2026*;
   - *Perka BSKAP 45-H-AN-2025 tentang Kerangka Asesmen TKA Jenjang SMA,
     MA sederajat dan SMK, MAK*;
   - *Permendikdasmen Nomor 9 Tahun 2025 tentang Tes Kemampuan Akademik*; dan
   - *Kepmendikdasmen Nomor 102/M/2025 tentang Mata Pelajaran Pendukung
     Program Studi dalam SNBP*.

   Gunakan tombol **Unduh** pada indeks untuk mengambil berkas. URL teknis
   `download_file/<kode>` yang tampil di halaman dapat berganti token ketika
   halaman dimuat ulang; karena itu indeks di atas adalah tautan rujukan yang
   lebih tahan perubahan. Untuk SMK, dokumen khusus BKPDM Nomor 1 Tahun 2026
   adalah rujukan terbaru yang tercantum di indeks pada tanggal riset. Indeks
   masih menampilkan dokumen 2025 sebagai dokumen pendamping/versi terdahulu;
   halaman ini tidak, dengan sendirinya, menyatakan status pencabutan dokumen
   tersebut.

### Klaim format yang terlihat pada FAQ resmi

Menurut [FAQ di beranda TKA](https://pusmendik.kemendikdasmen.go.id/tka/):

- Untuk jenjang SMA/MA/SMK/MAK, mata pelajaran yang diujikan adalah **Bahasa
  Indonesia, Matematika, Bahasa Inggris, dan dua mata pelajaran pilihan**.
  PPLG dan Matematika Tingkat Lanjut adalah dua pilihan yang dipakai dalam
  paket ini.
- Pilihan ganda biasa (PG) mempunyai satu jawaban benar. Pilihan ganda
  kompleks (PGK) dapat mempunyai lebih dari satu jawaban benar. Contoh di
  halaman mapel juga memakai bentuk PGK kategori (pernyataan benar/salah) dan
  PGK MCMA (memilih semua jawaban benar).
- Soal TKA sama-sama dikembangkan dengan mempertimbangkan kompetensi/materi
  yang berlaku pada Kurikulum 2013 dan Kurikulum Merdeka.
- TKA bukan pengukuran literasi/numerasi umum seperti AN; yang diukur adalah
  kompetensi mata pelajaran sesuai kurikulum. Penalaran dan pemecahan masalah
  tetap ditekankan.
- TKA bersifat sukarela dan tidak menentukan kelulusan menurut FAQ tersebut.
  Informasi ini adalah konteks penyelenggaraan, bukan materi yang perlu
  dihafalkan untuk menjawab soal.

Tidak ada klaim jumlah soal atau durasi di halaman kerangka mapel yang dipakai
di sini. Jangan menambahkan angka jumlah soal/waktu ke modul tanpa rujukan dari
petunjuk teknis/ketetapan penyelenggaraan terbaru.

## 2. Peta sumber per mata pelajaran

| Mapel | Halaman kerangka resmi | Cara menurunkan materi |
|---|---|---|
| Matematika wajib | [Halaman Matematika](https://pusmendik.kemendikdasmen.go.id/tka/tka/view/mata-pelajaran-wajib/sma/matematika) | Ambil bagian **Muatan**, **Kompetensi**, dan **Matriks Asesmen**; contoh soal dipakai untuk memeriksa karakter tugas. |
| Bahasa Indonesia wajib | [Halaman Bahasa Indonesia](https://pusmendik.kemendikdasmen.go.id/tka/tka/view/mata-pelajaran-wajib/sma/bahasa-indonesia) | Fokuskan modul pada keterampilan membaca dan tiga kompetensi membaca yang ditulis Pusmendik. |
| Bahasa Inggris wajib | [Halaman Bahasa Inggris](https://pusmendik.kemendikdasmen.go.id/tka/tka/view/mata-pelajaran-wajib/sma/bahasa-inggris) | Turunkan latihan dari jenis teks, konteks, tingkat A2/B1, dan matriks membaca; jangan menjadikan grammar terpisah sebagai kisi-kisi. |
| Matematika Tingkat Lanjut | [Halaman Matematika Tingkat Lanjut](https://pusmendik.kemendikdasmen.go.id/tka/tka/view/mata-pelajaran-pilihan/sma/matematika-tingkat-lanjut) | Pakai batasan ukuran/orde/komponen dan submateri persis pada matriks. |
| SMK-PPLG | [Halaman PPLG](https://pusmendik.kemendikdasmen.go.id/tka/tka/view/mata-pelajaran-pilihan/sma/pengembangan-perangkat-lunak-dan-gim-smk-mak) | Pakai elemen, subelemen, kompetensi, dan batasan/catatan PPLG; sumber muatannya adalah CP PPLG Fase E. |

Pada setiap halaman, Pusmendik menampilkan tab **Definisi**, **Muatan**,
**Kompetensi**, **Matriks Asesmen**, dan **Contoh Soal**. Isi modul belajar
sebaiknya dipetakan terutama ke tiga tab pertama dan matriks; contoh soal
resmi digunakan untuk mengamati bentuk penalaran, bukan disalin massal.

## 3. SMK — Pengembangan Perangkat Lunak dan Gim (PPLG)

### Definisi dan sumber kurikulum

Halaman [kerangka PPLG](https://pusmendik.kemendikdasmen.go.id/tka/tka/view/mata-pelajaran-pilihan/sma/pengembangan-perangkat-lunak-dan-gim-smk-mak)
mendefinisikan TKA PPLG sebagai pengukuran **penguasaan konsep, penalaran,
dan penerapan pengetahuan dasar kejuruan** di bidang pengembangan perangkat
lunak dan gim. Halaman itu menyebut ruang lingkup: proses bisnis; perkembangan
teknologi dan dunia kerja; profesi dan kewirausahaan; K3LH dan budaya kerja;
perangkat/tools; basis data; aset dan antarmuka pengguna; algoritma;
pemrograman terstruktur; serta pemrograman berorientasi objek.

Tab Muatan menyatakan bahwa muatan PPLG merujuk pada elemen/materi esensial
**Capaian Pembelajaran Program Keahlian PPLG Fase E** sebagaimana Salinan
Keputusan Kepala BSKAP Nomor **046/H/KR/2025**. Ini adalah alasan modul PPLG
tidak boleh dipersempit menjadi hafalan sintaks satu bahasa pemrograman.

### Muatan dan matriks yang harus dipelajari

#### A. Wawasan dunia kerja bidang PPLG

- **Profesi dan Kewirausahaan PPLG:** jenis profesi dan tugas utamanya,
  peluang usaha, serta prinsip kewirausahaan/technopreneurship perangkat
  lunak dan gim.
- **Manajemen Proyek dan Budaya Mutu:** tahapan dasar manajemen proyek,
  proses bisnis pengembangan perangkat lunak/gim, dan prinsip budaya mutu.

#### B. Kecakapan kerja dasar, K3, dan budaya kerja

- **K3LH dan Budaya Kerja Profesional:** prinsip K3LH, etika kerja, budaya
  kerja profesional, dan karakter lingkungan kerja PPLG.
- **Pengelolaan Aset Fisik dan Digital:** perangkat kerja, file proyek,
  direktori, aset digital, source code, media, basis data, dan dokumentasi
  proyek; termasuk menerapkan prosedur pengelolaannya pada skenario kerja.

#### C. Teknologi jaringan komputer

- **Lingkungan Sistem Operasi untuk Pengembangan:** pengelolaan file dan
  direktori proyek serta konfigurasi dasar lingkungan pengembangan pada
  sistem operasi.
- **Infrastruktur dan Perangkat Jaringan:** konfigurasi jaringan dasar untuk
  memastikan konektivitas pada lingkungan pengembangan.
- **Arsitektur dan Mekanisme TCP/IP:** fungsi layer TCP/IP dan protokol,
  mekanisme komunikasi berbasis TCP/IP, serta analisis gangguan koneksi.

  Muatan resmi menjelaskan konteks yang perlu dipahami: alamat IP,
  konektivitas antarperangkat, client-server, HTTP/HTTPS, akses basis data
  atau API melalui jaringan, dan dampak koneksi pada pengembangan, pengujian,
  serta distribusi aplikasi/gim.

#### D. Pemrograman terstruktur

- **Struktur Data dan Tipe Data:** menganalisis pemilihan tipe/struktur data
  pada potongan program atau skenario algoritmik.
- **Struktur Kontrol Program:** percabangan, perulangan, alur logika, dan
  efektivitas struktur kontrol.
- **Modularisasi Program:** fungsi, prosedur, pembagian modul, dan evaluasi
  efektivitas desain modular.

#### E. Pemrograman berorientasi objek (OOP)

- **Konsep Dasar dan Prinsip OOP:** class, object, atribut, method, dan
  prinsip dasar OOP.
- **Enkapsulasi dan Access Modifier:** access modifier, enkapsulasi,
  accessor/mutator (getter/setter), atribut, dan method.
- **Pewarisan:** relasi superclass-subclass dan penerapan inheritance.
- **Polymorphism:** method overriding, superclass/subclass, referensi objek,
  dan pemanggilan perilaku sesuai objek.

### Kompetensi/kognitif PPLG

Tab Kompetensi halaman resmi menyebut empat kemampuan lintas-materi:

1. **Pemahaman konseptual:** proses bisnis, lingkungan kerja, K3LH,
   teknologi penunjang, pemrograman terstruktur, dan OOP.
2. **Penerapan konsep:** menggunakan konsep PPLG untuk masalah kontekstual
   di lingkungan pengembangan perangkat lunak/gim.
3. **Analisis dan evaluasi:** menganalisis efektivitas solusi, struktur
   program, modularisasi, OOP, dan teknologi jaringan untuk pengembangan,
   pengujian, atau distribusi.
4. **Berpikir komputasional:** logika program, struktur data, dekomposisi,
   pola algoritmik, dan penyelesaian masalah berbasis algoritma.

Proses berpikir menurut level yang ditampilkan halaman:

| Level | Proses yang perlu dilatih | Inti tuntutan |
|---|---|---|
| Pengetahuan dan Pemahaman | Mengidentifikasi, menjelaskan, melaksanakan, menerapkan | Profesi/tahap proyek; kewirausahaan, budaya mutu, K3LH, etika; pengelolaan file/direktori; konfigurasi dasar; class-object dan inheritance. |
| Penerapan dan Implementasi | Mengimplementasikan | Konfigurasi jaringan dasar, komunikasi data, OOP, enkapsulasi, dan polymorphism untuk pengembangan/pengujian/perancangan. |
| Penalaran | Menganalisis, mengevaluasi, mengklasifikasi | Kendala koneksi, alur logika, pembagian fungsi/prosedur, tipe/struktur data, efektivitas kontrol/modularisasi, serta ketepatan access modifier, enkapsulasi, inheritance, dan polymorphism. |

Contoh resmi memperlihatkan konteks soal: peran UI/UX, permission file server
lokal, modularisasi fungsi, alamat IP di topologi aplikasi, perulangan dan
perhitungan, serta polymorphism melalui overriding. Contoh ini menguatkan
bahwa latihan harus berupa skenario/analisis potongan program, bukan hanya
definisi istilah.

Catatan batas: UI/UX, tools pengembangan, dan basis data dasar disebut pada
definisi ruang lingkup PPLG, tetapi halaman yang dibaca tidak memberi
subelemen matriks terpisah untuk masing-masingnya. Jadikan hal-hal tersebut
konteks pengelolaan aset/proyek dan verifikasi kembali PDF kerangka terbaru
sebelum membuat bab yang lebih luas dari matriks di atas.

## 4. Matematika Tingkat Lanjut (mapel pilihan)

### Definisi, muatan, dan kemampuan kognitif

[Halaman Matematika Tingkat Lanjut](https://pusmendik.kemendikdasmen.go.id/tka/tka/view/mata-pelajaran-pilihan/sma/matematika-tingkat-lanjut)
menyatakan bahwa asesmen mengukur pemahaman fakta, konsep, prinsip, dan
prosedur matematika serta penerapannya untuk pemecahan masalah. Muatannya
terdiri atas tiga elemen:

- **Aljabar**;
- **Geometri dan Pengukuran**; dan
- **Kalkulus**.

Logika matematika diintegrasikan ke elemen tersebut. Konteks dapat berupa
masalah matematika maupun situasi keseharian personal, keluarga, lingkungan
sekitar, lokal, atau global.

Kognitif yang ditampilkan halaman adalah:

| Level | Proses berpikir resmi | Terjemahan untuk latihan |
|---|---|---|
| 1 — Pengetahuan dan Pemahaman | Menghitung; memahami informasi; mengelompokkan; mengidentifikasi | Hitung prosedural, baca grafik/tabel/diagram/infografis, kenali objek dan konsep. |
| 2 — Aplikasi | Memodelkan; menerapkan; menginterpretasi | Ubah konteks menjadi pernyataan matematika, gunakan strategi pada masalah rutin, jelaskan makna representasi/hasil. |
| 3 — Penalaran | Menganalisis; memecahkan masalah; mengevaluasi | Hubungkan beberapa konsep, selesaikan konteks baru/tidak rutin, dan bandingkan strategi/solusi. |

Catatan pembacaan: tabel HTML Pusmendik memuat satu baris **Mengidentifikasi**
yang berulang pada Level 1. Di sini proses itu dicatat sekali karena duplikasi
tersebut tampak sebagai pengulangan tampilan, bukan kompetensi baru.

### Matriks materi resmi

#### A. Aljabar

- **Matriks:** determinan, invers, dan operasi matriks. Matriks berisi
  bilangan real; determinan/invers dibatasi ukuran **2×2 atau 3×3**. Pada
  halaman web, teks kompetensi menempelkan frasa “Program linear” setelah
  “Operasi matriks”; perlakukan ini sebagai catatan rendering dan verifikasi
  ke PDF kerangka terbaru sebelum menjadikannya bab tersendiri.
- **Polinomial:** operasi, pemfaktoran, dan suku sisa. Orde polinomial
  maksimum **4** dan seluruh koefisien bilangan real.
- **Fungsi:** domain, kodomain, range, dan grafik fungsi polinom, rasional,
  akar, eksponensial, logaritma, mutlak, dan trigonometri. Fungsi polinom
  maksimum orde **4**; bilangan pokok fungsi eksponensial berupa bilangan
  asli.

#### B. Geometri dan Pengukuran

- **Vektor:** vektor pada bidang dan ruang, panjang vektor, dan operasi
  vektor; komponen maksimum **tiga**.
- **Lingkaran:** persamaan lingkaran, persamaan garis singgung, luas/keliling
  daerah lingkaran atau sebagian daerah lingkaran.
- **Transformasi Geometri:** translasi, refleksi, rotasi, dilatasi, dan
  komposisinya pada bentuk geometris serta matriks transformasinya. Bentuk
  yang ditransformasi meliputi titik, garis, dan bangun datar.

#### C. Kalkulus yang benar-benar tercantum

Matriks halaman memberi baris **Elemen/Materi: Trigonometri; Sub-elemen:
Limit** (label elemen ini tampak tidak konsisten dengan Muatan yang menyebut
Kalkulus). Submaterinya adalah:

- limit fungsi aljabar; dan
- limit fungsi trigonometri,

dengan batasan **dapat diselesaikan tanpa Teorema L’Hopital**.

Tidak ada baris turunan atau integral pada matriks interaktif yang dibaca pada
29 Agustus 2026. Karena itu paket belajar tidak boleh menyatakan turunan atau
integral sebagai kisi-kisi resmi TKA MTK Tingkat Lanjut tanpa bukti dari revisi
kerangka yang lebih baru. Turunan/integral boleh muncul hanya sebagai
pengetahuan pengayaan/prasyarat apabila modul secara eksplisit menandainya
sebagai bukan submateri yang tercantum.

Contoh soal resmi mencakup determinan/invers/operasi matriks, periode dan
identifikasi grafik fungsi, vektor, persamaan lingkaran/garis singgung,
transformasi, limit aljabar, limit trigonometri, polinomial, dan suku sisa;
contoh-contoh tersebut cocok dipakai untuk memeriksa bahwa peta materi di atas
tidak terlalu sempit.

## 5. Matematika wajib

### Muatan dan kompetensi umum

Menurut [halaman Matematika wajib](https://pusmendik.kemendikdasmen.go.id/tka/tka/view/mata-pelajaran-wajib/sma/matematika),
elemen yang diukur adalah **bilangan, aljabar, geometri dan pengukuran, data
dan peluang, serta trigonometri**. Logika matematika diintegrasikan dalam
elemen tersebut. Masalah dapat berada dalam konteks matematika atau keseharian
(personal, keluarga, lingkungan sekitar, lokal, dan global).

Definisi dan tiga level proses berpikirnya sama pola umumnya dengan MTK TL:

- **Pengetahuan dan Pemahaman:** menghitung; memahami informasi dari grafik,
  tabel, diagram, infografis/visual; mengelompokkan; mengidentifikasi.
- **Aplikasi:** memodelkan; menerapkan strategi/operasi; menginterpretasikan
  situasi, pernyataan, representasi, atau masalah.
- **Penalaran:** menganalisis; memecahkan masalah baru/tidak rutin;
  mengevaluasi alternatif strategi/solusi; menyimpulkan; melakukan
  generalisasi; menjustifikasi langkah atau argumen matematis.

### Matriks materi wajib

- **Bilangan Real:** jenis dan sifat bilangan; operasi penjumlahan,
  pengurangan, perkalian, pembagian, gabungan, serta sifat komutatif,
  asosiatif, dan distributif. Cakupan bilangan real termasuk bilangan asli
  berpangkat bilangan bulat atau pecahan.
- **Persamaan/Pertidaksamaan Linear:** sistem persamaan linear multivariabel,
  sistem pertidaksamaan linear multivariabel, dan program linear. Banyak
  variabel maksimum **tiga**.
- **Fungsi:** domain, kodomain, range, serta representasi fungsi linear,
  kuadrat, dan rasional dalam berbagai bentuk; invers dan representasinya;
  komposisi dan representasinya. Identifikasi fungsi dapat analitis dan
  grafis.
- **Barisan dan Deret:** aritmetika dan geometri, termasuk penerapan pada
  pertumbuhan, peluruhan, bunga tunggal, dan bunga majemuk.
- **Objek Geometri:** hubungan dua sudut/garis/bidang; hubungan objek pada
  bangun datar/ruang; kesebangunan/kekongruenan; Teorema Pythagoras.
  Bangun datar yang disebut ialah segitiga, segi empat, lingkaran, dan
  gabungannya; bangun ruang meliputi bangun beraturan dengan sisi datar dan
  lengkung. Jarak dapat berupa titik-titik, garis-garis, bidang-bidang,
  titik-garis, dan titik-bidang.
- **Transformasi Geometri:** translasi, refleksi, rotasi, dilatasi, dan
  komposisinya pada **titik**.
- **Pengukuran:** keliling/luas bangun datar, volume/luas permukaan bangun
  ruang, dan jarak dua objek geometri.
- **Perbandingan Trigonometri:** sinus, kosinus, tangen, kotangen, sekan,
  dan kosekan.
- **Data:** penyajian dengan diagram batang, garis, lingkaran, grafik, tabel,
  dan bentuk visual; ukuran pemusatan dan penyebaran data tunggal maupun
  kelompok. Bullet ketiga pada matriks HTML yang dibaca berhenti pada kata
  **“Aturan”**, sehingga bagian itu adalah keterbatasan sumber yang harus
  dicatat, bukan dilengkapi sebagai fakta tanpa verifikasi.

  Contoh soal pada halaman yang sama secara eksplisit memuat **peluang suatu
  kejadian majemuk** dan **aturan pencacahan** (aturan penjumlahan, perkalian,
  permutasi, dan kombinasi). Karena itu topik peluang/pencacahan layak dibuat
  sebagai latihan berbasis contoh resmi, sambil mempertahankan catatan bahwa
  bullet matriks “Aturan” terpotong pada tampilan web.

## 6. Bahasa Indonesia wajib

Rujukan adalah [halaman Bahasa Indonesia wajib](https://pusmendik.kemendikdasmen.go.id/tka/tka/view/mata-pelajaran-wajib/sma/bahasa-indonesia).

### Muatan

TKA Bahasa Indonesia berfokus pada **membaca**. Teksnya terdiri atas:

- teks informasi tunggal maupun jamak, berisi fakta, konsep, prosedur, dan
  metakognisi dari berbagai bidang/topik, genre, dan konteks lokal, nasional,
  atau global;
- teks fiksi realisme atau absurd, dengan latar konkret/abstrak, tokoh
  berkarakter bulat, konflik tunggal/jamak dengan penyelesaian terbuka, alur
  campuran, dan sudut pandang campuran.

Karakteristik yang dijelaskan Pusmendik: kosakata umum/khusus, imbuhan
kompleks, kata abstrak, makna denotatif, istilah teknis, dan makna konotatif
dalam konteks luas; kalimat umumnya 8–12 kata dengan pola kompleks/inversi;
wacana memakai konjungsi antarparagraf bermakna pertentangan atau sebab-akibat
dan tanda baca yang mendukung makna; panjang teks sekitar **250–300 kata**
(kecuali puisi).

### Kompetensi/matriks

- **Pemahaman tekstual:** mengidentifikasi informasi tersurat; menyusun ulang,
  mengelompokkan, membuat ikhtisar, menyajikan kembali; mengenali kata
  serapan; menemukan latar/karakter/fenomena dari kosakata; menyusun kerangka
  atau bagan.
- **Pemahaman inferensial:** menyimpulkan ide pokok/gagasan pendukung,
  tokoh/peristiwa/latar/konflik/nilai; menjelaskan hubungan makna
  antarkalimat/paragraf; memprediksi lanjutan atau akhir uraian/cerita.
- **Evaluasi dan apresiasi:** menilai relevansi peristiwa dengan kehidupan,
  keakuratan/kesesuaian/kecukupan/ketepatan informasi, penggunaan bahasa,
  ketepatan penggambaran karakter/peristiwa/latar, serta menyimpulkan respons
  emosional terhadap puisi, prosa, dan drama.

Required knowledge pada modul Bahasa Indonesia harus membantu kemampuan membaca
di atas (kosakata dalam konteks, struktur paragraf, inferensi, bukti teks),
bukan mengubah asesmen menjadi ujian hafalan tata bahasa.

## 7. Bahasa Inggris wajib

Rujukan adalah [halaman Bahasa Inggris wajib](https://pusmendik.kemendikdasmen.go.id/tka/tka/view/mata-pelajaran-wajib/sma/bahasa-inggris).

### Muatan dan tingkat teks

TKA mengukur **keterampilan membaca** beragam teks dalam komunikasi sehari-hari,
vokasional, dan akademik. Jenis teks yang disebut ialah **descriptive,
recount, narrative, procedure, dan analytical exposition**. Topik merupakan
irisan kedua kurikulum dan menghindari kosakata teknis yang terlalu jarang
dipakai.

Target umum adalah tingkat **intermediate/B1 CEFR**:

- sekitar 250–350 kata;
- kosakata frekuensi tinggi sampai sekitar 3.000 kata;
- struktur kalimat sederhana dan kompleks; dan
- konteks sehari-hari, vokasional, atau akademik dasar yang berkaitan dengan
  minat/pengalaman/kebutuhan informasi umum.

Karena sebagian peserta berada di bawah B1, teks **A2** juga digunakan:

- sekitar 200–300 kata;
- kosakata frekuensi tinggi sampai sekitar 2.000 kata;
- struktur sederhana dan beberapa bentuk majemuk dasar; serta
- konteks sehari-hari/vokasional yang konkret dan dikenal.

### Kompetensi/matriks

- **Pemahaman tekstual:** menemukan informasi eksplisit, mengklasifikasi,
  membuat kerangka, meringkas, dan mensintesis informasi dari sumber lain.
- **Pemahaman inferensial:** menyimpulkan detail pendukung, topik/ide
  pokok/makna/target pembaca/tujuan/pesan moral, urutan kejadian,
  perbandingan, sebab-akibat, karakter tokoh, serta memprediksi hasil cerita.
- **Evaluasi dan apresiasi:** menilai realitas/fantasi, fakta/opini,
  kecukupan dan validitas informasi, kesesuaian bagian teks untuk
  menggambarkan karakter/aspek bacaan, serta menanggapi isi secara
  emosional/estetis.

Grammar dan kosakata pada paket belajar sebaiknya ditempatkan sebagai
**required knowledge untuk memahami teks**, bukan sebagai kisi-kisi mandiri
di luar keterampilan membaca yang dirumuskan halaman resmi.

## 8. Aturan pemakaian sumber pada modul

- Tandai setiap bab dengan elemen/subelemen resmi yang menjadi asalnya.
- Bagian **Required Knowledge** adalah jalur pedagogis agar peserta didik
  memahami materi; ia bukan klaim bahwa semua pengetahuan prasyarat itu akan
  muncul sebagai submateri terpisah di TKA.
- Untuk Matematika, tuliskan batasan numerik Pusmendik (maksimal tiga variabel,
  matriks 2×2/3×3, polinom orde 4, komponen vektor maksimal tiga, dan limit
  tanpa L’Hopital) di halaman materi yang relevan.
- Untuk PPLG, gunakan skenario pengembangan perangkat lunak/gim dan campurkan
  pertanyaan konsep, penerapan, analisis, serta evaluasi sesuai level resmi.
- Untuk Bahasa Indonesia/Inggris, gunakan bukti dari teks dan variasikan PG,
  PGK kategori, serta PGK MCMA sesuai contoh resmi.
- Bila isi halaman web dan PDF berbeda, simpan URL/versi dokumen yang
  diverifikasi dan prioritaskan kerangka terbaru yang berlaku untuk jenjang
  tersebut. Jangan menyimpulkan pencabutan atau menambah submateri hanya dari
  dugaan.
