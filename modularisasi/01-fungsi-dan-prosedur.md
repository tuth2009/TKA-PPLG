# Fungsi dan Prosedur (`P1`)

## Tujuan belajar

Membedakan fungsi dan prosedur serta merancang bagian program dengan input,
hasil, atau tindakan yang jelas.

## Prasyarat

- [Dasar fungsi, prosedur, dan modularisasi](00-dasar-fungsi-prosedur-dan-modularisasi.md)

## Materi

Fungsi digunakan saat suatu tugas menghasilkan nilai yang akan dipakai oleh
pemanggil. Nilai masukan diberikan melalui parameter, lalu hasil dikirim
kembali dengan `return`.

```text
function luas_persegi_panjang(panjang, lebar):
    return panjang * lebar
```

Pemanggil dapat menyimpan atau mengolah hasilnya:

```text
luas = luas_persegi_panjang(5, 3)
```

Prosedur lebih menekankan tindakan, misalnya menampilkan pesan atau
menyimpan perubahan. Jika suatu prosedur mengubah keadaan di luar dirinya,
perubahan itu merupakan efek samping dan sebaiknya terlihat jelas dari
tanggung jawab serta antarmukanya.

Jangan mengganti nilai balik dengan mencetak hasil jika pemanggil perlu
menggunakan hasil tersebut untuk perhitungan lain. `print` menampilkan
informasi, sedangkan `return` menyerahkan nilai ke pemanggil.

## Contoh

Fungsi menghitung total harga sebaiknya mengembalikan angka. Prosedur yang
menampilkan ringkasan transaksi dapat menangani tampilan. Memisahkan kedua
tugas tersebut membuat hasil hitung dapat digunakan ulang tanpa harus
menampilkan antarmuka.

## Latihan

1. Pemanggil perlu memakai hasil hitung untuk perhitungan berikutnya. Apa
   pilihan yang tepat? → **Fungsi yang mengembalikan hasil dengan `return`.**
2. Apa perbedaan `return` dengan `print`? → **`return` memberikan nilai ke
   pemanggil; `print` menampilkan informasi.**
3. Fungsi sekaligus menghitung harga dan mengirim email. Apa masalah
   desainnya? → **Dua tanggung jawab berbeda digabung; pertimbangkan
   memisahkannya.**

## Checklist

- [ ] Menentukan kapan nilai balik diperlukan.
- [ ] Membedakan nilai balik dengan keluaran yang hanya ditampilkan.
- [ ] Memisahkan perhitungan dari tindakan lain yang tidak terkait.

Lanjutkan ke [Parameter, return, scope, dan efek samping](02-parameter-return-scope-dan-efek-samping.md).
