# Portfolio Website Profesional

Website portfolio profesional untuk melamar pekerjaan. Website ini dibuat dengan HTML, CSS, dan JavaScript murni tanpa framework, sehingga ringan dan mudah di-deploy.

## Fitur

- ✅ Desain modern dan responsif
- ✅ Hero section dengan animasi typing
- ✅ Tentang saya dengan statistik
- ✅ Keahlian dengan progress bar animasi
- ✅ Timeline pengalaman kerja
- ✅ Showcase proyek
- ✅ Form kontak
- ✅ Navigasi mobile-friendly
- ✅ Smooth scroll dan animasi
- ✅ Social media links

## Cara Menjalankan di Localhost

### Opsi 1: Menggunakan Python (Rekomendasi)

1. Pastikan Python terinstal di komputer Anda
2. Buka terminal/command prompt di folder ini
3. Jalankan perintah:
   ```bash
   python -m http.server 8000
   ```
4. Buka browser dan akses: `http://localhost:8000`

### Opsi 2: Menggunakan Node.js

1. Install http-server globally:
   ```bash
   npm install -g http-server
   ```
2. Jalankan server:
   ```bash
   http-server -p 8000
   ```
3. Buka browser dan akses: `http://localhost:8000`

### Opsi 3: Menggunakan VS Code Live Server

1. Install ekstensi "Live Server" di VS Code
2. Klik kanan pada `index.html`
3. Pilih "Open with Live Server"

## Cara Deploy ke Google Sites

### Metode 1: Menggunakan Google Sites (Embed)

1. **Upload file ke hosting gratis**
   - Upload folder `PORTOFOLIO` ke Netlify, Vercel, atau GitHub Pages
   - Atau gunakan layanan seperti Tiiny.host atau Surge.sh

2. **Buat Google Sites**
   - Buka [sites.google.com](https://sites.google.com)
   - Klik "Blank" untuk membuat site baru
   - Beri nama site Anda

3. **Embed Website**
   - Di Google Sites, klik "Insert" → "Embed"
   - Pilih "Embed Code"
   - Masukkan kode iframe:
   ```html
   <iframe src="URL_WEBSITE_ANDA" width="100%" height="600" frameborder="0"></iframe>
   ```
   - Ganti `URL_WEBSITE_ANDA` dengan URL dari hosting Anda

### Metode 2: Menggunakan Google Sites (Manual Copy)

1. **Copy konten HTML**
   - Buka `index.html` di text editor
   - Copy konten di dalam `<body>` tag

2. **Paste ke Google Sites**
   - Di Google Sites, buka halaman baru
   - Paste konten HTML
   - Google Sites akan otomatis format kontennya

3. **Upload CSS dan JS**
   - Untuk styling dan interactivity penuh, disarankan menggunakan metode embed di atas

### Metode 3: Deploy ke Netlify (Paling Mudah)

1. Buka [app.netlify.com](https://app.netlify.com)
2. Sign up atau login
3. Drag and drop folder `PORTOFOLIO` ke Netlify
4. Website akan langsung live dengan URL gratis
5. Copy URL dan gunakan di Google Sites atau share langsung

### Metode 4: Deploy ke GitHub Pages

1. Buat repository baru di GitHub
2. Upload file-file portfolio ke repository
3. Go to Settings → Pages
4. Pilih branch `main` dan folder `/root`
5. Website akan live di `username.github.io/repository-name`

## Kustomisasi

### Ganti Informasi Pribadi

Edit file `index.html` dan ganti placeholder:

- `[Nama Anda]` - Nama lengkap Anda
- `[Nama Perusahaan]` - Nama perusahaan tempat Anda bekerja
- `email@example.com` - Email Anda
- `+62 812 3456 7890` - Nomor telepon
- `[Kota, Negara]` - Lokasi Anda
- Link social media di bagian `href="#"`

### Ganti Foto Profil

1. Siapkan foto profil Anda
2. Simpan di folder `PORTOFOLIO` dengan nama `profile.jpg`
3. Di `index.html`, ganti:
   ```html
   <div class="profile-placeholder">
       <i class="fas fa-user"></i>
   </div>
   ```
   dengan:
   ```html
   <img src="profile.jpg" alt="Profile" class="profile-image">
   ```
4. Di `styles.css`, tambahkan:
   ```css
   .profile-image {
       width: 350px;
       height: 350px;
       border-radius: 50%;
       object-fit: cover;
       border: 5px solid rgba(255, 255, 255, 0.3);
   }
   ```

### Ganti Gambar Proyek

Untuk setiap proyek di section `#projects`:

1. Siapkan screenshot proyek
2. Simpan di folder `PORTOFOLIO/images/`
3. Di `index.html`, ganti placeholder dengan:
   ```html
   <img src="images/project1.jpg" alt="Project Name">
   ```

### Ubah Warna Tema

Di `styles.css`, ubah variabel CSS di `:root`:

```css
:root {
    --primary-color: #2563eb;    /* Warna utama */
    --secondary-color: #1e40af;  /* Warna sekunder */
    --accent-color: #3b82f6;     /* Warna aksen */
}
```

### Tambah/Ubah Keahlian

Di `index.html`, edit section `.skills-grid` untuk menambah atau mengubah skill cards.

### Tambah/Ubah Pengalaman

Di `index.html`, edit section `.timeline` untuk menambah atau mengubah timeline items.

### Tambah/Ubah Proyek

Di `index.html`, edit section `.projects-grid` untuk menambah atau mengubah project cards.

## Struktur File

```
PORTOFOLIO/
├── index.html          # Halaman utama
├── styles.css          # Styling
├── script.js           # JavaScript untuk interaktivitas
├── README.md           # Dokumentasi ini
└── images/             # Folder untuk gambar (opsional)
    ├── profile.jpg
    ├── project1.jpg
    └── project2.jpg
```

## Tips untuk Melamar Kerja

1. **Customize untuk setiap lamaran** - Sesuaikan portfolio dengan posisi yang dilamar
2. **Highlight proyek relevan** - Tampilkan proyek yang sesuai dengan job description
3. **Tambahkan link ke live demo** - Pastikan proyek bisa diakses dan dicoba
4. **Include contact information yang jelas** - Memudahkan recruiter menghubungi Anda
5. **Test di berbagai browser** - Pastikan tampilan konsisten
6. **Optimize untuk mobile** - Banyak recruiter melihat portfolio di mobile
7. **Keep it updated** - Update portfolio secara berkala dengan proyek terbaru

## Support

Jika mengalami masalah atau pertanyaan, silakan cek:
- Dokumentasi HTML/CSS/JavaScript
- Forum komunitas web development
- Dokumentasi platform hosting yang digunakan

## License

Website ini dibuat untuk penggunaan pribadi dalam melamar pekerjaan. Silakan dimodifikasi sesuai kebutuhan.
