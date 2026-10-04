# Lora — Browser Android yang Ringan

Lora adalah browser web Android yang kecil (± 2 MB) dan cepat, dibangun dengan Kotlin,
Jetpack Compose, dan Material 3 (dynamic color / Material You di Android 12+).

Repo ini hanya berisi **rilis APK**. Unduh versi terbaru di halaman
[**Releases**](https://github.com/wahyu6070/lora-browser-lite/releases/latest).

## Fitur

- **Multi-tab** dengan pemulihan sesi — tab dibuka kembali walau HP mati mendadak
- **Bisa dijadikan browser default** — membuka link http/https dari aplikasi lain
- **Mode penyamaran** dengan profil terpisah: cookie dan data situs dihapus saat keluar
- **Pengunduh bawaan**
  - konfirmasi sebelum mengunduh (nama berkas bisa diubah, ukuran ditampilkan)
  - pause / resume, lanjut otomatis saat koneksi putus
  - unduhan tetap tercatat setelah aplikasi ditutup dan bisa dilanjutkan
  - cek checksum SHA-256 / MD5
- **Pemblokir iklan & pelacak** (bisa dimatikan)
- **Mode malam** untuk halaman web, tanpa kedipan putih saat memuat
- Bookmark, riwayat, situs privat (disembunyikan dari riwayat)
- Ganti user-agent, mode desktop, cari di halaman, lihat sumber halaman, terjemahkan
- Izin kamera / mikrofon / lokasi **per situs**, hanya saat situs memintanya
- Login HTTP (misalnya halaman admin router) dan halaman error dengan tombol coba lagi
- Tampilan klasik (bar bawah) atau modern (bar atas ala Chrome), skala UI bisa diatur
- Bahasa: Indonesia, Inggris, Jepang, Mandarin, Rusia, Arab

## Persyaratan

- Android 8.0 (API 26) atau lebih baru
- Android System WebView / Google Chrome versi terbaru (disarankan, agar mode penyamaran
  bisa memisahkan cookie)

## Cara memasang

1. Buka [Releases](https://github.com/wahyu6070/lora-browser-lite/releases/latest) dan unduh
   berkas `lora-<versi>.apk`.
2. Buka berkasnya, izinkan "Instal aplikasi tak dikenal" untuk pengelola berkas / browser
   Anda bila diminta.
3. Pembaruan bisa dipasang langsung di atas versi lama — data tidak hilang.

## Izin yang dipakai

| Izin | Untuk apa |
|---|---|
| Internet, status jaringan | Menjelajah web |
| Notifikasi, layanan latar depan | Menampilkan dan menjaga unduhan tetap berjalan |
| Penyimpanan (hanya Android 10 ke bawah) | Menyimpan unduhan ke folder Download |
| Kamera, mikrofon, lokasi | Hanya ditanyakan saat sebuah situs memintanya |

Lora tidak memakai akses "semua berkas", tidak menyertakan pelacak, dan tidak mengirim
riwayat penjelajahan ke mana pun.

## Pembuat

Dibuat oleh [wahyu6070](https://github.com/wahyu6070).
