# 🗺️ Peta Infografis Interaktif Sebaran Mahasiswa S1 Angkatan 2024 (IT-PLN)

Aplikasi web visualisasi dan peta infografis interaktif sebaran asal domisili mahasiswa baru program sarjana (S1) Reguler Angkatan 2024 Institut Teknologi PLN (IT-PLN).

Dibangun menggunakan integrasi peta **OpenStreetMap (OSM)** dan **Leaflet**, aplikasi ini memungkinkan eksplorasi geografis bertingkat (*drill-down*) dari skala Nasional hingga tingkat Kecamatan secara presisi.

---

## ✨ Fitur Utama

- 🌐 **Peta Realistis OpenStreetMap (OSM)**: Menampilkan kontur wilayah, batas administratif, jalan tol, dan jalan lokal hingga tingkat kecamatan.
- 🎨 **Multi-Basemap Switcher**:
  - `🗺️ OSM Standar`: Peta resmi OpenStreetMap.
  - `🌍 Humanitarian`: OSM berfokus pada kontras tinggi batas wilayah.
  - `🛰️ Satelit`: Citra satelit bumi nyata.
  - `🌙 Dark OSM`: Mode malam elegan.
  - `☀️ Voyager`: Tampilan terang minimalis.
- 🔍 **Eksplorasi Bertingkat (Drill-Down 3 Level)**:
  - **Level 1 (Nasional)**: 33 Provinsi dengan bubble marker proporsional.
  - **Level 2 (Provinsi)**: 261 Kota & Kabupaten.
  - **Level 3 (Kota/Kabupaten)**: 576 Kecamatan dengan koordinat presisi.
- 📋 **Modal & Kartu Detail**: Klik pin kecamatan untuk melihat rincian jumlah mahasiswa per program studi.
- 🔎 **Pencarian Cepat (*Instant Autocomplete*)**: Cari langsung nama kecamatan, kota, atau provinsi.
- 🎓 **Filter Multi-Dimensi**: Filter berdasarkan 11 Program Studi dan 6 gugus kepulauan di Indonesia.
- 📊 **Panel Statistik & Peringkat**: Peringkat 10 besar kecamatan, kota, dan provinsi asal mahasiswa terbanyak.
- 📥 **Master Data Table & Export CSV**: Tabel lengkap 576 kecamatan yang dapat disaring dan diunduh ke format Excel/CSV.

---

## 📈 Ringkasan Statistik Data

| Indikator | Jumlah | Keterangan |
| :--- | :---: | :--- |
| **Total Mahasiswa** | **883** | Mahasiswa S1 Reguler Angkatan 2024 |
| **Program Studi** | **11** | Teknik & Manajemen Bisnis |
| **Provinsi Terjangkau** | **33** | Dari 38 Provinsi di Indonesia |
| **Kota / Kabupaten** | **261** | Dari Sabang sampai Merauke |
| **Kecamatan Presisi** | **576** | Terpetakan dengan titik koordinat |

---

## 🚀 Cara Menjalankan

1. Clone repositori ini:
   ```bash
   git clone https://github.com/anj1n923/Infografis_posisi_domisili_mahasiswa2024.git
   cd Infografis_posisi_domisili_mahasiswa2024
   ```

2. Buka `index.html` langsung di browser Anda (Google Chrome, Firefox, Safari, atau Microsoft Edge).
   *Tidak memerlukan instalasi server backend atau dependensi tambahan!*

3. **Deploy ke GitHub Pages**:
   - Buka menu **Settings** > **Pages** di repositori GitHub Anda.
   - Pada bagian **Build and deployment > Source**, pilih branch `main` dan folder `/ (root)`.
   - Simpan (*Save*), dan website infografis akan otomatis aktif secara online melalui URL GitHub Pages Anda.

---

## 📁 Struktur Direktori

```text
├── index.html       # Aplikasi web peta interaktif mandiri (Leaflet + OSM)
├── geo_data.json    # Dataset geografis hierarkis (Provinsi -> Kota -> Kecamatan)
├── raw_data.json    # Data mentah ekstraksi Sheet 1
└── README.md        # Dokumentasi proyek
```

---

## 📜 Lisensi & Atribusi Data

- **Sumber Data Mahasiswa:** Data Sheet 1 S1 Reguler 2024 - Institut Teknologi PLN.
- **Peta & Kartografi:** Data peta terbuka © [OpenStreetMap](https://www.openstreetmap.org/copyright) contributors.
- **Map Engine:** [Leaflet.js](https://leafletjs.com/).
