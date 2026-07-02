# 🎯 TUBES ELMAG — Physics Golf Game

Tugas Besar Elektromagnetika yang mengimplementasikan simulasi fisika sederhana dalam bentuk game bergaya **mini-golf**. Pemain menarik bola menggunakan mouse untuk memberikan gaya dorong, lalu bola akan bergerak mengikuti hukum fisika (gaya, gesekan, dan tumbukan) hingga masuk ke dalam lubang di setiap level.

![Python](https://img.shields.io/badge/Python-100%25-blue)
![Pygame](https://img.shields.io/badge/Engine-Pygame-green)

---

## ✨ Fitur

- Simulasi fisika bola: gaya dorong, gesekan permukaan, dan pantulan terhadap dinding
- Sistem multi-level dengan desain lintasan berbeda tiap level
- Rintangan bergerak (*carts*) yang dapat menggagalkan permainan jika tersentuh
- Sistem nyawa (*lives*) — permainan dimulai ulang dari level tersebut jika nyawa habis
- Kontrol drag-and-release untuk menentukan arah dan kekuatan tembakan bola

---

## 🎮 Cara Bermain

1. Klik tombol **Start** pada layar awal untuk memulai permainan
2. **Klik dan tahan** pada bola, lalu **tarik ke arah berlawanan** dari tujuan tembakan
3. **Lepaskan klik** untuk menembakkan bola — semakin jauh tarikan, semakin besar gayanya
4. Arahkan bola hingga masuk ke dalam lubang untuk lanjut ke level berikutnya
5. Hindari menyentuh rintangan (cart) dan area di luar lintasan agar tidak kehilangan nyawa

---

## 🔧 Prasyarat

Pastikan Anda telah menginstal:
- **Python 3.10+**
- **Pygame**

---

## 🚀 Cara Menjalankan

### Opsi 1 — Menjalankan langsung (executable)
Jalankan file `main.exe` yang tersedia di root folder (khusus Windows).

### Opsi 2 — Menjalankan dari source code
```bash
# Install dependensi
pip install pygame

# Jalankan game
python main.py
```

---

## 📁 Struktur Proyek
TUBES-ELMAG/
├── images/              # Aset gambar/sprite game
├── main.py              # Entry point dan game loop utama
├── game_manager.py      # Pengelolaan level, skor, dan status permainan
├── game_objects.py      # Definisi objek Ball dan Hole
├── physics.py           # Perhitungan fisika: gaya, gesekan, tumbukan
├── rigidbody.py         # Struktur dasar objek dengan properti fisik
├── shapes.py            # Definisi bentuk geometri (Line, dsb.)
├── scene.py             # Pengelolaan scene/tampilan
├── levels.py            # Definisi dan konfigurasi tiap level
├── cell.py              # Representasi grid/sel pada papan permainan
├── transformation.py    # Konversi koordinat piksel ke indeks grid
├── sprite_sheet.py       # Pengelolaan sprite sheet untuk animasi
├── config.py             # Konfigurasi global (ukuran layar, radius bola, dll.)
└── main.exe              # Build executable untuk Windows

## 📄 Lisensi
Proyek ini dibuat untuk keperluan tugas akademik mata kuliah Elektromagnetika.
