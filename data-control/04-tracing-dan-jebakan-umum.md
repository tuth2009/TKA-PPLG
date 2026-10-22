# Tracing dan Jebakan Umum (`P1`)

## Tujuan belajar

Menelusuri eksekusi pseudocode dan mengenali kesalahan umum pada tipe data,
struktur data, percabangan, dan perulangan.

## Prasyarat

- [Tipe data dasar](01-tipe-data.md)
- [Struktur data dasar](02-struktur-data.md)
- [Percabangan dan perulangan](03-percabangan-dan-perulangan.md)

## Materi

Tracing adalah mengikuti instruksi program satu per satu sambil mencatat nilai
variabel. Trace table membantu menunjukkan nilai sebelum dan sesudah suatu
langkah, kondisi yang diperiksa, dan apakah instruksi dijalankan.

Contoh:

```text
total = 0
for n in [2, 4, 5]:
    if n % 2 == 0:
        total = total + n
```

| `n` | `n % 2 == 0` | `total` sesudah iterasi |
|---:|:---:|---:|
| Awal | — | 0 |
| 2 | benar | 2 |
| 4 | benar | 6 |
| 5 | salah | 6 |

Jebakan umum yang perlu diperiksa:

- **Off-by-one** pada batas loop.
- Kondisi loop mengubah variabel yang salah atau tidak berubah.
- Membandingkan string dengan angka tanpa konversi atau aturan bahasa yang
  jelas.
- Memakai list untuk lookup key-value yang lebih tepat menggunakan
  map/dictionary.
- Mengasumsikan setiap elemen diproses tanpa menelusuri kondisi percabangan.

Saat hasil tidak sesuai dugaan, jangan hanya membaca baris terakhir. Telusuri
nilai awal, setiap kondisi, perubahan variabel, dan struktur data yang
digunakan.

## Contoh

Untuk mencari email berdasarkan username, list pasangan tanpa aturan
pencarian yang jelas dapat membuat lookup membingungkan. Map/dictionary lebih
sesuai karena username berperan sebagai key dan email sebagai value.

## Latihan

1. Pada contoh trace table, berapa nilai akhir `total`? → **6.**
2. `n % 2 == 0` memeriksa apa? → **Apakah `n` bilangan genap.**
3. Data username ke email disimpan paling tepat sebagai apa? →
   **Map/dictionary.**
4. Apa langkah awal saat hasil program tidak sesuai dugaan? →
   **Telusuri nilai awal, kondisi, dan perubahan variabel langkah demi
   langkah.**

## Checklist

- [ ] Membuat trace table untuk percabangan dan perulangan.
- [ ] Menelusuri nilai variabel pada setiap iterasi.
- [ ] Mengenali off-by-one dan risiko loop tak berakhir.
- [ ] Memeriksa kesesuaian tipe serta struktur data dengan operasi program.
