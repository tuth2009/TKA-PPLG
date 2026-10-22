# Pengelolaan Aset Proyek (`P1`)

## Tujuan belajar

Mengenali aset fisik dan digital dalam proyek, menatanya agar mudah ditemukan,
melacak perubahan, dan menjaga akses serta salinan data.

## Konsep inti

**Aset fisik** adalah perangkat yang digunakan untuk bekerja, seperti laptop,
monitor, router, dan media penyimpanan. **Aset digital** adalah berkas atau
hasil kerja proyek, seperti source code, konfigurasi, database, desain,
dokumentasi, audio/visual, dan hasil build.

| Jenis aset | Contoh | Hal yang perlu diperhatikan |
|---|---|---|
| Fisik | Laptop, monitor, router, media penyimpanan | Kondisi perangkat, lokasi, dan keselamatan penggunaan |
| Source | Kode sumber, skema data, skrip | Version control dan riwayat perubahan |
| Konfigurasi | Pengaturan aplikasi dan lingkungan | Hak akses dan perlindungan nilai sensitif |
| Konten | Gambar, audio, font, model 3D | Sumber, izin, dan lisensi |
| Dokumentasi | Kebutuhan, keputusan, panduan | Penamaan, lokasi, dan kemutakhiran |
| Hasil build | Berkas hasil kompilasi atau build | Pemisahan dari source serta kebijakan penyimpanan |

Kelola aset dengan struktur direktori dan penamaan yang konsisten. Version
control membantu melacak perubahan pada berkas yang sesuai, sementara backup
menyediakan salinan untuk pemulihan. Checksum atau riwayat dapat membantu
memeriksa integritas dan perubahan aset. Backup harus disimpan dan diuji sesuai
kebijakan proyek; keberadaan salinan saja belum memastikan pemulihan berhasil.

Terapkan **least privilege**: setiap pengguna atau proses hanya memperoleh
hak akses yang diperlukan. Jangan menyimpan secret seperti password API atau
token di repository. Gunakan mekanisme pengelolaan secret yang disetujui,
seperti secret manager atau environment variable; `.env.example` cukup memuat
nama variabel dan contoh nilai nonrahasia.

Pisahkan artefak build berukuran besar dari source code bila sesuai dengan
kebijakan proyek. Sebelum menghapus atau memindahkan aset, periksa path,
riwayat, hak akses, dan ketersediaan backup.

## Contoh struktur proyek

```text
project/
├─ src/          # source code
├─ tests/        # pengujian
├─ assets/       # gambar/audio dengan lisensi jelas
├─ docs/         # kebutuhan dan keputusan
├─ .env.example  # nama variabel saja, tanpa secret
└─ README.md
```

## Penerapan dan latihan

1. Password API ditemukan di kode. Pindahkan pengelolaannya ke mekanisme secret
   yang disetujui, cabut atau rotasi kredensial bila sudah terpapar, dan jangan
   melakukan commit secret.
2. Aset terhapus tidak sengaja. Pulihkan dari backup atau version history,
   verifikasi hasil pemulihan, lalu dokumentasikan kejadian.
3. Proses hanya perlu membaca berkas konfigurasi. Berikan hak baca yang
   diperlukan, bukan akses mengubah yang tidak dibutuhkan.
4. File build berukuran besar tidak diperlukan untuk mengembangkan source.
   Pisahkan dan kelola sesuai kebijakan penyimpanan proyek.
5. Aset gambar akan dimasukkan ke gim. Catat sumber dan pastikan izin atau
   lisensinya sesuai tujuan penggunaan.

## Checklist

- [ ] Dapat membedakan aset fisik, source, konfigurasi, konten, dokumentasi, dan hasil build.
- [ ] Struktur direktori dan penamaan konsisten.
- [ ] Perubahan dapat ditelusuri dan backup dapat dipulihkan.
- [ ] Akses menerapkan least privilege.
- [ ] Secret tidak disimpan di repository.
- [ ] Sumber dan izin konten proyek dapat diketahui.