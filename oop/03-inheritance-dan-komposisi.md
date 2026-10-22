# Inheritance dan Komposisi (`P1`)

## Tujuan belajar

Menentukan kapan subclass mewarisi superclass dan kapan hubungan antarobject
lebih tepat dimodelkan dengan komposisi.

## Prasyarat

- [Class dan object](01-class-dan-object.md)
- [Enkapsulasi dan access modifier](02-enkapsulasi-dan-access-modifier.md)

## Materi

**Inheritance** membentuk hubungan antara superclass yang lebih umum dan
subclass yang lebih khusus. Subclass dapat mewarisi perilaku atau data yang
sesuai dari superclass, lalu menambahkan atau menyesuaikan perilakunya.

Gunakan inheritance bila hubungan konseptual **“is-a”** benar. Contohnya,
`QRPayment` adalah jenis `Payment`. Jangan menggunakan inheritance hanya agar
kode dapat dipakai ulang; relasi yang dipaksakan membuat desain membingungkan.

Jika suatu object **memiliki** atau **menggunakan** object lain, relasinya
adalah “has-a”. Dalam kasus tersebut, **komposisi** sering lebih sesuai:
class menyimpan atau menerima object lain untuk mendelegasikan tugas, tanpa
mengklaim bahwa class tersebut adalah jenis dari object itu.

## Contoh pseudocode

```text
class Payment:
    method pay(): return "generic"

class QRPayment extends Payment:
    method pay(): return "scan QR"
```

`QRPayment` dapat mewarisi `Payment` jika pembayaran QR memang merupakan jenis
pembayaran. Namun, sebuah `Receipt` yang memiliki `Payment` lebih tepat
digambarkan dengan komposisi daripada menjadikan `Receipt` subclass `Payment`.

## Latihan

1. `QRPayment is-a Payment`. Apakah inheritance masuk akal? →
   **Ya, jika relasi tersebut sesuai dengan domain aplikasi.**
2. Dua class hanya memiliki hubungan “has-a”. Apa yang dipertimbangkan? →
   **Komposisi, bukan inheritance.**
3. Apakah inheritance selalu pilihan terbaik untuk berbagi kode? →
   **Tidak; pilih berdasarkan hubungan dan tanggung jawab, bukan hanya reuse.**

## Checklist

- [ ] Menjelaskan peran superclass dan subclass.
- [ ] Menguji apakah hubungan “is-a” benar sebelum memakai inheritance.
- [ ] Mengenali hubungan “has-a” yang lebih tepat memakai komposisi.
- [ ] Menghindari inheritance yang hanya dipakai demi berbagi kode.

Lanjutkan ke [Polymorphism dan method overriding](04-polymorphism-dan-overriding.md).
