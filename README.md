# AR Wall 3D

Web app ringan untuk menempelkan foto persegi di tampilan kamera dengan metode **4 titik sudut**.

## Fitur
- Upload foto dari splash screen.
- Mulai AR lalu atur foto dengan **drag 4 titik sudut** (TL, TR, BR, BL).
- Tanpa slider position/rotation: pengaturan perspektif langsung dari sudut.
- Flip horizontal, reset titik, simpan snapshot.

## Menjalankan project
```bash
python3 -m http.server 4173
```
Buka `http://localhost:4173`.

## Cara pakai
1. Pilih foto (disarankan rasio 1:1/persegi).
2. Tekan **Mulai AR**.
3. Geser 4 titik sudut di kanvas agar pas ke bidang dinding.
4. Tekan **Simpan** untuk ekspor hasil gabungan kamera + overlay.

## Struktur
- `index.html`: UI + logika kamera + warp 4 sudut.
