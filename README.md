# 🎂 Birthday Riddle Gatekeeper

Sebuah platform digital sederhana yang dirancang sebagai kado ulang tahun interaktif. Website ini berfungsi sebagai "pintu gerbang" di mana penerima harus memecahkan teka-teki personal sebelum dapat mengakses pesan ucapan utama.

---

## 🛠️ Tech Stack

Project ini dibangun dengan pendekatan minimalis agar ringan dan mudah diakses melalui perangkat mobile:

* **Frontend:** HTML5, Tailwind CSS (via CDN)
* **Interactivity:** Vanilla JavaScript
* **Animations:** [Canvas Confetti](https://github.com/catdad/canvas-confetti)
* **Deployment:** Vercel / Netlify / GitHub Pages

---

## 🏗️ Alur Fitur (User Journey)

1.  **The Riddle Stage**: Pengunjung disambut dengan pertanyaan atau memori spesifik. Akses ke konten utama dikunci di balik validasi input.
2.  **Gatekeeping Logic**: Logika JavaScript sederhana untuk mencocokkan input dengan kunci jawaban (case-insensitive).
3.  **The Celebration Stage**: Setelah jawaban benar, sistem akan:
    * Memicu animasi confetti.
    * Menampilkan pesan ucapan dengan efek *typewriter*.
    * Memutar latar musik (optional).

---

## 📂 Struktur Folder

```text
├── index.html          # Halaman utama & Logika Teka-teki
├── assets/
│   ├── css/            # Custom styling (jika diperlukan)
│   ├── js/             # Script utama
│   ├── img/            # Galeri foto kenangan
│   └── audio/          # Musik latar
└── README.md
```

---

## 🚀 Cara Penggunaan

1.  **Clone Repository**:
    ```bash
    git clone https://github.com/username/birthday-riddle.git
    ```
2.  **Sesuaikan Teka-Teki**:
    Buka `index.html` dan cari bagian script untuk mengubah variabel `correctAnswer` dan teks pertanyaan.
3.  **Kustomisasi Pesan**:
    Isi bagian ID `#birthday-content` dengan pesan personal, foto, atau video.
4.  **Deploy**:
    Hubungkan repository ini ke Vercel atau Netlify untuk mendapatkan URL publik yang bisa dikirimkan kepada si penerima.

---

## 📝 Catatan Pengembangan

* **Responsivitas**: Website dioptimalkan untuk tampilan mobile-first mengingat link kemungkinan besar diakses melalui aplikasi chat.
* **Keamanan**: Karena ini adalah proyek berbasis client-side, jawaban disimpan dalam kode JavaScript. Ini cukup untuk penggunaan personal selama penerima tidak melakukan *inspect element*.

---

> "Karena sebuah ucapan akan terasa lebih bermakna jika ada sedikit perjuangan di dalamnya." ✨