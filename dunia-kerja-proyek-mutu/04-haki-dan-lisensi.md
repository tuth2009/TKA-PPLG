# HAKI dan Lisensi dalam Pengembangan (`P1`)

## Target belajar

Mengenali bentuk HAKI yang berkaitan dengan produk digital dan memahami
pentingnya memeriksa izin penggunaan sebelum mendistribusikan produk.

## Materi

Produk perangkat lunak dan gim dapat memuat karya serta identitas yang
dilindungi. Hal-hal yang perlu diperhatikan antara lain:

- **Hak cipta** atas kode dan aset seperti gambar, audio, atau materi lainnya.
- **Lisensi dependensi** yang mengatur cara library atau komponen pihak lain
  boleh digunakan dan didistribusikan.
- **Merek** yang berkaitan dengan nama atau identitas produk.
- **Izin penggunaan konten** yang menentukan apakah suatu konten boleh
  digunakan dalam produk.

Sebelum library atau aset digunakan dan produk didistribusikan, tim perlu
membaca serta mematuhi ketentuan lisensinya. Penggunaan suatu komponen tidak
otomatis berarti semua batasan lisensinya boleh diabaikan.

### Hak cipta, lisensi, dan merek

Hak cipta berkaitan dengan karya, misalnya kode, ilustrasi, musik, foto,
video, font, dan dokumentasi. Saat memakai karya milik pihak lain, tim perlu
memastikan izin yang berlaku mencakup cara penggunaan yang direncanakan.
Mencantumkan nama pembuat saja tidak otomatis menggantikan izin apabila
lisensinya mensyaratkan izin atau kewajiban lain.

Lisensi memberi ketentuan tentang penggunaan suatu perangkat lunak atau aset.
Perangkat lunak **open-source** dapat dipelajari, digunakan, atau
didistribusikan berdasarkan lisensinya; istilah tersebut bukan berarti
"tanpa hak cipta" atau "bebas syarat". Secara umum, lisensi permisif cenderung
mengizinkan penggunaan luas dengan kewajiban tertentu, sedangkan beberapa
lisensi copyleft dapat mewajibkan karya turunan yang didistribusikan mengikuti
ketentuan lisensi tertentu. Detailnya bergantung pada teks lisensi dan cara
komponen digunakan, jadi jangan mengambil kesimpulan hanya dari nama
kategori.

Merek membantu membedakan produk atau layanan. Sebelum memilih nama produk,
periksa agar pengguna tidak keliru mengira produk memiliki hubungan atau
dukungan dari pemilik merek lain. Perlindungan dan aturan HAKI dapat bergantung
pada yurisdiksi; penjelasan ini adalah materi umum, bukan nasihat hukum.

### Inventaris dan pemeriksaan dependensi/aset

Sebelum rilis, tim sebaiknya memiliki catatan komponen pihak lain yang dipakai.
Untuk setiap library atau aset, catat nama, versi, sumber, lisensi/izin, dan
lokasi teks lisensi. Periksa juga dependensi tidak langsung yang ikut
digunakan, karena aplikasi dapat mendistribusikan komponen yang tidak dipilih
secara langsung.

Langkah pemeriksaan yang dapat diterapkan:

1. Pastikan komponen berasal dari sumber yang dapat dikenali dan versinya
   diketahui.
2. Baca lisensi atau izin yang berlaku untuk versi dan aset tersebut.
3. Cocokkan ketentuan dengan tujuan penggunaan: penggunaan internal,
   modifikasi, distribusi, atau penggunaan komersial bila relevan.
4. Catat dan penuhi kewajiban, misalnya menyertakan teks lisensi,
   pemberitahuan hak cipta, atribusi, atau menyediakan informasi tertentu
   jika diwajibkan.
5. Periksa hak penggunaan untuk aset seperti font, musik, gambar, model 3D,
   dan paket gim secara terpisah; izin untuk satu aset tidak otomatis berlaku
   pada aset lain.
6. Tinjau ulang catatan ketika versi dependensi atau cara distribusi berubah.

Jika izin atau sumber tidak jelas, jangan menganggap materi itu bebas
digunakan. Pilih alternatif dengan ketentuan yang jelas atau minta klarifikasi
kepada pemegang hak. Untuk peluncuran komersial atau ketidakpastian hukum yang
penting, mintalah peninjauan dari pihak yang kompeten.

## Contoh

Sebuah aplikasi menggunakan library pihak lain. Sebelum merilis aplikasi, tim
memeriksa lisensi library tersebut dan mengikuti ketentuannya dalam penggunaan
serta distribusi.

## Latihan

1. Apa yang perlu dilakukan terhadap lisensi library sebelum distribusi?
   **Dibaca dan dipatuhi.**
2. Sebutkan dua hal yang mungkin terkait HAKI dalam produk digital.
   **Hak cipta kode/aset dan lisensi dependensi.**
3. Apakah aset yang ditemukan di internet otomatis bebas digunakan?
   **Tidak; izin penggunaan dan ketentuannya harus diperiksa.**
4. Apakah mencantumkan kredit selalu cukup untuk memenuhi lisensi?
   **Tidak; ikuti semua kewajiban dalam lisensi. Kredit saja belum tentu cukup.**
5. Mengapa versi dependensi perlu dicatat? **Agar tim dapat mengetahui lisensi
   komponen yang benar-benar dipakai dan meninjau ulang ketika versi berubah.**
6. Apa yang sebaiknya dilakukan jika izin aset tidak diketahui?
   **Jangan menganggapnya bebas; cari izin yang jelas, ganti aset, atau minta
   klarifikasi pemegang hak.**

## Checklist

- [ ] Dapat menyebutkan contoh HAKI dan lisensi dalam produk digital.
- [ ] Memahami bahwa lisensi dependensi perlu diperiksa sebelum distribusi.
- [ ] Memeriksa izin penggunaan aset dan konten yang digunakan.
- [ ] Mencatat versi, sumber, lisensi, dan kewajiban komponen pihak lain.
