# SIMPASI (Sistem Perencanaan dan Analisis Simpang APILL) - Universitas Tidar

Aplikasi Web Interaktif Profesional untuk Analisis Kapasitas dan Kinerja Simpang Bersinyal (APILL) berdasarkan standar **Pedoman Kapasitas Jalan Indonesia (PKJI 2023 - Ditjen Bina Marga Kementerian PUPR)**.

**Dibuat dan dikembangkan oleh: Kintan Alifia Astari (Universitas Tidar)**  
*Jurusan Teknik Sipil, Fakultas Teknik, Universitas Tidar Magelang*

---

## 🌟 Fitur & Spesifikasi Teknis

1. **Header & Branding Akademik**
   - Logo resmi Universitas Tidar Magelang.
   - Tombol "💾 Simpan Sesi" (LocalStorage) & "📂 Muat Proyek" (Reload data).
   - Tombol "📄 Cetak Laporan PDF Profesional" (Kop Surat Resmi Universitas Tidar).
   - Sakelar Light Mode & Dark Mode.

2. **Modul Utama & Navigasi Tab**
   - **Tab 1: Form Input Data & Rekomendasi Pakar**:
     - Input geometri simpang 4 lengan (Utara, Timur, Selatan, Barat): Lebar masuk ($W_a$), lebar keluar ($W_{out}$), lebar LTOR, kelandaian.
     - Input volume arus lalu lintas per gerakan (LT, ST, RT) terurai KR, KB, SM.
     - Pilihan fase APILL (2 s.d. 4 fase), tipe lingkungan (COM, RES, RAC), ukuran kota.
     - Kotak interaktif "💡 Panduan Pakar" (Analisis Pros & Cons Tipe Pendekat P/O dan Jumlah Fase).
   - **Tab 2: Peta GIS Interaktif (Leaflet.js)**:
     - Penandaan koordinat geografis simpang dengan fitur klik peta untuk auto-fill lokasi (*default* Magelang).
   - **Tab 3: Laporan Formulir SA-I s.d. SA-V**:
     - Rekapitulasi presisi standar PKJI 2023 mulai dari konversi skru/jam, arus jenuh $S_0$ & $S$, waktu siklus Webster $c$, alokasi hijau $g_i$, kapasitas $C$, derajat kejenuhan $DS$, panjang antrian $QL$, hingga tundaan $D$ dan Tingkat Pelayanan (LOS A-F).
     - Panel rumus matematika transparan (*Explainable Engine*).
   - **Tab 4: Grafik Analisis Kinerja (Chart.js)**:
     - Visualisasi Derajat Kejenuhan ($DS$) per lengan pendekat dengan garis batas kritis $DS = 0.85$ dan grafik garis tundaan.
   - **Tab 5: Simulasi Visual 2D Top-Down Simpang APILL**:
     - Animasi HTML5 Canvas top-down simpang 4 lengan yang merender lampu lalu lintas (Merah, Kuning, Hijau) dan pergerakan blok kendaraan secara proporsional sesuai waktu siklus.

3. **Watermark Identitas Resmi**:
   - Tercantum rapi di bagian footer web:  
     **"Dibuat dan dikembangkan oleh Kintan Alifia Astari (Universitas Tidar)"**
   - Otomatis tercetak di bagian footer setiap halaman dokumen laporan PDF resmi.

---

## 📚 Landasan Standar
- **PKJI 2023**: Pedoman Kapasitas Jalan Indonesia, Bagian Simpang Bersinyal, Direktorat Jenderal Bina Marga, Kementerian PUPR.
- **F.V. Webster (1958)**: *Traffic Signal Settings*, Road Research Technical Paper.
