# Aksara — REST API Peminjaman Buku

API pencatatan peminjaman buku perpustakaan. Petugas meja sirkulasi mencatat buku yang dipinjam anggota, memperbarui data (termasuk pengembalian), menghapus catatan yang salah, dan menyaring daftar — misalnya hanya yang **terlambat**.

Dibangun dengan **Node.js**, **Express.js**, dan **Supabase** (Postgres). Jika kredensial Supabase belum diisi, API tetap jalan dengan penyimpanan memori dan data contoh supaya endpoint bisa langsung diuji.

## Base URL

Deployment Vercel (diperbarui otomatis setelah publish):

**Belum dipublish.** Setelah repository terhubung ke Vercel, base URL berbentuk `https://<nama-proyek>.vercel.app`.

Contoh pemanggilan begitu URL itu ada:

```bash
curl "https://<nama-proyek>.vercel.app/loans?status=Terlambat"