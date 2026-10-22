# PPLG — Pengembangan Perangkat Lunak dan Gim

Repositori ini berisi bahan belajar Markdown untuk persiapan TKA PPLG:
peta prasyarat, materi per topik, latihan tracing lintas topik, dan instruksi
opsional untuk memakai AI sebagai tutor. File `materi-*.md` menjadi sumber
ringkas per rumpun; file bernomor `00-`, `01-`, dan seterusnya memecahnya
menjadi urutan belajar yang lebih terarah.

## Cakupan resmi

Pusmendik mendefinisikan TKA PPLG sebagai pengukuran konsep, penalaran, dan
penerapan pengetahuan dasar kejuruan dalam pengembangan perangkat lunak/gim.
Muatan dirujukkan ke materi esensial CP PPLG Fase E (Salinan Keputusan Kepala
BSKAP Nomor 046/H/KR/2025). Daftar matriks rinci dan URL resmi ada di
[sources-pusmendik.md](sources-pusmendik.md).

## Cara menggunakan project

1. Mulai dari [peta prasyarat](00-peta-prasyarat.md) untuk memahami hubungan
   antartopik.
2. Pelajari materi sesuai urutan modul di bawah. Gunakan file `materi-*.md`
   sebagai ringkasan rumpun atau indeks jika ingin melihat cakupan utuh.
3. Setelah memahami konsep, kerjakan modul
   [tracing dan latihan skenario](tracing-secenario/materi-tracing-skenario.md)
   untuk menerapkannya pada kasus per topik dan latihan integratif.
4. Jika menggunakan AI sebagai tutor, salin
   [instruksi AI tutor PPLG](INSTRUKSI-AI-TUTOR.md) ke fitur instruksi AI yang
   digunakan. Instruksi itu mengarahkan perilaku tutor; sumber belajar tetap
   dokumen materi di project ini.

## Peta Required Knowledge

```text
Wawasan kerja + etika + K3LH
├─ pengelolaan OS, file, aset, dokumentasi
├─ jaringan dasar → TCP/IP → HTTP/API/client-server
└─ berpikir komputasional
   ├─ tipe/struktur data → kontrol → fungsi/prosedur → modularisasi
   └─ class/object → enkapsulasi → inheritance → polymorphism
```

## Urutan modul

1. [Peta prasyarat dan cara membaca kode](00-peta-prasyarat.md)
2. Dunia kerja, proses bisnis, proyek, dan mutu:
   - Sumber materi: [Dunia kerja, proses bisnis, proyek, dan mutu](dunia-kerja-proyek-mutu/materi-dunia-kerja-proyek-mutu.md)
      - [Dasar dunia kerja, proyek, dan mutu PPLG](dunia-kerja-proyek-mutu/00-dasar-dunia-kerja-proyek-mutu.md)
      - [Profesi dan tugas dalam PPLG](dunia-kerja-proyek-mutu/01-profesi-pplg.md)
      - [Proses bisnis dan tahapan proyek](dunia-kerja-proyek-mutu/02-proses-bisnis-dan-proyek.md)
      - [Budaya mutu](dunia-kerja-proyek-mutu/03-budaya-mutu.md)
      - [HAKI dan lisensi](dunia-kerja-proyek-mutu/04-haki-dan-lisensi.md)
      - [Technopreneurship](dunia-kerja-proyek-mutu/05-technopreneurship.md)
3. K3LH, budaya kerja, aset, dan sistem operasi:
   - Sumber materi: [sumber materi K3LH, aset, dan sistem operasi](k3lh-aset-os/materi-k3lh-aset-os.md)
      - [Dasar K3LH, budaya kerja, aset, dan sistem operasi](k3lh-aset-os/00-dasar-k3lh-aset-os.md)
      - [K3LH di lingkungan kerja PPLG](k3lh-aset-os/01-k3lh.md)
      - [Budaya kerja profesional](k3lh-aset-os/02-budaya-kerja.md)
      - [Pengelolaan aset proyek](k3lh-aset-os/03-pengelolaan-aset.md)
      - [Sistem operasi, berkas, dan direktori](k3lh-aset-os/04-sistem-operasi-file.md)
4. Jaringan dan TCP/IP:
   - Sumber materi: [sumber materi Jaringan dan TCP/IP](jaringan-tcpip/materi-jaringan-tcpip.md)
      - [Dasar jaringan dan model TCP/IP](jaringan-tcpip/00-dasar-jaringan-dan-tcp-ip.md)
      - [Client-server dan DNS](jaringan-tcpip/01-client-server-dan-dns.md)
      - [HTTP dan API](jaringan-tcpip/02-http-dan-api.md)
      - [Diagnosis konektivitas](jaringan-tcpip/03-diagnosis-konektivitas.md)
5. Tipe/struktur data dan kontrol:
   - Sumber materi: [sumber materi Tipe/struktur data dan kontrol](data-control/materi-data-kontrol.md)
      - [Dasar tipe data, struktur data, dan struktur kontrol](data-control/00-dasar-tipe-struktur-data-dan-kontrol.md)
      - [Tipe data dasar](data-control/01-tipe-data.md)
      - [Struktur data dasar](data-control/02-struktur-data.md)
      - [Percabangan dan perulangan](data-control/03-percabangan-dan-perulangan.md)
      - [Tracing dan jebakan umum](data-control/04-tracing-dan-jebakan-umum.md)
6. Fungsi, prosedur, dan modularisasi:
   - Sumber materi: [sumber materi Fungsi, prosedur, dan modularisasi](modularisasi/materi-modularisasi.md)
      - [Dasar fungsi, prosedur, dan modularisasi](modularisasi/00-dasar-fungsi-prosedur-dan-modularisasi.md)
      - [Fungsi dan prosedur](modularisasi/01-fungsi-dan-prosedur.md)
      - [Parameter, return, scope, dan efek samping](modularisasi/02-parameter-return-scope-dan-efek-samping.md)
      - [Desain dan pengujian modular](modularisasi/03-desain-dan-pengujian-modular.md)
7. OOP: class, enkapsulasi, inheritance, polymorphism
   - Sumber materi: [sumber materi OOP: class, enkapsulasi, inheritance, polymorphism](oop/materi-oop.md)
      - [Dasar Object-Oriented Programming](oop/00-dasar-oop.md)
      - [Class dan object](oop/01-class-dan-object.md)
      - [Enkapsulasi dan access modifier](oop/02-enkapsulasi-dan-access-modifier.md)
      - [Inheritance dan komposisi](oop/03-inheritance-dan-komposisi.md)
      - [Polymorphism dan method overriding](oop/04-polymorphism-dan-overriding.md)
8. Tracing dan latihan skenario
   - Indeks materi: [Tracing dan latihan skenario PPLG](tracing-secenario/materi-tracing-skenario.md)
      - [Tracing data dan struktur kontrol](tracing-secenario/01-tracing-data-dan-kontrol.md)
      - [Skenario dunia kerja, proyek, dan mutu](tracing-secenario/02-skenario-dunia-kerja-dan-mutu.md)
      - [Skenario K3LH, budaya kerja, aset, dan sistem operasi](tracing-secenario/03-skenario-k3lh-aset-dan-os.md)
      - [Skenario jaringan, HTTP, dan API](tracing-secenario/04-skenario-jaringan-http-dan-api.md)
      - [Skenario fungsi dan modularisasi](tracing-secenario/05-skenario-fungsi-dan-modularisasi.md)
      - [Skenario Object-Oriented Programming](tracing-secenario/06-skenario-oop.md)
      - [Latihan integratif PPLG](tracing-secenario/07-latihan-integratif-pplg.md)

PPLG tidak diuji sebagai hafalan sintaks satu bahasa. Biasakan membaca
pseudocode atau potongan kode, mengenali efeknya, lalu memilih desain yang
paling aman/efektif untuk skenario proyek.
