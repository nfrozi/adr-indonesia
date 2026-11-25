# ADR Indonesia: Contoh & Templat Architecture Decision Records (ADR)

Repo ini berisi **contoh nyata dan templat Architecture Decision Records (ADR)** dalam Bahasa Indonesia. Cocok untuk tim proyek perkuliahan, komunitas, maupun tim software yang ingin mendokumentasikan keputusan teknis secara ringkas dan mudah ditinjau.

> *Architecture Decision Record* (ADR) adalah dokumen singkat yang mencatat satu keputusan arsitektur penting beserta **konteks**, **alternatif**, **keputusan**, dan **konsekuensinya** agar semua paham *alasan* di balik pilihan yang diambil, bukan hanya hasilnya.

## Isi repo

| Berkas | Keterangan |
| ------ | ---------- |
| [`docs/adr/README.md`](docs/adr/README.md) | Panduan kapan dan cara menulis ADR |
| [`docs/adr/000-templat.md`](docs/adr/000-template.md) | Template siap salin untuk ADR baru |
| [`docs/adr/001-contoh-memakai-mysql.md`](docs/adr/001-contoh-memakai-mysql.md) | Contoh ADR lengkap: keputusan memakai MySQL sebagai database |

## Cara memakai

1. Salin `docs/adr/000-template.md` menjadi `NNN-judul-singkat.md` (nomor urut berikutnya).
2. Isi bagian **Konteks**, **Alternatif yang dipertimbangkan**, **Keputusan**, dan **Konsekuensi**.
3. Buka Pull Request dan minta tinjauan anggota tim lain.
4. Setelah di-merge, ubah **Status** menjadi **Diterima**.
5. Bila keputusan berubah, jangan hapus ADR lama. Tulis ADR baru, lalu tandai ADR lama sebagai **Digantikan oleh ADR-NNN**.

## Kapan menulis ADR?

Tulis ADR saat tim memilih hal yang sulit diubah atau berdampak pada banyak bagian:

- database atau framework yang dipakai
- pembagian modul dan struktur proyek
- cara login dan hak akses
- cara menyimpan data pribadi
- cara deployment

Perubahan kecil seperti nama variabel tidak perlu ADR.

## Kenapa ADR?

- **Konteks keputusan tidak hilang** saat anggota tim berganti.
- **Reviu lebih terarah**. Keputusan dibahas lewat Pull Request.
- **Onboarding cepat**. Anggota baru paham arsitektur dan alasannya.
- **Audit & refleksi mudah**. Jejak keputusan teknis tersimpan rapi di version control.

## Rujukan

- GDS. Architecture decisions. The GDS Way. https://gds-way.digital.cabinet-office.gov.uk/standards/architecture-decisions.html
- Nygard, M. (2011). [Documenting architecture decisions](https://cognitect.com/blog/2011/11/15/documenting-architecture-decisions). Cognitect Blog.
- ADR GitHub. https://adr.github.io

## Lisensi

Repo ini dilisensikan di bawah [MIT License](LICENSE). Bebas digunakan, disalin, dan dimodifikasi untuk kebutuhan proyek Anda.
