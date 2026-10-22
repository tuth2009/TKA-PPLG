# Skenario K3LH, Budaya Kerja, Aset, dan Sistem Operasi (`P1`)

## Tujuan belajar

Menerapkan keselamatan kerja, etika profesional, perlindungan aset, serta
penggunaan path dan sistem berkas saat menangani masalah proyek.

## Prasyarat

- [Dasar K3LH, budaya kerja, aset, dan sistem operasi](../k3lh-aset-os/00-dasar-k3lh-aset-os.md)
- [K3LH di lingkungan kerja PPLG](../k3lh-aset-os/01-k3lh.md)
- [Budaya kerja profesional](../k3lh-aset-os/02-budaya-kerja.md)
- [Pengelolaan aset proyek](../k3lh-aset-os/03-pengelolaan-aset.md)
- [Sistem operasi, berkas, dan direktori](../k3lh-aset-os/04-sistem-operasi-file.md)

## Skenario: menyiapkan laporan insiden

Saat menguji aplikasi, anggota tim melihat kabel melintang di jalur berjalan.
Mereka juga menemukan token API di file konfigurasi yang akan dilampirkan
bersama log ke laporan bug. File berada di folder proyek yang path-nya belum
dipastikan.

Prioritaskan keselamatan: amankan area dan laporkan kondisi sesuai prosedur.
Nilai risiko dan utamakan penghilangan bahaya bila dapat dilakukan dengan
aman. Jangan menangani perangkat listrik berbahaya tanpa wewenang. Sebelum berbagi
laporan, hapus atau samarkan token serta data pribadi. Jangan memasukkan
kredensial ke repository. Pastikan direktori kerja dan path, simpan laporan
di lokasi dokumentasi yang disepakati, dan berikan akses hanya kepada pihak
yang memerlukannya.

## Latihan

1. Apa respons awal terhadap kabel yang membahayakan jalur berjalan? →
   **Amankan atau hindari area, atur kabel sesuai prosedur, dan laporkan bila
   diperlukan.**
2. File konfigurasi berisi token hendak di-commit. Apa tindakan tepat? →
   **Jangan commit token; gunakan mekanisme secret yang disetujui. Jika sudah
   terpapar, cabut/rotasi kredensial sesuai prosedur.**
3. Laporan bug memuat tangkapan layar dengan data pengguna. Apa yang perlu
   dilakukan sebelum dibagikan? → **Hapus atau samarkan data sensitif dan
   bagikan hanya kepada pihak yang berwenang.**
4. Sebuah aset tidak sengaja terhapus. Bagaimana memulihkannya dengan aman? →
   **Periksa lokasi dan perubahan, pulihkan dari backup atau version history,
   verifikasi hasil, lalu catat kejadian.**
5. Apa yang harus dipastikan sebelum memindahkan file dengan path relatif? →
   **Direktori kerja saat ini, tujuan path, hak akses, serta ketersediaan
   backup jika operasi berisiko.**
6. Sebuah proses hanya perlu membaca konfigurasi. Hak akses apa yang
   diberikan? → **Hak baca yang dibutuhkan saja (least privilege), bukan hak
   mengubah yang tidak diperlukan.**

## Checklist

- [ ] Mendahulukan keselamatan dan melaporkan bahaya sesuai prosedur.
- [ ] Menjaga kredensial, privasi pengguna, dan izin penggunaan aset.
- [ ] Menerapkan least privilege serta mengetahui peran backup dan version
  control.
- [ ] Memastikan direktori kerja dan path sebelum operasi file.
- [ ] Mempertimbangkan permission dan pemulihan aset sebelum mengubah file.
