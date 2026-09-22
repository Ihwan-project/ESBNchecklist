# Checklist Simulasi Demo Sistem Transaksi SBSN Ritel Online

Formulir checklist untuk pengujian (demo) sistem penjualan SBSN Ritel oleh Mitra Distribusi.
Direktorat Jenderal Pengelolaan Pembiayaan dan Risiko (DJPPR) — Kementerian Keuangan.

## Buka formulir

👉 **https://Ihwan-project.github.io/checklist-pengujian-sbsn/**

_(ganti `USERNAME` dengan nama akun GitHub Anda setelah GitHub Pages aktif)_

## Cakupan pengujian

| Bagian | Isi |
|---|---|
| Pra‑pengujian | Disclaimer, ketentuan & syarat, kesiapan environment |
| Investor A | Registrasi → Pemesanan & Pembayaran SR → Ubah Parameter Seri → Pemesanan SR → Pemesanan ST |
| Investor B | Registrasi → Update Profile/Data Investor → Pemesanan & Pembayaran ST |
| Early Redemption | Investor A (cek menu & eligibilitas), Investor B (pengujian nominal) |
| Cek e‑mail | Konfirmasi registrasi, pemesanan, pembayaran, dan early redemption |

Total 63 butir uji, masing‑masing dengan status **Pass / Fail / N‑A**, kolom catatan, dan lampiran screenshot.

## Cara pakai

1. Buka tautan di atas (cukup lewat browser, tidak perlu instalasi).
2. Isi identitas pengujian: Mitra Distribusi, evaluator, tanggal, environment, seri SR/ST.
3. Isi data Investor A dan Investor B pada tabel **Data Investor Pengujian**.
4. Tandai setiap butir uji dengan Pass/Fail/N‑A dan lampirkan screenshot bila diperlukan.
5. Simpan hasil:
   - **Simpan progres** → berkas `.json` untuk dilanjutkan/di‑share ke rekan penguji (gunakan **Muat progres** untuk membukanya kembali).
   - **Ekspor CSV / Excel** → rekap untuk diolah lebih lanjut.
   - **Cetak / Simpan PDF** → dokumen berita acara pengujian.

## Catatan privasi

Halaman ini **tidak mengirim data ke mana pun**. Semua isian hanya berada di browser penguji
sampai diekspor sendiri menjadi berkas JSON/CSV/PDF. Karena repositori ini bersifat publik,
**data investor (nama, SID, NIK, tanggal lahir) sengaja dikosongkan** dari berkas HTML.
Data pengujian yang sebenarnya cukup disimpan pada berkas progres `.json` di komputer masing‑masing
dan **jangan diunggah ke repositori ini**.

## Struktur berkas

```
index.html    — formulir checklist (mandiri, tanpa dependensi eksternal)
robots.txt    — mencegah halaman diindeks mesin pencari
.nojekyll     — agar GitHub Pages menyajikan berkas apa adanya
.gitignore    — mencegah berkas progres/ekspor ikut terunggah
```

## Perubahan

| Versi | Tanggal | Keterangan |
|---|---|---|
| 1.0 | 2026-09-22 | Rilis awal — 63 butir uji |
