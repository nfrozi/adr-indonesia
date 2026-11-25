# 001. Memakai MySQL sebagai database

- **Tanggal:** 2026-11-25
- **Status:** Diterima
- **Pengambil keputusan:** Seluruh anggota tim

## Konteks

Aplikasi mencatat barang, kategori, dan transaksi penjualan. Data berbentuk tabel dan saling berhubungan (lihat `docs/erd.md`). Seluruh anggota tim sudah pernah memakai SQL dasar pada mata kuliah basis data. Mitra tidak punya server khusus, sehingga database harus bisa dijalankan di laptop untuk uji coba.

## Alternatif yang dipertimbangkan

- MySQL: relasional, banyak materi belajar, mudah dipasang.
- PostgreSQL: relasional dan kaya fitur, tetapi belum dikenal tim.
- Database dokumen: kurang cocok untuk data yang banyak relasi.

## Keputusan

Kami memakai MySQL sebagai database. Skema disimpan sebagai skrip SQL di `database/schema.sql`, dan data uji di `database/seed.sql`.

## Konsekuensi

+ Seluruh anggota langsung bisa bekerja tanpa belajar teknologi baru.
+ Skema bisa dibuat ulang dari skrip di laptop mana pun.
- Perlu memasang server MySQL di setiap laptop dan di server uji.
- Bila nanti butuh fitur khusus yang tidak ada di MySQL, keputusan ini ditinjau ulang lewat ADR baru.
