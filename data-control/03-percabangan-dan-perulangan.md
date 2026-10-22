# Percabangan dan Perulangan (`P1`)

## Tujuan belajar

Menjelaskan bagaimana kondisi memilih jalur program dan bagaimana perulangan
menjalankan instruksi berulang kali.

## Prasyarat

- [Dasar tipe data, struktur data, dan struktur kontrol](00-dasar-tipe-struktur-data-dan-kontrol.md)
- [Tipe data dasar](01-tipe-data.md)

## Materi

Percabangan dan perulangan adalah struktur kontrol yang mengatur alur program.

- **`if/else`** memilih jalur berdasarkan hasil kondisi.
- **`for`** umumnya digunakan ketika jumlah iterasi atau elemen yang diproses
  diketahui.
- **`while`** digunakan ketika pengulangan berlanjut selama suatu kondisi
  masih terpenuhi.

Kondisi harus menggunakan nilai dan operator yang sesuai. Dalam perulangan,
periksa batas awal dan akhir, serta pastikan nilai atau keadaan yang
mempengaruhi kondisi berubah sehingga program dapat berhenti.

Contoh jebakan yang perlu diperiksa:

- **Off-by-one:** batas awal atau akhir loop membuat satu iterasi terlalu
  banyak atau terlalu sedikit.
- **Kondisi tidak berubah:** loop seperti `while x > 0` dapat berjalan tanpa
  akhir jika `x` tidak pernah dikurangi atau diubah.
- **Variabel yang salah diubah:** nilai yang berubah bukan nilai yang dipakai
  dalam kondisi loop.

## Contoh

```text
x = 3
while x > 0:
    tampilkan(x)
    x = x - 1
```

Nilai `x` berubah dari `3` ke `2`, `1`, lalu `0`. Ketika `x` menjadi `0`,
kondisi `x > 0` tidak lagi benar dan loop berhenti.

## Latihan

1. `for i=1..3` menjumlahkan semua nilai `i`. Hasilnya? → **6.**
2. `while x>0` tidak pernah mengubah `x`. Apa risikonya? → **Loop tidak
   berakhir jika kondisi awal benar.**
3. Apa yang perlu diperiksa saat hasil loop berbeda satu langkah? →
   **Batas awal/akhir dan jumlah iterasi (off-by-one).**

## Checklist

- [ ] Menjelaskan fungsi `if/else`, `for`, dan `while`.
- [ ] Memilih jenis perulangan berdasarkan kondisi masalah.
- [ ] Memeriksa batas iterasi dan perubahan kondisi agar loop dapat berhenti.

Lanjutkan ke [Tracing dan jebakan umum](04-tracing-dan-jebakan-umum.md).
