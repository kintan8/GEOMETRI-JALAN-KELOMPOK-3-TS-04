# SID-JALAN UNTIDAR | Sistem Informasi Desain Geometrik Jalan Raya

Aplikasi Web Interaktif (Kalkulator & Sistem Pakar) untuk Perencanaan Geometrik Jalan Raya berdasarkan standar **Pedoman Desain Geometrik Jalan (PDGJ 2021 Ditjen Bina Marga)** dan literatur akademik **"Dasar-Dasar Perencanaan Geometrik Jalan" (Silvia Sukirman)**.

Dikembangkan untuk civitas akademika **Jurusan Teknik Sipil, Fakultas Teknik, Universitas Tidar Magelang**.

---

## 🌟 Fitur Utama

1. **Header & Academic Branding**
   - Logo resmi Universitas Tidar Magelang.
   - Sakelar Light Mode & Dark Mode.
   - Preset studi kasus (Trase Berbukit Vd=60 km/j & Trase Datar Vd=80 km/j).

2. **Formulir Input Koordinat Dinamis (Google Earth WGS-84)**
   - Mendukung input langsung **Latitude & Longitude** yang disalin dari Google Earth.
   - Penyelarasan otomatis ke koordinat metrik lokal $(X, Y)$ secara presisi.
   - Fitur *Quick Paste* koordinat format `Lat, Lon`.

3. **Jendela Pratinjau Posisi Koordinat & Denah Trase (Live Preview Window)**
   - Pratinjau langsung di atas foto satelit bumi resolusi tinggi (ESRI World Imagery).
   - Klik langsung di peta satelit untuk menambahkan titik PI baru.
   - Garis tangen dan lengkung jalan ter-update seketika (*real-time*).

4. **Sistem Rekomendasi Parameter (💡 Saran Pakar & Pros-Cons)**
   - Analisis $R_{min}$ matematis vs $R$ rekomendasi di lapangan.
   - Evaluasi panjang peralihan ($L_s$) berdasarkan 3 kriteria (Modifikasi Shortt, Kelandaian Relatif, dan Waktu Tempuh 3 Detik).
   - Rekomendasi bentuk tikungan (Full Circle vs Spiral-Circle-Spiral vs Spiral-Spiral).
   - Peringatan keamanan alinyemen vertikal ($L_v$ vs Waktu Tempuh 3 Detik dan Jarak Pandang Henti JPH).

5. **Hasil Perhitungan Stationing (STA) Kontinu**
   - Perhitungan stasioning resmi sepanjang sumbu jalan (STA PI, STA TS, STA SC, STA CS, STA ST).
   - Tabel Rangkuman Stationing Titik-Titik Kritis Trase Jalan.

6. **Explainable Engine & Landasan Teori**
   - Accordion rumus matematis lengkap dan narasi acuan standar Bina Marga.

7. **Visualisasi Grafik Profil 2D & Export Multi-Format**
   - Profil Memanjang (Longitudinal Profile Canvas) dengan arsiran Galian (*Cut*) & Timbunan (*Fill*).
   - Export file **Excel / CSV**.
   - Export file **KML 3D** untuk dibuka langsung di **Google Earth Pro & Google Earth Web**.

---

## 🚀 Deployment ke Vercel

Proyek ini telah dikonfigurasi dengan `vercel.json` dan siap di-deploy langsung ke Vercel dalam hitungan detik.
Setiap perubahan (*commit & push*) pada repository GitHub akan otomatis memicu redeployment live pada Vercel.

---

## 📚 Landasan Standar & Referensi
- **PDGJ 2021**: Pedoman Desain Geometrik Jalan No. 13/P/BM/2021, Direktorat Jenderal Bina Marga, Kementerian Pekerjaan Umum dan Perumahan Rakyat.
- **Silvia Sukirman (1999)**: *Dasar-Dasar Perencanaan Geometrik Jalan*, Penerbit Nova, Bandung.
