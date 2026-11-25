# Catatan Keputusan Arsitektur (ADR)

Folder ini berisi catatan keputusan teknis penting proyek, satu keputusan per berkas, supaya seluruh anggota tim dan dosen paham **alasan** di balik pilihan yang diambil.

## Kapan menulis ADR?

Tulis ADR saat tim memilih hal yang sulit diubah atau berdampak pada banyak bagian, misalnya:

- database atau framework yang dipakai
- pembagian modul dan struktur proyek
- cara login dan hak akses
- cara menyimpan data pribadi
- cara deployment

Perubahan kecil seperti nama variabel tidak perlu ADR.

## Cara menulis

1. Salin `000-template.md` menjadi `NNN-judul-singkat.md` (nomor urut berikutnya).
2. Isi bagian Konteks, Alternatif, Keputusan, dan Konsekuensi.
3. Buka Pull Request dan minta tinjauan anggota lain.
4. Setelah di-merge, ubah Status menjadi **Diterima**.

## Jika keputusan berubah

Jangan hapus ADR lama. Tulis ADR baru, lalu ubah Status ADR lama menjadi **Digantikan oleh ADR-NNN** dan tautkan ke ADR baru.

## Daftar ADR

| No | Judul | Status |
| -- | ----- | ------ |
| 001 | [Memakai MySQL sebagai database](001-contoh-memakai-mysql.md) | Diterima |

## Rujukan

- GDS. (2026). Architecture decisions. The GDS Way. https://gds-way.digital.cabinet-office.gov.uk/standards/architecture-decisions.html
- Nygard, M. (2011). [Documenting architecture decisions](https://cognitect.com/blog/2011/11/15/documenting-architecture-decisions). Cognitect Blog.
- https://adr.github.io
