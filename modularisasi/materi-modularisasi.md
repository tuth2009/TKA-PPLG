# Fungsi, Prosedur, dan Modularisasi (`P1`)

## Target TKA

Menganalisis pembagian fungsi/prosedur serta mengevaluasi efektivitas desain
modular pada solusi perangkat lunak/gim.

## Required Knowledge

- [Tipe data dan kontrol](04-data-kontrol.md).
- Parameter, return value, scope, dan efek samping.
- Dekomposisi dan pengujian unit sederhana.

## Inti materi

Fungsi menerima input dan mengembalikan output; prosedur dapat berfokus pada
tindakan/efek samping. Modul yang baik punya satu tanggung jawab, antarmuka
jelas, dependensi kecil, nama bermakna, dan mudah diuji. Hindari fungsi raksasa,
variabel global yang tak terkendali, atau duplikasi logika.

## Contoh

```text
function total_price(items, tax_rate):
    subtotal = sum(item.price for item in items)
    return subtotal * (1 + tax_rate)
```

Fungsi ini dapat diuji dengan daftar kosong, satu item, dan tarif nol. Ia tidak
seharusnya sekaligus mengubah UI atau menulis database tanpa dinyatakan jelas.

## Latihan

1. Fungsi dengan dua tanggung jawab tak terkait → **pecah menjadi modul lebih kecil**.
2. Nilai yang harus dipakai pemanggil → **return**, bukan hanya print.
3. Variabel lokal → **tidak otomatis dapat diakses di luar fungsi**.
4. Duplikasi validasi di lima route → **buat modul validasi reusable**.
5. Desain modular efektif diukur dari → **kohesi, dependensi, keterujian, dan keterbacaan**.

## Checklist

- [ ] Menentukan input/output fungsi.
- [ ] Membedakan return value dan efek samping.
- [ ] Menilai kohesi, dependensi, dan keterujian modul.
