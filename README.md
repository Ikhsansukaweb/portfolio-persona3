# Portfolio — Muhammad Ikhsan Setiawan

Portfolio interaktif bergaya **Persona 3 Reload Pause Menu**, dibangun dengan HTML, CSS, dan JavaScript murni (tanpa framework).

Dibuat ulang secara pixel-perfect dari estetika Atlus: layout miring dinamis, banner geometris pecah, transisi lingkaran, video background, dan efek suara Web Audio.

## Fitur

- **Menu utama bergaya P3R** — navigasi keyboard (panah + ENTER + ESC) dan mouse
- **PROJECT** — kartu social-link berisi project nyata, klik untuk buka repo GitHub
- **SKILLS** — bar statistik dengan tab kategori (Frontend / Backend / Mobile / Tools)
- **ABOUT** — profil, foto, bio, dan kutipan
- **CONTACT** — UI pesan ponsel dengan alamat email
- **Loading screen** dengan progress bar
- **Sound effect** (Web Audio API) untuk navigasi dan konfirmasi
- **Video background** per halaman

## Struktur

```
index.html          markup utama (menu, 4 halaman, modal)
css/style.css       seluruh gaya visual
js/main.js          data + engine interaksi & animasi
assets/             video background, foto profil, favicon
fonts/              font Persona 3 (Rodin Pro, Skip Std)
sfx/                efek suara menu
```

## Menjalankan

Cukup buka `index.html`, atau jalankan server lokal:

```bash
python3 -m http.server 8000
```

Lalu buka `http://localhost:8000`.

## Data

Semua isi portfolio (project, skill, profil, kontak) ada di bagian atas `js/main.js`:

| Variabel | Isi |
|---|---|
| `options` | 4 menu utama + kartu modal |
| `slinkData` | Kartu project (judul, subjudul, link) |
| `skillTabsList` | Tab kategori skill |
| `skillGroupsData` | Daftar skill + nilai level |

## Kredit

Desain awal terinspirasi **Persona 3 Reload** (Atlus). Seluruh isi dan data diubah untuk portfolio pribadi.
