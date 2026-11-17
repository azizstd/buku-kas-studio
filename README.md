# 📐 Buku Kas Studio & Proyek Arsitektur

Aplikasi manajemen keuangan kas terintegrasi untuk studio arsitektur, interior, dan kontraktor. Dibuat murni dengan **HTML5, CSS3, dan Vanilla JavaScript** tanpa dependensi backend atau framework berat, sehingga cepat, ringan, aman, dan dapat dijalankan langsung di peramban web (*browser*).

Mendukung tampilan responsif penuh untuk **Smartphone (iOS & Android)**, **Tablet**, hingga **Desktop**.

---

## ✨ Fitur Utama

### 🏢 1. Kas Besar Studio
- **Dashboard Ringkasan Eksekutif**: Pantau total saldo studio, saldo kas tunai, saldo non-tunai (bank), serta dana yang tersebar di proyek secara *real-time*.
- **Spending Overview (Donut Chart)**: Analisis komposisi pengeluaran proyek berdasarkan jenis pekerjaan dengan diagram donat interaktif.
- **Kontrol Keseimbangan Rekening (Anti-Nombok)**: Fitur rekonsiliasi untuk membandingkan saldo catatan buku dengan saldo fisik asli di rekening bank/dompet kas, lengkap dengan indikator selisih (Kurang, Pas, Lebih).
- **Riwayat Transaksi Kas Besar**: Pencatatan termin klien, modal drop proyek, dan biaya operasional studio.

### 🔨 2. Kas Kecil Operasional Proyek
- **Multi-Proyek**: Pengelolaan banyak proyek arsitektur/interior secara terpisah.
- **Mode Pengelolaan Fleksibel**:
  - *Dikelola Sendiri*: Kasir lapangan langsung dikontrol oleh tim studio.
  - *Dikelola PIC*: Pemantauan dana yang ditransfer ke PIC/mandor di lapangan, laporan pemakaian, serta sisa pertanggungjawaban dana.
- **Dana Talangan Pribadi**: Pencatatan uang pribadi pemilik/tim yang ditalangkan untuk proyek, dan pelacakan penggantian dari kas studio.
- **Indikator Realisasi Belanja (Burn Rate)**: Visualisasi progres persentase anggaran proyek yang telah terpakai.
- **Diagram Pengeluaran per Jenis Pekerjaan**: Visualisasi batang horizontal rincian belanja (Pekerjaan Persiapan, Struktur, Arsitektur, Interior, MEP, Landscape, Operasional, dll.).

### ⚖️ 3. Manajemen Kasbon Tukang & Kalkulator Upah Sabtu
- **Pelacakan Kasbon Aktif**: Mencatat kasbon harian mandor dan tukang agar tidak terlupa saat hari gajian.
- **Kalkulator Potong Kasbon Otomatis**: Menghitung otomatis upah bersih mingguan setelah dipotong kasbon, dengan dukungan pelunasan bertahap (sebagian) atau lunas penuh.

### 📱 4. Desain Responsif Mobile-First
- **Off-Canvas Sidebar Drawer**: Menu navigasi samping meluncur halus dari sisi kiri dengan *backdrop blur*.
- **Bottom Navigation Bar**: Navigasi bawah ramah sentuhan jempol di smartphone (Kas Besar, Proyek, Tombol Tambah Transaksi, Riwayat, Menu).
- **iOS & Android Optimized**: Mencegah *auto-zoom* saat mengetik form di Safari iOS, serta mendukung safe-area (*notch* / *home indicator*).
- **Mode Gelap (Dark Mode) & Terang (Light Mode)**: Tombol ganti tema yang nyaman di mata untuk pemakaian siang maupun malam di lapangan.

### 💾 5. Impor, Ekspor, dan Cadangan Data
- **Smart Append Import Excel**: Impor file `.xlsx`, `.xls`, atau `.csv` tanpa menghapus data yang sudah ada (baris lama otomatis dilewati untuk mencegah duplikasi).
- **Ekspor Excel Lengkap**: Mengunduh seluruh rekapitulasi proyek, buku kas besar, dan buku kasbon ke dalam satu file Excel multi-sheet.
- **Pencadangan JSON & Pengingat Mingguan**: Fitur simpan dan pulihkan (*backup & restore*) seluruh data studio ke file JSON lokal tanpa khawatir kehilangan data saat cache browser dibersihkan.

---

## 🚀 Cara Menjalankan

Tidak memerlukan instalasi Node.js, server web khusus, atau database backend:

1. Unduh atau clone repositori ini:
   ```bash
   git clone https://github.com/<username>/<nama-repo>.git
   ```
2. Buka file `index.html` langsung di browser favorit Anda (Google Chrome, Safari, Microsoft Edge, Firefox):
   - Klik ganda pada `index.html`, atau
   - Buka peramban dan seret file `index.html` ke dalam tab peramban.

---

## 🛠️ Teknologi yang Digunakan

- **HTML5 & CSS3**: Custom CSS Variables, Flexbox, Grid, dan Media Queries.
- **JavaScript (ES6+)**: Logika akuntansi kas kecil, rekonsiliasi, dan manipulasi DOM lokal.
- **LocalStorage API**: Penyimpanan data aman langsung di browser pengguna (offline-ready).
- **SheetJS (xlsx.full.min.js)**: Pemrosesan impor dan ekspor file spreadsheet Excel secara *client-side*.

---

## 📄 Lisensi

Proyek ini dirilis di bawah lisensi MIT. Silakan gunakan dan kembangkan sesuai kebutuhan studio Anda.
