# Tipe Data Dasar (`P1`)

## Tujuan belajar

Memilih tipe data yang sesuai dengan nilai dan operasi yang dibutuhkan program.

## Prasyarat

- [Dasar tipe data, struktur data, dan struktur kontrol](00-dasar-tipe-struktur-data-dan-kontrol.md)

## Materi

Tipe data menentukan jenis nilai yang disimpan dan operasi yang bermakna bagi
nilai tersebut:

| Tipe | Kegunaan umum | Contoh |
|---|---|---|
| Integer | Bilangan bulat | jumlah barang, indeks |
| Floating-point | Bilangan dengan bagian desimal | ukuran, hasil pengukuran |
| Boolean | Nilai benar atau salah | `is_valid`, `is_open` |
| String | Teks | nama, alamat, pesan |

Pilih tipe berdasarkan domain, bukan hanya bentuk sementara nilai. Misalnya,
jumlah barang biasanya berupa bilangan bulat, sedangkan hasil pengukuran dapat
memerlukan nilai desimal. Kondisi seperti apakah pengguna sudah masuk lebih
tepat direpresentasikan sebagai boolean daripada teks `"yes"` atau `"no"`.

Operator juga bergantung pada tipe dan aturan bahasa pemrograman. Berhati-hati
saat mencampur string dengan angka: konversi atau aturan bahasa yang tidak
sesuai dapat menghasilkan error atau perilaku yang tidak diharapkan.

## Contoh

Jika `jumlah = 3` lalu program menghitung `jumlah + 2`, hasilnya adalah
`5` untuk operasi bilangan. Jika input berasal dari teks, program mungkin
perlu mengubahnya menjadi tipe angka sebelum menghitung.

## Latihan

1. Tipe yang cocok untuk jumlah siswa? → **Integer.**
2. Tipe yang cocok untuk status pintu terbuka atau tertutup? → **Boolean.**
3. Mengapa teks angka perlu diperiksa sebelum dijumlahkan? → **Karena nilai
   string dan angka memiliki tipe serta aturan operasi yang berbeda.**

## Checklist

- [ ] Memilih integer, floating-point, boolean, atau string sesuai domain.
- [ ] Memahami bahwa tipe menentukan operasi yang sesuai.
- [ ] Mengenali perlunya konversi atau aturan eksplisit saat mencampur teks dan
  angka.

Lanjutkan ke [Struktur data dasar](02-struktur-data.md).
