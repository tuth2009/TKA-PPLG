# Dasar Tipe Data, Struktur Data, dan Struktur Kontrol (`P1`)

## Tujuan belajar

Memahami bagaimana program merepresentasikan data, menyimpan kumpulan nilai,
dan mengatur urutan instruksi untuk menyelesaikan masalah.

## Prasyarat

- [Peta prasyarat PPLG](../00-peta-prasyarat.md)
- Memahami bahwa program menjalankan instruksi secara berurutan.

## Materi

Program menerima, menyimpan, dan mengolah data. **Tipe data** menjelaskan
jenis nilai dan operasi yang sesuai. **Struktur data** mengatur kumpulan nilai
agar dapat digunakan dengan tepat. **Struktur kontrol** menentukan instruksi
mana yang berjalan dan berapa kali.

Saat menganalisis program, ikuti alur berikut:

1. Kenali data masukan dan tujuan pengolahan.
2. Tentukan tipe serta struktur data yang sesuai.
3. Ikuti kondisi dan pengulangan yang mengatur alur.
4. Telusuri perubahan nilai variabel langkah demi langkah.
5. Cocokkan hasil akhir dengan tujuan program.

Gunakan tabel jejak (trace table) untuk mencatat nilai variabel setelah
instruksi penting. Cara ini membantu menemukan kesalahan batas perulangan,
kondisi yang tidak pernah berubah, atau nilai yang diproses dengan tipe yang
tidak sesuai.

## Contoh

```text
total = 0
for n in [2, 4, 5]:
    if n % 2 == 0:
        total = total + n
```

`total` dimulai dari `0`. Nilai `2` dan `4` memenuhi kondisi genap, sedangkan
`5` tidak. Jejak nilai `total`: `0 → 2 → 6`; hasil akhirnya **6**.

## Latihan

1. Apa fungsi tipe data? → **Menjelaskan jenis nilai dan operasi yang sesuai.**
2. Apa yang ditentukan struktur kontrol? → **Instruksi yang dijalankan dan
   kapan atau berapa kali instruksi dijalankan.**
3. Untuk apa tabel jejak digunakan? → **Mencatat perubahan nilai dan alur
   program langkah demi langkah.**

## Checklist

- [ ] Menjelaskan hubungan tipe data, struktur data, dan struktur kontrol.
- [ ] Menelusuri perubahan nilai variabel berdasarkan urutan instruksi.
- [ ] Menggunakan trace table untuk memeriksa hasil program.

Lanjutkan ke [Tipe data dasar](01-tipe-data.md).
