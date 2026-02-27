# AR Wall 3D

Web app sederhana untuk menempelkan foto ke dinding secara AR-style lewat kamera HP.

## Fitur
- Upload foto dari splash screen.
- Tombol **Mulai AR** untuk masuk ke mode kamera.
- Kontrol posisi (`X/Y/Z`), rotasi (`X/Y/Z`), dan ukuran.
- Lock tracking, flip foto, reset, dan simpan snapshot.
- Kompatibel untuk Safari iOS dan Chrome Android.

## Cara menjalankan
Karena ini single-file app, cukup jalankan static server dari root project:

```bash
python3 -m http.server 4173
```

Lalu buka:

- `http://localhost:4173`

> Untuk HP, akses lewat IP LAN mesin yang menjalankan server.

## Catatan penggunaan
- Saat tidak ada data gyroscope (atau izin belum diberikan), objek sekarang tetap dibuat dengan orientasi default supaya gambar langsung terlihat setelah tekan **Mulai AR**.
- Di iOS, jika diminta, izinkan sensor gerak agar tracking lebih natural.

## Struktur project
- `index.html`: UI, styling, dan seluruh logika AR/canvas.
