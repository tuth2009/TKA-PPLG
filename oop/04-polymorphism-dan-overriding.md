# Polymorphism dan Method Overriding (`P1`)

## Tujuan belajar

Menelusuri bagaimana pemanggilan method melalui referensi superclass dapat
menghasilkan perilaku subclass yang sesuai dengan object sebenarnya.

## Prasyarat

- [Inheritance dan komposisi](03-inheritance-dan-komposisi.md)

## Materi

**Polymorphism** memungkinkan kode menggunakan antarmuka atau referensi
superclass sementara object sebenarnya merupakan instance subclass. Dengan
demikian, pemanggil dapat bekerja melalui kontrak umum tanpa harus memilih
perilaku tiap subclass secara manual.

**Method overriding** terjadi ketika subclass menyediakan implementasi
sendiri untuk method yang diwarisi. Pada polymorphism dinamis, implementasi
yang dijalankan ditentukan oleh tipe object sebenarnya saat runtime, sesuai
dengan aturan bahasa.

Untuk menganalisis potongan program:

1. Identifikasi tipe referensi.
2. Identifikasi class object yang dibuat.
3. Periksa apakah subclass meng-override method.
4. Tentukan implementasi yang dipanggil berdasarkan object dan aturan bahasa.

## Contoh pseudocode

```text
class Payment:
    method pay(): return "generic"

class QRPayment extends Payment:
    method pay(): return "scan QR"

Payment p = new QRPayment()
p.pay()
```

Referensi `p` bertipe `Payment`, tetapi object sebenarnya adalah
`QRPayment`. Karena method `pay` di-override, pemanggilan menghasilkan
`"scan QR"` pada model polymorphism runtime yang ditunjukkan pseudocode ini.

## Latihan

1. `Payment p = new QRPayment(); p.pay()` memanggil implementasi mana jika
   `QRPayment` meng-override `pay`? → **Implementasi `QRPayment.pay`.**
2. Dalam contoh, apa tipe referensi dan tipe object sebenarnya? →
   **Referensi `Payment`; object `QRPayment`.**
3. Apa manfaat polymorphism? → **Kode dapat menggunakan antarmuka umum dan
   membiarkan object yang sesuai menyediakan perilaku spesifik.**

## Checklist

- [ ] Membedakan tipe referensi dengan tipe object sebenarnya.
- [ ] Menjelaskan method overriding.
- [ ] Menelusuri implementasi method yang dipilih saat runtime.
- [ ] Menghubungkan polymorphism dengan antarmuka superclass.
