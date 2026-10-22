# Struktur Data Dasar (`P1`)

## Tujuan belajar

Memilih struktur data sederhana berdasarkan cara nilai akan disimpan dan
digunakan.

## Prasyarat

- [Tipe data dasar](01-tipe-data.md)

## Materi

Struktur data mengatur nilai agar operasi yang dibutuhkan dapat dilakukan
dengan jelas:

| Struktur | Kegunaan umum | Contoh |
|---|---|---|
| Array/list | Menyimpan urutan elemen | daftar nilai atau barang |
| Map/dictionary | Menghubungkan key dengan value | username ke alamat email |
| Set | Menyimpan elemen unik | kumpulan tag tanpa duplikasi |

Pilih struktur berdasarkan pola penggunaan. Gunakan list ketika urutan atau
akses berdasarkan posisi diperlukan. Gunakan map/dictionary untuk mencari
nilai berdasarkan key. Gunakan set ketika keunikan elemen perlu dijaga.

Jangan memilih struktur hanya karena sudah familiar. Pertimbangkan operasi
yang sering dilakukan dan pastikan setiap elemen memiliki arti yang jelas.

## Contoh

Data pasangan `username → email` lebih tepat disimpan sebagai map/dictionary
karena email dicari menggunakan username. Jika yang dibutuhkan hanya daftar
nama tanpa duplikasi, set dapat mewakili kebutuhan itu dengan lebih jelas.

## Latihan

1. Data username ke email paling tepat disimpan sebagai apa? →
   **Map/dictionary.**
2. Data item yang tidak boleh berulang? → **Set.**
3. Kapan list sesuai digunakan? → **Saat data berupa urutan elemen yang perlu
   diakses atau diproses berdasarkan urutannya.**

## Checklist

- [ ] Membedakan kegunaan array/list, map/dictionary, dan set.
- [ ] Memilih struktur data berdasarkan cara data akan digunakan.
- [ ] Mengenali kebutuhan key-value dan elemen unik.

Lanjutkan ke [Percabangan dan perulangan](03-percabangan-dan-perulangan.md).
