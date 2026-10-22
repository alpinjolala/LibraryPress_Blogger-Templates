# PustakaKu - Template Blogger Web Perpustakaan Sekolah

**PustakaKu** adalah template Blogger responsif dan modern yang dirancang khusus untuk website perpustakaan sekolah. Dilengkapi dengan desain antarmuka yang bersih (biru & oranye), mode gelap (dark mode), integrasi pencarian OPAC (Online Public Access Catalog), dan manajemen koleksi buku berbasis label Blogger.

Dibuat oleh: **Muhammad Alfin Ramadhan, M.A.**

Versi: **1.0.0**

🔗 **[Lihat Demo Template PustakaKu](https://www.pustakaku.muhalfinramadhan.web.id/)**

## 📸 Cuplikan Tampilan (Screenshots)

*Berikut adalah cuplikan antarmuka dari template PustakaKu:*

**Tampilan Utama / Hero Section**
![Header Depan](https://github.com/alpinjolala/PustakaKu_Blogger-Templates/blob/main/Header_Depan.png)

**Dashboard Utama**
![Dashboard](https://github.com/alpinjolala/PustakaKu_Blogger-Templates/blob/main/Dashboard.png)

**Tampilan Jelajah Koleksi & Slider Buku**
![Jelajahi Koleksi](https://github.com/alpinjolala/PustakaKu_Blogger-Templates/blob/main/Jelajahi%20Koleksi.png)

## ✨ Fitur Utama

* **Desain Modern & Responsif:** Tampil sempurna di desktop, tablet, dan smartphone.
* **Mode Gelap (Dark Mode):** Dilengkapi tombol *toggle* dengan penyimpanan preferensi (Local Storage).
* **Integrasi Pencarian OPAC & Blog:** Form pencarian ganda (Tab) di halaman depan untuk mencari buku di katalog perpustakaan eksternal atau mencari artikel di blog.
* **Menu Navigasi Canggih:** Mendukung Sub-menu (Dropdown) dan Mega Menu berbasis Label.
* **Koleksi Buku & Slider:** Tampilan ala rak buku untuk label koleksi dengan fitur *swipe/scroll* horizontal.
* **Statistik Perpustakaan Animatif:** Angka statistik yang menghitung otomatis saat di-scroll (Reveal on scroll).
* **SEO & Meta Tags Ready:** Otomatis menghasilkan meta *Open Graph* dan *Twitter Card*.
* **Widget Jam Layanan Dinamis:** Menampilkan status "Buka/Tutup" secara *real-time* berdasarkan hari dan jam.
* **Tombol Berbagi (Share):** WhatsApp, Facebook, X (Twitter), Telegram, dan Salin Tautan.
* **Optimasi Kecepatan:** *Lazy load* gambar, ikon menggunakan SVG Sprite, dan kustomisasi CSS minimalis.
* **Slot Iklan Siap Pakai:** Tersedia area iklan di atas, dalam postingan, dan atas footer.
* **Halaman 404 Kustom:** Halaman error khusus jika link tidak ditemukan.

## 🚀 Panduan Instalasi

1. Login ke dasbor [Blogger](https://www.blogger.com).
2. Pilih blog perpustakaan Anda.
3. Masuk ke menu **Tema (Theme)**.
4. Klik tombol ikon panah ke bawah di sebelah tombol *Sesuaikan* (Customize), lalu pilih **Pulihkan (Restore)**.
5. Klik **Upload** dan pilih file `PustakaKu-Perpustakaan-Sekolah.xml`.
6. Tunggu hingga proses upload selesai.

> **Penting:** Pastikan untuk mengatur **Setelan -> Format -> Zona Waktu** ke Waktu Indonesia Barat/Tengah/Timur agar widget Jam Layanan berfungsi akurat.

## ⚙️ Panduan Pengaturan Widget

Template ini menggunakan pengaturan standar Widget Blogger yang dimodifikasi. Anda dapat mengaturnya melalui menu **Tata Letak (Layout)**.

### 1. Mengatur Sub-menu & Mega Menu (Widget Menu Utama)

Buka widget **LinkList** bernama `Menu Utama`. Format penulisan namanya adalah:

* `Nama Menu`: Menu biasa.
* `_Nama Sub`: Tambahkan 1 garis bawah (`_`) untuk membuat dropdown.
* `__Nama Sub Sub`: Tambahkan 2 garis bawah (`__`) untuk dropdown bertingkat.
* **Mega Menu:** Tulis URL dengan format `mega:NamaLabel` (contoh: URL diisi `mega:Koleksi`).

### 2. Mengatur URL Pencarian OPAC (Katalog Buku)

Agar tab pencarian "Katalog Buku" berfungsi dan mengarah ke sistem OPAC perpustakaan Anda (misal: SLiMS/InlisLite):

1. Buka Tata Letak.
2. Edit widget HTML bernama **"URL Pencarian OPAC"** (di bawah bagian Hero).
3. Masukkan URL *Base Search* OPAC Anda. Contoh untuk SLiMS: `https://opac.sekolah.sch.id/index.php?search=search&keywords=`
4. Jika dibiarkan kosong, tab OPAC akan otomatis disembunyikan.

### 3. Mengatur Slider "Koleksi Buku Terbaru"

1. Edit widget HTML bernama **"Koleksi Buku Terbaru"**.
2. Pada bagian **Konten (Content)**, isikan **nama label** yang ingin ditampilkan (misal: `Koleksi` atau `Buku Baru`).
3. Template otomatis memuat postingan dengan label tersebut dan menampilkan gambar pertamanya (rasio 2:3) sebagai cover buku.

### 4. Mengatur Jam Layanan Dinamis (Widget Sidebar)

Widget ini menggunakan atribut data HTML untuk mengecek status buka/tutup.

1. Edit widget HTML bernama **"Jam Layanan"** di Sidebar.
2. Perhatikan kode: `data-schedule="1,2,3,4|07:30-16:00;5|07:30-16:30;6|08:00-12:00"`
   * `1,2,3,4` = Hari Senin - Kamis (0 = Minggu)
   * `07:30-16:00` = Jam buka dan tutup.
3. Sesuaikan teks dan angka tersebut sesuai jam operasional perpustakaan Anda.

### 5. Mengubah Warna Tema

Anda tidak perlu mengedit kode CSS. Cukup buka menu **Tema -> Sesuaikan (Customize)**:

* Pilih menu **Lanjutan (Advanced)**.
* Anda bisa mengubah Warna Primer (Biru), Warna Aksen (Oranye), dan warna latar lainnya melalui *Theme Designer Options*.

## 📝 Aturan Penulisan Postingan Buku

Agar postingan buku tampil optimal (seperti buku dengan cover):

1. Upload gambar sampul/cover buku sebagai gambar **pertama** di dalam postingan. (Disarankan rasio gambar potret/berdiri).
2. Tambahkan **Label** khusus seperti `Koleksi`, `Fiksi`, atau `Buku Pelajaran` agar masuk ke dalam grid kategori atau slider.
3. Jika menulis artikel berita biasa, hindari menggunakan label khusus buku tersebut agar bentuk halamannya menyesuaikan artikel standar.

## 📜 Lisensi & Hak Cipta

Template ini dibuat oleh [Muhammad Alfin Ramadhan, M.A.](https://www.muhalfinramadhan.web.id)

Dilarang menjual template ini tanpa izin dari pembuat. Anda bebas menggunakannya untuk website instansi atau sekolah Anda. Salah satu bentuk menghargai adalah dengan tidak menghapus atribusi atau copyright pada footer blogger Anda.

Dibuat dengan ❤️ untuk meningkatkan literasi sekolah di Indonesia.
