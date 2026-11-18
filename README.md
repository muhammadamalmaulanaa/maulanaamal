# 🎓 EDUFLEX — Learn Without Limits
### Platform Edukasi Digital untuk Pelajar, Mahasiswa, dan Pengajar

Proyek ini dibangun berdasarkan rancangan desain UI/UX dan struktur dashboard pada gambar acuan dengan ketelitian tinggi (**pixel-perfect, modern, clean, dan minimalis**), menggunakan palet warna dan tipografi resmi:
- **Font**: Poppins (Heading & Judul) & Inter (UI & Teks Konten)
- **Primary Blue**: `#2563EB` / `#3B82F6` (Electric Royal Blue)
- **Secondary Purple**: `#7C3AED` / `#8B5CF6` (Vibrant Indigo Purple)
- **Dark Slate / Navy**: `#0F172A` / `#1E293B` (Sidebar & Kontras Tinggi)
- **Background & Card**: `#F8FAFC` (Clean Light Gray) & `#FFFFFF` (Pure White)

---

## 🖼️ 6 Panel Tampilan Sesuai Rancangan Gambar

Aplikasi ini mengintegrasikan seluruh 6 tampilan mockup utama yang dapat diakses melalui alur navigasi normal maupun tombol **Quick Preview Roster** di bilah atas:

### 1. Landing Page (Public Page)
- **Header / Navbar**: Logo EDUFLEX dengan ikon topi wisuda, tautan navigasi (*Home, Courses, About*), tombol pencarian cepat, tombol *Login*, dan tombol *Register*.
- **Hero Section**: 
  - Judul besar: *"Unlock Your Potential with EDUFLEX"*
  - Deskripsi: *"Belajar keterampilan baru dengan cara yang lebih fleksibel, interaktif, dan menyenangkan."*
  - Tombol CTA: *"Explore Courses ->"*
  - Ilustrasi vektor 3D siswa memegang laptop dengan floating graduation badge dan ambient glowing circle (`assets/hero-student.svg`).
- **Floating Search & Category Pills**: Input cari kursus terpadu dengan filter pill kategori: `</> Programming`, `Design`, `Marketing`, dan `Business`.
- **Kursus Populer**: 3 kartu kursus unggulan:
  1. *UI/UX Design Fundamentals* (Andi Pratama, ⭐ 4.8, 12 Materi)
  2. *Web Development Basics* (Budi Santoso, ⭐ 4.7, 14 Materi)
  3. *Digital Marketing Strategy* (Sari Dewi, ⭐ 4.9, 10 Materi)

### 2. Dashboard Siswa (User Dashboard)
- **Sidebar Navy**: Logo EDUFLEX, menu *Dashboard, My Learning, Explore, Progress, Certificates, Profile*, serta tombol *Logout*.
- **Topbar**: Input pencarian kursus, ikon notifikasi aktif dengan indikator badge, dan inisial avatar pengguna (**AM** - Ahmad).
- **Banner "Keep Learning!"**: Gradien biru dengan pesan motivasi *"Your future starts with today's progress"*, tombol CTA *"Continue Learning ->"*, dan artwork 3D tumpukan buku bertopi toga (`assets/books-cap.svg`).
- **4 Kartu Metrik Cepat**:
  - `04 Courses` (Ikon buku biru)
  - `12 Lessons` (Ikon play ungu)
  - `85% Progress` (Ikon chart tren cyan)
  - `03 Certificates` (Ikon piala gold)
- **Continue Learning**: Kartu resume pembelajaran horizontal dengan *progress bar* interaktif 75% tuntas dan tombol *Continue*.
- **Rekomendasi Kursus**: Rekomendasi kursus personal untuk siswa.

### 3. Halaman Pembelajaran (Classroom & Player)
- **Navigasi Atas**: Tombol `← Kembali ke Kursus` dan status modul kursus.
- **Video Player Interaktif**:
  - Tampilan video 16:9 dengan overlay tombol Play besar.
  - Kontrol kustom lengkap: Play/Pause, timeline scrubber yang dapat di-klik untuk menggeser durasi (0:00 / 12:45), volume/mute, selector kecepatan putar (1x, 1.25x, 1.5x, 2x), dan fullscreen.
- **Informasi Materi**: Judul materi *"Prinsip Desain"*, deskripsi pembelajaran, tombol solid biru *"✓ Mark as Complete"*, tombol ungu *"⚡ Start Quiz"*, serta tombol navigasi *"← Sebelumnya"* dan *"Selanjutnya →"*.
- **Tab Belajar Interaktif**:
  - *Catatan Siswa*: Menyimpan catatan materi otomatis ke memori lokal browser (`localStorage`).
  - *Ringkasan Materi*: Poin-poin intisari konsep desain (Hierarki, Konsistensi, Umpan Balik).
  - *Tanya AI Assistant*: Simulasi asisten AI edukasi yang siap menjawab pertanyaan seputar materi.
- **Daftar Materi (Kurikulum Playlist)**:
  1. *1. Pengenalan UI/UX* (Badge: `✓ Selesai`)
  2. *2. Prinsip Desain* (Badge: `▶ Sedang Dipelajari`)
  3. *3. Wireframing* (Badge: `Belum Selesai`)
  4. *4. Prototyping* (Badge: `Belum Selesai`)
  5. *5. Studi Kasus* (Badge: `Belum Selesai`)

### 4. Katalog Kursus (Explore Courses)
- Judul *"Jelajahi Kursus"* dan subjudul informatif.
- Toolbar filter pencarian seketika (*real-time debounce search*), pil kategori dinamis (*Semua, Programming, Design, Marketing, Business*), dan dropdown pengurutan (*Terpopuler, Rating Tertinggi, Materi Terbanyak, Nama A-Z*).
- Grid kursus kaya informasi dengan thumbnail vektor 3D, instruktur, jumlah materi, rating bintang, dan tombol *"View Course"*.

### 5. Dashboard Admin (Admin Panel)
- **Sidebar Khusus Admin**: Menu *Overview, Users, Courses, Categories, Lessons, Quizzes, Reports, Settings*.
- **3 KPI Stat Cards**:
  - `12.5K Total Users`
  - `245 Total Courses`
  - `98.5% Completion Rate`
- **Aktivitas Pengguna (Chart.js)**: Grafik garis dinamis dengan kurva halus (*smooth tension*) dan gradien biru transparan menampilkan tren pertumbuhan pengguna dari Januari hingga Juni.
- **Pengguna Terbaru (Recent Activity Feed)**: Daftar aktivitas real-time:
  - *Siti Aisyah* (2 menit lalu - Online)
  - *Rizki Pratama* (5 menit lalu - Akun Baru)
  - *Dewi Lestari* (10 menit lalu - Lulus Kuis 100)
  - *Budi Santoso* (15 menit lalu - Sertifikat Diterbitkan)
- **Tabel Manajemen Kursus (CRUD)**: Admin dapat menambahkan kursus baru via modal formulir, mengubah data kursus, dan menghapus kursus dengan sinkronisasi langsung ke katalog publik.

### 6. Desain Responsif (Mobile Preview)
- Menampilkan 3 simulasi mockup frame ponsel cerdas interaktif yang persis dengan ilustrasi panel 6 di gambar:
  1. *Mobile: Landing Page* (Navigasi ringkas, hero mobile, kursus populer)
  2. *Mobile: Dashboard Siswa* (Kartu sapaan Ahmad, kartu keep learning, 2x2 grid statistik)
  3. *Mobile: Halaman Pembelajaran* (Mobile player, mark as complete, navigasi sebelumnya/selanjutnya)
- Seluruh antarmuka web juga dirancang **fully responsive** pada layar ponsel, tablet, laptop, dan monitor desktop sebenarnya!

---

## ⚡ Fitur Utama Tambahan (Interactive Modals)

1. **Kuis Interaktif & Gamifikasi**:
   - 5 pertanyaan konsep desain UI/UX sebenarnya.
   - Timer hitung mundur 10:00 otomatis.
   - Evaluasi jawaban instan, penilaian skor (0-100), dan letusan konfeti perayaan (*confetti canvas*) saat siswa lulus (skor >= 80).
2. **HTML5 Canvas Certificate Generator**:
   - Menghasilkan sertifikat kelulusan resmi beresolusi tinggi (900x600 px) secara dinamis atas nama siswa (**Ahmad**), nama kursus, nomor verifikasi resmi, dan cap segel emas *Verified*.
   - Tombol **Unduh PNG (HD)** dan **Cetak / Print**.
3. **Autentikasi & Multi-Role Switching**:
   - Modal Login & Registrasi dengan tab peralihan.
   - Tombol cepat 1-klik untuk beralih antara peran **Ahmad (Siswa)** dan **Siti Aminah (Admin)**.

---

## 📁 Struktur Berkas Proyek

```
EduFlex-App/
├── index.html                 # Halaman aplikasi utama (SPA) dengan seluruh 6 tampilan
├── style.css                  # Desain sistem CSS modern, clean, minimalis, dan responsif
├── script.js                  # Logika interaktif, state management, kuis, sertifikat, & chart
├── README.md                  # Dokumentasi proyek lengkap
└── assets/                    # Aset grafis vektor 3D murni (SVG)
    ├── logo.svg               # Logo EDUFLEX biru
    ├── logo-white.svg         # Logo EDUFLEX putih untuk sidebar gelap
    ├── hero-student.svg       # Ilustrasi 3D siswa laptop & graduation cap
    ├── books-cap.svg          # Ilustrasi 3D tumpukan buku & topi wisuda
    ├── course-uiux.svg        # Ilustrasi kartu UI/UX Design Fundamentals
    ├── course-web.svg         # Ilustrasi kartu Web Development Basics
    ├── course-marketing.svg   # Ilustrasi kartu Digital Marketing Strategy
    ├── course-python.svg      # Ilustrasi kartu Python for Beginners
    ├── course-graphic.svg     # Ilustrasi kartu Graphic Design Essentials
    └── course-business.svg    # Ilustrasi kartu Financial Modeling & Business
```

---

## 🚀 Cara Menjalankan Proyek

1. **Buka Langsung di Browser**:
   - Cukup klik dua kali berkas `index.html` yang berada di dalam folder `EduFlex-App`, atau klik kanan lalu pilih **Open with Google Chrome / Microsoft Edge**.
2. **Menggunakan VS Code Live Server**:
   - Buka folder `EduFlex-App` di VS Code.
   - Klik kanan pada `index.html` dan pilih **Open with Live Server**.
   - Buka `http://127.0.0.1:5500/EduFlex-App/index.html`.
3. **Melalui Python Simple HTTP Server**:
   ```bash
   cd EduFlex-App
   python -m http.server 8080
   ```
   Buka peramban di `http://localhost:8080`.
