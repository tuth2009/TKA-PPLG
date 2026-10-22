# Dasar Object-Oriented Programming (`P1`)

## Tujuan belajar

Memahami bagaimana OOP mengelompokkan state dan perilaku dalam class dan
object, serta bagaimana enkapsulasi, inheritance, dan polymorphism mendukung
desain program.

## Prasyarat

- [Tipe data dan struktur kontrol](../data-control/00-dasar-tipe-struktur-data-dan-kontrol.md)
- [Dasar fungsi, prosedur, dan modularisasi](../modularisasi/00-dasar-fungsi-prosedur-dan-modularisasi.md)

## Materi

Object-Oriented Programming (OOP) adalah cara menyusun program dengan
menggunakan object yang menggabungkan data dan perilaku:

- **Class** mendefinisikan bentuk atau cetak biru object.
- **Object** adalah instance yang dibuat dari class.
- **Atribut/state** menyimpan keadaan atau data object.
- **Method/perilaku** mendefinisikan tindakan yang dapat dilakukan object.

Dalam merancang class, tentukan data apa yang menjadi tanggung jawab object
dan perilaku apa yang berkaitan dengan data tersebut. Access modifier dan
enkapsulasi membantu mengendalikan bagaimana state digunakan. Inheritance
dapat membentuk relasi antara class umum dan class khusus; polymorphism
memungkinkan perilaku yang sesuai dengan jenis object dijalankan melalui
antarmuka bersama.

Gunakan fitur OOP untuk memperjelas tanggung jawab, bukan sekadar menambah
lapisan. Inheritance tepat ketika relasi “is-a” benar; jika satu object hanya
memiliki atau menggunakan object lain (“has-a”), komposisi sering lebih tepat.

## Contoh

Class `Payment` dapat mendefinisikan state pembayaran dan method `pay`.
Object `QRPayment` dapat mewakili pembayaran QR. Jika `QRPayment` memang jenis
pembayaran, class itu dapat mewarisi `Payment` dan menyediakan implementasi
`pay` yang sesuai.

## Latihan

1. Apa yang disebut cetak biru object? → **Class.**
2. Apa yang disebut instance dari class? → **Object.**
3. Kapan inheritance masuk akal? → **Saat relasi subclass terhadap
   superclass benar-benar “is-a”.**
4. Apa alternatif saat relasinya “has-a”? → **Pertimbangkan komposisi.**

## Checklist

- [ ] Membedakan class dan object.
- [ ] Menjelaskan hubungan atribut/state dan method/perilaku.
- [ ] Menyebutkan tujuan enkapsulasi, inheritance, dan polymorphism.
- [ ] Mempertimbangkan komposisi untuk relasi “has-a”.

Lanjutkan ke [Class, object, atribut, dan method](01-class-dan-object.md).
