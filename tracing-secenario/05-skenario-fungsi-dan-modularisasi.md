# Skenario Fungsi dan Modularisasi (`P1`)

## Tujuan belajar

Menganalisis tanggung jawab fungsi, aliran nilai, scope, efek samping, dan
keterujian desain modular.

## Prasyarat

- [Dasar fungsi, prosedur, dan modularisasi](../modularisasi/00-dasar-fungsi-prosedur-dan-modularisasi.md)
- [Fungsi dan prosedur](../modularisasi/01-fungsi-dan-prosedur.md)
- [Parameter, return, scope, dan efek samping](../modularisasi/02-parameter-return-scope-dan-efek-samping.md)
- [Desain dan pengujian modular](../modularisasi/03-desain-dan-pengujian-modular.md)

## Skenario: fungsi pemrosesan pesanan

Fungsi `processOrder` membaca input, memvalidasi data, menghitung pajak,
menulis database, mengirim email, dan memperbarui tampilan. Hasilnya sulit
diuji karena satu pemanggilan mengerjakan banyak hal dan menimbulkan beberapa
efek samping.

Pertimbangkan memecah alur menjadi validasi, perhitungan total, penyimpanan,
dan pemberitahuan. Fungsi perhitungan dapat menerima input melalui parameter
dan mengembalikan hasil dengan `return`; penyimpanan atau pengiriman email
dapat menjadi tindakan terpisah dengan efek samping yang jelas. Desain tidak
harus memecah setiap baris menjadi fungsi kecil—batas modul sebaiknya
mencerminkan tanggung jawab yang bermakna.

## Latihan

1. Pemanggil perlu memakai hasil hitung pajak. Apakah hasil cukup di-`print`?
   → **Tidak; kembalikan nilai dengan `return`.**
2. Variabel yang dideklarasikan lokal dalam fungsi otomatis dapat digunakan
   di luar fungsi? → **Tidak; scope-nya terbatas menurut aturan bahasa.**
3. `processOrder` menjalankan banyak tanggung jawab. Apa yang dapat
   diperbaiki? → **Pisahkan tugas yang berbeda dengan antarmuka dan
   dependensi yang jelas.**
4. Validasi yang sama disalin di beberapa route. Apa desain yang dapat
   dipertimbangkan? → **Modul validasi reusable yang menerima input jelas dan
   mengembalikan hasil validasi.**
5. Kasus apa untuk menguji fungsi total harga? → **Daftar kosong, satu item,
   dan tarif pajak nol, dengan nilai hasil yang diharapkan.**
6. Apa yang diperiksa untuk menilai desain modular? → **Kohesi tanggung
   jawab, kejelasan antarmuka, kecilnya dependensi, minimnya duplikasi,
   keterbacaan, dan keterujian.**

## Checklist

- [ ] Menentukan parameter dan hasil yang harus dikembalikan.
- [ ] Membedakan return value dengan print dan efek samping.
- [ ] Mengenali batas scope variabel lokal.
- [ ] Memecah tanggung jawab tanpa membuat abstraksi yang tidak diperlukan.
- [ ] Menyusun kasus uji unit termasuk kasus batas.
