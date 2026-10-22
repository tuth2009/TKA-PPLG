# HTTP dan API (`P1`)

## Tujuan belajar

Mengenali bagian permintaan HTTP, memahami kelompok status respons, dan
menjelaskan batas aman antara client dengan database.

## Prasyarat

- [Client-server dan DNS](01-client-server-dan-dns.md)
- Pemahaman dasar tentang data terstruktur seperti JSON.

## Materi

HTTP adalah protokol aplikasi untuk komunikasi client-server. Sebuah HTTP
request umumnya memuat:

- **Method**, yang menyatakan jenis operasi yang diminta.
- **URL**, yang menunjukkan alamat resource.
- **Header**, yang membawa metadata permintaan.
- **Body**, yang dapat membawa data; format JSON umum digunakan untuk
  pertukaran data API.

Server mengirim HTTP response dengan status yang memberi gambaran hasil
permintaan:

| Kelompok status | Arti umum |
|---|---|
| `2xx` | Permintaan berhasil |
| `3xx` | Pengalihan |
| `4xx` | Masalah pada permintaan atau otorisasi client |
| `5xx` | Masalah saat server menangani permintaan |

Perhatikan status tertentu:

- `401` menunjukkan autentikasi yang valid diperlukan.
- `403` menunjukkan akses tidak diizinkan.
- `404` menunjukkan resource atau route tidak ditemukan.
- `500` menunjukkan masalah pada server.

API menjadi perantara akses data dan fungsi aplikasi. Jangan membuka database
atau menaruh kredensial database di client. Gunakan server/API untuk
memvalidasi permintaan dan mengendalikan akses.

## Contoh

Respons `404` dapat berarti jaringan dan server berfungsi, tetapi route atau
resource yang diminta tidak ditemukan. Respons `500` mengarahkan pemeriksaan ke
log server dan input yang diproses; itu bukan otomatis kesalahan browser.

## Latihan

1. HTTP `401` menandakan apa? → **Autentikasi yang valid diperlukan.**
2. Apa arti umum `404`? → **Resource atau route tidak ditemukan.**
3. Mengapa kredensial database tidak boleh diberikan ke client? →
   **Agar akses database dikendalikan melalui server/API dan validasi.**

## Checklist

- [ ] Menyebutkan method, URL, header, dan body pada request.
- [ ] Membedakan kelompok status `2xx`, `3xx`, `4xx`, dan `5xx`.
- [ ] Membedakan makna status `401`, `403`, `404`, dan `500`.
- [ ] Menjelaskan peran server/API dalam melindungi akses database.

Lanjutkan ke [Diagnosis konektivitas](03-diagnosis-konektivitas.md).
