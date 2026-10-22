# OOP: Class, Enkapsulasi, Inheritance, Polymorphism (`P1`)

## Target TKA

Menerapkan class/object, access modifier, enkapsulasi, inheritance, serta
polymorphism melalui overriding atau referensi superclass.

## Required Knowledge

- [Tipe data dan kontrol](04-data-kontrol.md).
- [Modularisasi](05-modularisasi.md).
- Perbedaan definisi dan instansiasi, method, serta state.

## Inti materi

Class mendefinisikan atribut/state dan method/perilaku; object adalah instance.
Enkapsulasi menyembunyikan state dan memberi akses melalui method yang menjaga
aturan. `private` biasanya hanya diakses class sendiri, `protected` class dan
turunannya (tergantung bahasa), `public` dari luar. Pilih access modifier
berdasarkan kebutuhan, bukan selalu public.

Inheritance menyatakan subclass mewarisi perilaku/data superclass bila relasi
“is-a” memang benar. Polymorphism memungkinkan referensi superclass menunjuk
object subclass; method overriding dipilih berdasarkan tipe object saat runtime.
Jangan memakai inheritance hanya untuk berbagi kode jika komposisi lebih tepat.

## Contoh pseudocode

```text
class Payment:
    private amount
    method pay(): return "generic"

class QRPayment extends Payment:
    method pay(): return "scan QR"

Payment p = new QRPayment()
p.pay()  # "scan QR" (overriding/polymorphism)
```

`amount` tidak boleh diubah sembarangan dari luar; setter dapat memvalidasi
amount tidak negatif.

## Latihan

1. Cetak biru objek → **class**.
2. Menjaga amount tidak negatif → **enkapsulasi + validasi setter/method**.
3. Subclass “QRPayment is-a Payment” → **inheritance masuk akal**.
4. `Payment p=new QRPayment(); p.pay()` → **method QRPayment dipanggil jika override**.
5. Dua class hanya “has-a” bukan “is-a” → **pertimbangkan composition**.

## Checklist

- [ ] Menjelaskan class, object, atribut, dan method.
- [ ] Memilih access modifier dan enkapsulasi.
- [ ] Menelusuri inheritance, overriding, dan polymorphism.
