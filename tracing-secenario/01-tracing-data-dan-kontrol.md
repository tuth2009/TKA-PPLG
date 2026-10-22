# Tracing Data dan Struktur Kontrol (`P1`)

## Tujuan belajar

Menelusuri perubahan nilai program, memilih struktur data, dan menemukan
kesalahan pada percabangan maupun perulangan.

## Prasyarat

- [Dasar tipe data, struktur data, dan struktur kontrol](../data-control/00-dasar-tipe-struktur-data-dan-kontrol.md)
- [Tipe data dasar](../data-control/01-tipe-data.md)
- [Struktur data dasar](../data-control/02-struktur-data.md)
- [Percabangan dan perulangan](../data-control/03-percabangan-dan-perulangan.md)
- [Tracing dan jebakan umum](../data-control/04-tracing-dan-jebakan-umum.md)

## Skenario: menghitung skor

```text
score = 0
for x in [3, 8, 10, 11]:
    if x >= 10:
        score = score + 2
    else:
        score = score + 1
```

Trace setiap iterasi:

| `x` | Kondisi `x >= 10` | Perubahan skor | Skor akhir iterasi |
|---:|:---:|---:|---:|
| awal | — | — | 0 |
| 3 | salah | `+1` | 1 |
| 8 | salah | `+1` | 2 |
| 10 | benar | `+2` | 4 |
| 11 | benar | `+2` | 6 |

Hasil akhirnya **6**. Menulis perubahan per iterasi mencegah kesalahan saat
menebak hasil hanya dari jumlah elemen.

## Latihan

1. `for i = 1..3` menambahkan `i` ke `total` yang dimulai dari 0. Berapa hasil
   akhirnya? → **6.**
2. `while x > 0` tidak pernah mengubah `x`, dan `x` dimulai dari 2. Apa
   risikonya? → **Kondisi terus benar sehingga terjadi loop tak berakhir.**
3. Program menyimpan pasangan `username → email`. Struktur apa yang paling
   sesuai untuk pencarian berdasarkan username? → **Map/dictionary.**
4. Program mengumpulkan tag dan harus mencegah duplikasi. Struktur apa yang
   sesuai? → **Set.**
5. Apa yang diperiksa jika hasil loop berbeda satu iterasi dari dugaan? →
   **Batas awal/akhir (off-by-one), kondisi, dan nilai yang diperbarui.**
6. Input `"12"` bertipe string dibandingkan dengan angka `12`. Apa yang
   perlu diperiksa? → **Tipe input dan aturan/conversion bahasa; konversi
   secara eksplisit bila operasi angka yang dimaksud.**

## Checklist

- [ ] Menyusun trace table untuk nilai dan kondisi di setiap iterasi.
- [ ] Memilih list, map/dictionary, atau set sesuai pola penggunaan.
- [ ] Mengenali off-by-one, variabel kondisi yang salah, dan loop tak berakhir.
- [ ] Memeriksa tipe nilai dan operator yang digunakan dalam kondisi.
