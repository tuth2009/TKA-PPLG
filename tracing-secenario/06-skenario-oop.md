# Skenario Object-Oriented Programming (`P1`)

## Tujuan belajar

Menelusuri state dan perilaku object, memilih enkapsulasi serta relasi class,
dan menentukan method yang berjalan melalui polymorphism.

## Prasyarat

- [Dasar Object-Oriented Programming](../oop/00-dasar-oop.md)
- [Class dan object](../oop/01-class-dan-object.md)
- [Enkapsulasi dan access modifier](../oop/02-enkapsulasi-dan-access-modifier.md)
- [Inheritance dan komposisi](../oop/03-inheritance-dan-komposisi.md)
- [Polymorphism dan method overriding](../oop/04-polymorphism-dan-overriding.md)

## Skenario: jenis pembayaran

```text
class Payment:
    private amount
    method pay(): return "generic"

class QRPayment extends Payment:
    method pay(): return "scan QR"

Payment p = new QRPayment()
p.pay()
```

`Payment` adalah class, sedangkan `p` adalah referensi ke object `QRPayment`.
`amount` dilindungi agar tidak dapat diubah sembarangan; method yang mengubah
nilainya perlu menjaga aturan seperti nilai tidak negatif. Karena
`QRPayment` adalah jenis `Payment`, inheritance sesuai. Jika `pay` dioverride,
pemanggilan melalui `p` menjalankan implementasi object `QRPayment` pada model
polymorphism runtime ini.

## Latihan

1. Cetak biru object adalah apa? → **Class.**
2. Bagaimana menjaga `amount` tetap valid? → **Lindungi state dengan
   enkapsulasi dan validasi pada method yang mengubahnya.**
3. Apa tipe referensi `p` dan tipe object sebenarnya? → **Referensi
   `Payment`, object `QRPayment`.**
4. Jika `QRPayment.pay` meng-override `Payment.pay`, implementasi mana yang
   dipanggil? → **`QRPayment.pay`.**
5. `Receipt` menyimpan sebuah `Payment`. Apakah `Receipt` harus menjadi
   subclass `Payment`? → **Tidak; relasinya “has-a”, jadi komposisi lebih
   sesuai.**
6. Modifier apa yang umumnya membatasi atribut ke class itu sendiri? →
   **`private` (dengan rincian yang dapat berbeda menurut bahasa).**

## Checklist

- [ ] Membedakan class, object, state, dan method.
- [ ] Menjaga state melalui enkapsulasi serta access modifier.
- [ ] Memastikan hubungan “is-a” sebelum memakai inheritance.
- [ ] Memilih komposisi untuk hubungan “has-a”.
- [ ] Menelusuri overriding melalui referensi superclass.
