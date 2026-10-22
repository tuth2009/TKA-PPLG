# Sistem Operasi, Berkas, dan Direktori (`P1`)

## Tujuan belajar

Memahami lokasi dan organisasi file serta menggunakan operasi dasar sistem
operasi untuk menemukan dan mengelola berkas proyek dengan aman.

## Konsep inti

Sistem operasi mengelola perangkat keras, menjalankan aplikasi, dan
menyediakan cara untuk mengakses file. Sistem berkas mengatur data dalam file
dan direktori.

- **Path absolut** menunjukkan lokasi dari titik awal sistem berkas.
- **Path relatif** menunjukkan lokasi berdasarkan direktori kerja saat ini.
- **File** menyimpan data; **folder/direktori** mengelompokkan file dan
  direktori lain.
- **Ekstensi** sering menunjukkan jenis file, tetapi tidak menjamin isi file
  sesuai ekstensi atau berasal dari sumber tepercaya.
- **Permission** menentukan tindakan yang diizinkan, misalnya membaca,
  mengubah, atau menjalankan file.

Contoh susunan direktori proyek:

```text
project/
├─ src/
├─ tests/
├─ assets/
├─ docs/
└─ README.md
```

Operasi dasar dapat dilakukan melalui antarmuka grafis atau terminal. Berikut
contoh konsep perintah; nama dan perilakunya dapat berbeda menurut sistem
operasi atau shell:

| Tujuan | Contoh |
|---|---|
| Melihat lokasi saat ini | `pwd` |
| Melihat isi direktori | `ls` atau `dir` |
| Membuat direktori | `mkdir` |
| Berpindah direktori | `cd` |
| Memeriksa perubahan repository | `git status` |

Pastikan direktori kerja dan path benar sebelum membuka atau mengubah berkas.
Path relatif hanya tepat jika dihitung dari direktori kerja yang sesuai.
Sebelum menghapus atau memindahkan aset, verifikasi path, periksa backup, dan
tinjau perubahan dengan `git status` jika proyek menggunakan Git. Jangan
menjalankan operasi yang tidak dipahami pada direktori yang belum dipastikan.

## Latihan

1. Pilih file di dalam proyek dan tulis path relatifnya dari direktori proyek.
2. Tentukan folder yang tepat untuk menyimpan kode sumber, pengujian, aset,
   dan dokumentasi.
3. Jelaskan perbedaan path absolut dan path relatif untuk file yang sama.
4. Sebelum memindahkan atau menghapus berkas, verifikasi lokasi, perubahan
   repository, dan ketersediaan backup.

## Checklist

- [ ] Dapat menjelaskan fungsi contoh perintah dasar.
- [ ] Dapat membedakan path absolut dan relatif.
- [ ] Memahami hubungan file, folder, ekstensi, dan permission.
- [ ] Dapat menjelaskan struktur direktori proyek sederhana.
- [ ] Memastikan lokasi dan path sebelum melakukan operasi berkas.
- [ ] Memeriksa backup sebelum menghapus atau memindahkan aset.