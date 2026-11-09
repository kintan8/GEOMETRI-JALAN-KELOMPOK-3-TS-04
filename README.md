# SID-JALAN UNTIDAR - Perencanaan Geometrik Jalan & Kanvas CAD Interaktif

Aplikasi Web Interaktif Perencanaan Geometrik Jalan Terintegrasi berbasis Standar Bina Marga PDGJ 2021 dan Buku "Dasar-Dasar Perencanaan Geometrik Jalan" oleh Prof. Ir. Silvia Sukirman.

Dikembangkan oleh **Kintan Alifia Astari & Kelompok 3 TS-04** - Jurusan Teknik Sipil, Fakultas Teknik, **Universitas Tidar (UNTIDAR)** Magelang.

---

## Fitur Utama

1. **Parameter Desain & Koordinat Trase WGS-84**
   - Pemilihan klasifikasi medan (Datar, Perbukitan, Pegunungan).
   - Input koordinat GPS Google Earth (WGS-84 Lat/Lon) dengan fitur Quick Paste.
   - Peta Pratinjau Interaktif Leaflet dengan citra satelit resolusi tinggi ESRI World Imagery.
   - Perhitungan otomatis jarak antar-PI, azimut sudut kompas, dan sudut defleksi tikungan.

2. **Analisis Alinyemen Horizontal (Bina Marga PDGJ 2021 & Silvia Sukirman)**
   - Klasifikasi otomatis jenis tikungan:
     - **Full Circle (F-C)**
     - **Spiral - Circle - Spiral (S-C-S)**
     - **Spiral - Spiral (S-S)**
   - Perhitungan superelevasi desain ($e$), panjang peralihan ($L_s$), pergeseran busur ($p$), absis ($k$), tangen ($T_s / T_c$), jarak eksternal ($E_s / E_c$), dan panjang total tikungan ($L_{tot}$).
   - Evaluasi kelayakan teknis: pencegahan overlap tikungan dan waktu tempuh minimal pada busur lingkaran ($L_c \ge 25$ m).

3. **Kanvas CAD Interaktif (AutoCAD Style Drawing)**
   - **Mode Lengkung Lengkap**: Mendukung semua jenis tikungan (F-C, S-C-S, dan S-S).
   - **Visualisasi Gambar Kerja Standar**: Batas kertas gambar (A4, A3, OFF), margin teknis, dan Kop Etiket resmi Universitas Tidar.
   - **Anotasi Dimensi Teknik**: Dimensi otomatis untuk $T_s / T_c$, $E_s / E_c$, $L_s$, $L_c$, $R$, $\Delta$, $\theta_s$, $p$, dan $k$.
   - **Kontrol Layer CAD (ON/OFF)**:
     - `GARIS_UTAMA` (Tangen, Busur Lengkung, Spiral)
     - `GARIS_SUMBU` (Sumbu Jalan, Sumbu Bagi PI-O)
     - `GARIS_POTONG` (Garis Jari-jari Radial ke Pusat O)
     - `DIMENSI_NOTASI` (Ukuran dan Notasi Teknik)
     - `TITIK_KONTROL` (PI, TC, CT, TS, SC, CS, ST, O)
     - `KOP_ETIKET` (Garis Kertas, Judul Gambar, Skala Grafis, Arah Utara)
   - **Detail Notasi Interaktif**: Klik elemen garis atau dimensi pada kanvas untuk memunculkan detail parameter, rumus matematis, serta penjelasan teknis dan standar Bina Marga.
   - **Ekspor Vektor & Raster**:
     - **Unduh DXF**: Format standar ASCII DXF yang dapat dibuka langsung di AutoCAD, Civil 3D, atau LibreCAD.
     - **Unduh PNG**: Raster resolusi tinggi siap cetak.
   - **Workspace OpenCAD Studio**: Drawer parametrik live untuk menyetel $R$, $\Delta$, $L_s$, dan $V_d$ secara bebas dengan pembaruan kanvas seketika.

4. **Alinyemen Vertikal & Profil Memanjang 2D**
   - Lengkung vertikal cembung (crest) dan cekung (sag).
   - Diagram profil memanjang 2D dengan arsiran galian (cut) dan timbunan (fill) serta estimasi volume tanah.

5. **Visualisasi 3D & Google Earth Export**
   - Ekspor trase jalan ke format 3D KML untuk visualisasi langsung di Google Earth Desktop & Web.
   - Ekspor rekapitulasi stasioning dan koordinat ke CSV/Excel.

---

## Deploy & Akses Live

Aplikasi ini dideploy secara otomatis di Vercel:
👉 **[https://sid-jalan-untidar.vercel.app](https://sid-jalan-untidar.vercel.app)**

Repository GitHub:
👉 **[https://github.com/kintan8/GEOMETRI-JALAN-KELOMPOK-3-TS-04](https://github.com/kintan8/GEOMETRI-JALAN-KELOMPOK-3-TS-04)**
