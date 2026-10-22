# Tipe Data, Struktur Data, dan Struktur Kontrol (`P1`)

## Target TKA

Menganalisis tipe/struktur data, alur percabangan/perulangan, dan efektivitas
kontrol pada potongan program atau skenario algoritmik.

## Required Knowledge

- [Peta prasyarat PPLG](00-peta-prasyarat.md).
- Operator aritmetika, perbandingan, logika, assignment.
- Membaca pseudocode dan tabel jejak (trace table).

## Inti materi

Pilih tipe sesuai domain: integer untuk hitungan bulat, floating untuk ukuran
desimal, boolean untuk kondisi, string untuk teks. Struktur data array/list
menyimpan urutan; map/dictionary menghubungkan key-value; set menyimpan elemen
unik. Analisis penggunaan bukan sekadar menghafal nama.

Percabangan `if/else` memilih jalur. Perulangan `for` cocok saat jumlah iterasi
diketahui; `while` saat berhenti berdasarkan kondisi. Pastikan kondisi berubah
agar tidak infinite loop. Telusuri nilai variabel baris demi baris.

## Contoh tracing

```text
total = 0
for n in [2, 4, 5]:
    if n % 2 == 0:
        total = total + n
```

Nilai total: 0 → 2 → 2 → 2+4 = **6**. Angka 5 tidak masuk karena ganjil.

## Jebakan umum

- Off-by-one pada batas loop.
- Mengubah kondisi pada variabel yang salah.
- Membandingkan string dan angka tanpa konversi/aturan bahasa.
- Memakai list saat lookup key-value yang lebih tepat memakai map.

## Latihan

1. `for i=1..3` menjumlahkan i → **6**.
2. Kondisi `while x>0` tetapi x tidak dikurangi → **loop tak berakhir**.
3. Data username→email paling tepat → **map/dictionary**.
4. Data item tanpa duplikasi → **set**.
5. `n%2==0` memeriksa → **bilangan genap**.

## Checklist

- [ ] Memilih tipe/struktur data sesuai kebutuhan.
- [ ] Membuat trace table untuk loop dan percabangan.
- [ ] Mengenali off-by-one dan infinite loop.
