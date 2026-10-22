# Dasar Fungsi, Prosedur, dan Modularisasi (`P1`)

## Tujuan belajar

Memahami cara memecah solusi menjadi bagian-bagian yang memiliki tanggung
jawab jelas, serta peran fungsi dan prosedur dalam menyusun program.

## Prasyarat

- [Tracing dan jebakan umum](../data-control/04-tracing-dan-jebakan-umum.md)
- Memahami variabel, alur kontrol, dan cara menelusuri instruksi program.

## Materi

Saat masalah program membesar, menempatkan semua instruksi dalam satu bagian
membuat solusi sulit dibaca, diuji, dan diubah. **Dekomposisi** memecah
masalah menjadi tugas-tugas lebih kecil. Bagian program yang menangani tugas
tertentu dapat dirancang sebagai fungsi, prosedur, atau modul.

- **Fungsi** menerima input, mengolahnya, dan mengembalikan output melalui
  nilai balik (`return`).
- **Prosedur** berfokus pada tindakan. Prosedur dapat menghasilkan efek pada
  sistem atau lingkungan, dan tidak harus mengembalikan nilai untuk dipakai
  pemanggil.
- **Modul** mengelompokkan bagian program yang berkaitan agar tanggung
  jawabnya dapat dipahami dan digunakan.

Antarmuka yang jelas membantu pemanggil memahami informasi yang perlu
diberikan dan hasil atau tindakan yang dapat diharapkan. Variabel lokal
membatasi data pada bagian yang membutuhkannya. Perubahan pada keadaan di luar
fungsi/prosedur disebut **efek samping**; efek tersebut perlu dinyatakan dan
dikendalikan agar perilaku program mudah dipahami.

## Contoh

```text
function total_price(items, tax_rate):
    subtotal = sum(item.price for item in items)
    return subtotal * (1 + tax_rate)
```

Fungsi `total_price` menghitung dan mengembalikan total harga. Ia memiliki
input yang jelas dan dapat diuji tanpa sekaligus mengubah tampilan aplikasi
atau menulis ke database.

## Latihan

1. Apa tujuan dekomposisi? → **Memecah masalah menjadi tugas lebih kecil yang
   lebih mudah dikelola.**
2. Jika pemanggil memerlukan hasil perhitungan, apa yang digunakan? →
   **Nilai balik (`return`).**
3. Apa yang dimaksud efek samping? → **Perubahan atau tindakan yang
   memengaruhi keadaan di luar nilai balik fungsi.**

## Checklist

- [ ] Menjelaskan fungsi dekomposisi dan modularisasi.
- [ ] Membedakan fungsi yang mengembalikan nilai dari prosedur yang berfokus
  pada tindakan.
- [ ] Mengenali input, output, dan kemungkinan efek samping.

Lanjutkan ke [Fungsi dan prosedur](01-fungsi-dan-prosedur.md).
