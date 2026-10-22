# Desain dan Pengujian Modular (`P1`)

## Tujuan belajar

Mengevaluasi pembagian tanggung jawab, dependensi, dan keterujian suatu
desain modular, lalu merencanakan pengujian unit sederhana.

## Prasyarat

- [Parameter, return, scope, dan efek samping](02-parameter-return-scope-dan-efek-samping.md)
- Memahami dekomposisi masalah menjadi langkah yang dapat dikelola.

## Materi

Modul yang baik menangani tanggung jawab yang jelas. Modul sebaiknya memiliki
**kohesi** tinggi: bagian-bagian di dalamnya berkaitan erat dan mendukung
satu tujuan. Hubungan antar modul sebaiknya tidak lebih rumit dari yang
diperlukan; dependensi yang kecil dan antarmuka yang jelas memudahkan
perubahan serta pengujian.

Saat mengevaluasi desain, periksa:

- **Tanggung jawab:** apakah fungsi atau modul melakukan satu tugas yang
  saling berkaitan?
- **Antarmuka:** apakah input, output, dan tindakan mudah dipahami?
- **Dependensi:** apakah modul bergantung pada terlalu banyak bagian lain?
- **Duplikasi:** apakah logika yang sama disalin di banyak tempat?
- **Keterujian:** dapatkah perilaku diuji dengan input dan hasil yang jelas?
- **Keterbacaan:** apakah nama dan alur mudah dipahami?

Hindari fungsi raksasa yang menangani banyak tugas, variabel global yang tidak
terkendali, serta duplikasi logika. Jika validasi yang sama muncul di banyak
route, misalnya, pertimbangkan satu modul validasi yang dapat digunakan
bersama.

Pengujian unit sederhana memeriksa satu fungsi atau bagian kecil secara
terpisah. Pilih kasus normal dan kasus batas yang relevan. Untuk fungsi total
harga, contoh kasusnya meliputi daftar kosong, satu item, dan tarif pajak nol.
Jika fungsi memiliki efek samping, rencanakan bagaimana perubahan tersebut
diamati atau diuji.

## Contoh

Fungsi `total_price(items, tax_rate)` dapat diuji dengan memberi masukan dan
membandingkan nilai balik dengan hasil yang diharapkan. Karena fungsi tidak
sekaligus mengubah UI atau database, hasilnya lebih mudah diisolasi.

## Latihan

1. Fungsi memiliki dua tanggung jawab yang tidak terkait. Apa yang dapat
   dilakukan? → **Pecah menjadi fungsi atau modul lebih kecil dengan
   tanggung jawab yang jelas.**
2. Validasi yang sama disalin di lima route. Apa perbaikan yang dapat
   dipertimbangkan? → **Buat modul validasi reusable dengan antarmuka yang
   sesuai.**
3. Kasus apa yang dapat dipakai untuk menguji total harga? →
   **Daftar kosong, satu item, dan tarif nol, beserta hasil yang diharapkan.**
4. Bagaimana menilai efektivitas desain modular? → **Periksa kohesi,
   kejelasan dependensi dan antarmuka, keterujian, serta keterbacaan.**

## Checklist

- [ ] Memecah fungsi raksasa berdasarkan tanggung jawab.
- [ ] Menilai kohesi dan dependensi antar modul.
- [ ] Menghindari duplikasi logika dan global yang tidak terkendali.
- [ ] Menentukan input, hasil yang diharapkan, dan kasus uji unit sederhana.
- [ ] Mengevaluasi desain melalui keterbacaan dan kemudahan pengujian.
