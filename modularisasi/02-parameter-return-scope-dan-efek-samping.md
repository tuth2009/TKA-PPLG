# Parameter, Return, Scope, dan Efek Samping (`P1`)

## Tujuan belajar

Menelusuri aliran data ke dan dari fungsi serta memahami jangkauan variabel
dan dampak perubahan keadaan.

## Prasyarat

- [Fungsi dan prosedur](01-fungsi-dan-prosedur.md)

## Materi

**Parameter** adalah nama input yang didefinisikan oleh fungsi/prosedur.
**Argumen** adalah nilai yang diberikan ketika fungsi/prosedur dipanggil.
Parameter yang jelas membuat kebutuhan bagian program terlihat pada
antarmukanya.

**Return value** adalah nilai yang dikirim kembali kepada pemanggil. Jika
suatu hasil dibutuhkan oleh bagian lain, kembalikan nilai tersebut alih-alih
hanya menampilkannya.

**Scope** adalah jangkauan tempat suatu nama atau variabel dapat diakses.
Variabel lokal yang dibuat di dalam fungsi umumnya hanya dapat digunakan di
fungsi tersebut. Karena itu, variabel lokal tidak otomatis dapat dibaca dari
luar. Aturan rinci dapat berbeda antarbahasa, tetapi mengandalkan variabel
global tanpa kebutuhan yang jelas membuat hubungan antarbagian lebih sulit
ditelusuri.

**Efek samping** adalah perubahan di luar nilai balik, misalnya mengubah
variabel global, menulis file, memperbarui database, atau mengubah tampilan.
Efek samping dapat dibutuhkan, tetapi perlu dinyatakan dengan jelas agar
pemanggil memahami konsekuensi pemanggilan fungsi/prosedur.

## Contoh

```text
function tambah_pajak(subtotal, tarif):
    total = subtotal * (1 + tarif)
    return total
```

`subtotal` dan `tarif` adalah parameter. `total` adalah variabel lokal dan
hasilnya dikirim melalui `return`. Fungsi ini tidak mengubah data lain.

## Latihan

1. Apakah variabel lokal otomatis dapat diakses di luar fungsi? →
   **Tidak; aksesnya dibatasi oleh scope sesuai aturan bahasa.**
2. Apa manfaat parameter yang jelas? → **Menunjukkan input yang dibutuhkan
   oleh fungsi/prosedur.**
3. Fungsi mengubah variabel global tanpa memberi tahu pemanggil. Apa yang
   perlu diperhatikan? → **Perubahan itu merupakan efek samping yang
   menyulitkan pemahaman dan pengujian; nyatakan atau rancang ulang dengan
   antarmuka yang jelas.**

## Checklist

- [ ] Membedakan parameter dan argumen.
- [ ] Menelusuri nilai yang masuk dan return value yang keluar.
- [ ] Memahami bahwa variabel lokal memiliki scope terbatas.
- [ ] Mengenali dan menjelaskan efek samping.

Lanjutkan ke [Desain dan pengujian modular](03-desain-dan-pengujian-modular.md).
