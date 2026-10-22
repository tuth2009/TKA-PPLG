# Enkapsulasi dan Access Modifier (`P1`)

## Tujuan belajar

Menjelaskan bagaimana enkapsulasi melindungi state object dan memilih tingkat
akses yang sesuai untuk atribut maupun method.

## Prasyarat

- [Class dan object](01-class-dan-object.md)

## Materi

**Enkapsulasi** membatasi akses langsung ke state dan menyediakan method atau
antarmuka untuk menggunakannya dengan aturan yang terjaga. Tujuannya bukan
menyembunyikan semua informasi tanpa alasan, melainkan menjaga agar perubahan
state tetap valid.

Access modifier umumnya menyatakan siapa yang dapat mengakses anggota class:

| Modifier | Akses umum |
|---|---|
| `private` | Hanya dari dalam class yang mendefinisikan |
| `protected` | Dari class dan turunannya; aturan rinci bergantung bahasa |
| `public` | Dapat diakses dari luar melalui antarmuka class |

Detail modifier dapat berbeda antarbahasa pemrograman. Pilih akses sesuai
kebutuhan, bukan menjadikan semua anggota `public` secara otomatis. Jika nilai
harus memenuhi aturan tertentu, method dapat memvalidasi nilai sebelum
mengubah state.

## Contoh pseudocode

```text
class Payment:
    private amount

    method set_amount(value):
        if value >= 0:
            amount = value
```

`amount` tidak diubah sembarangan dari luar. Method `set_amount` menjaga
aturan bahwa nilainya tidak negatif.

## Latihan

1. Bagaimana menjaga `amount` tidak negatif? → **Enkapsulasi state dan
   validasi pada method yang mengubahnya.**
2. Modifier yang umumnya membatasi akses hanya di dalam class? → **`private`.**
3. Apakah semua atribut sebaiknya `public`? → **Tidak; pilih akses sesuai
   kebutuhan dan aturan yang harus dijaga.**

## Checklist

- [ ] Menjelaskan tujuan enkapsulasi.
- [ ] Membedakan akses umum `private`, `protected`, dan `public`.
- [ ] Memahami bahwa aturan akses spesifik dapat berbeda antarbahasa.
- [ ] Menentukan tempat validasi untuk melindungi state object.

Lanjutkan ke [Inheritance dan komposisi](03-inheritance-dan-komposisi.md).
