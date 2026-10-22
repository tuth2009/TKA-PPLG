# Class dan Object (`P1`)

## Tujuan belajar

Membedakan definisi class dari object yang dibuat berdasarkan definisi
tersebut, serta mengenali state dan perilaku object.

## Prasyarat

- [Dasar Object-Oriented Programming](00-dasar-oop.md)

## Materi

**Class** mendeskripsikan data dan perilaku yang dimiliki suatu jenis object.
Definisi class belum dengan sendirinya menjadi object yang sedang digunakan.
**Object** adalah instance class yang memiliki state sendiri dan dapat
menjalankan method yang didefinisikan class.

- **Atribut** menyimpan data atau state.
- **Method** adalah operasi/perilaku yang terkait dengan class atau object.
- **Instansiasi** adalah proses membuat object dari class.

Contohnya, `Payment` dapat menjadi class, sedangkan pembayaran tertentu yang
dibuat dari class itu adalah object. Beberapa object dapat berasal dari class
yang sama, tetapi masing-masing merepresentasikan instance dan state
tersendiri.

## Contoh pseudocode

```text
class Lamp:
    state = "off"
    method turn_on():
        state = "on"

lampu_kamar = new Lamp()
lampu_meja = new Lamp()
```

`Lamp` adalah class. `lampu_kamar` dan `lampu_meja` adalah dua object hasil
instansiasi class tersebut.

## Latihan

1. Cetak biru object disebut apa? → **Class.**
2. Apa yang dimaksud instansiasi? → **Membuat object dari class.**
3. Dalam contoh, manakah object? → **`lampu_kamar` dan `lampu_meja`.**

## Checklist

- [ ] Membedakan definisi class dengan instance object.
- [ ] Mengenali atribut sebagai state dan method sebagai perilaku.
- [ ] Menjelaskan bahwa beberapa object dapat dibuat dari satu class.

Lanjutkan ke [Enkapsulasi dan access modifier](02-enkapsulasi-dan-access-modifier.md).
