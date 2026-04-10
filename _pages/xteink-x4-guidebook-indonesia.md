---
layout: default
title: Panduan XTEInk X4
permalink: /xteink-x4/
nav_order: 2
---

# XTEInk X4 Guidebook Indonesia: Panduan Lengkap Pemilik

**XTEInk X4 adalah e-reader saku ultra-tipis seharga ~$58 USD dengan layar E-Ink 4.3 inci, tanpa touchscreen, dan dioperasikan sepenuhnya dengan tombol fisik.** Perangkat ini dirancang untuk ditempel di belakang smartphone via magnet MagSafe, menjadikannya pendamping baca yang selalu siap di saku. Panduan ini ditulis khusus untuk pembeli di Indonesia — mulai dari setup awal, transfer buku, hingga tips perawatan di iklim tropis.

---

## 1. Quick start: dari unboxing sampai baca buku pertama

### Isi dalam kotak

Saat membuka paket XTEInk X4, Anda akan menemukan: unit e-reader X4, quick start guide, **microSD card** (16GB atau 32GB tergantung batch), screen protector, dan 2 magnetic stick-on ring untuk menempel di smartphone. Pembelian dari situs resmi biasanya menyertakan adapter microSD ke USB sebagai bonus.

### Langkah setup awal

**Charge dulu.** Hubungkan X4 ke sumber daya via kabel USB-C (kabel tidak termasuk — gunakan kabel USB-C standar). Pengisian penuh membutuhkan **2–3 jam**, dan baterai 650mAh mampu bertahan hingga **14 hari** dengan pemakaian 1–3 jam per hari. Indikator baterai ditampilkan sebagai ikon di layar.

Masukkan microSD card ke slot di sisi kiri perangkat — dorong perlahan sampai terdengar bunyi klik. Pastikan kartu dalam format **exFAT** (bukan FAT32 atau NTFS). Nyalakan perangkat dengan menekan dan menahan tombol Power selama beberapa detik.

### Mengganti bahasa dari Chinese ke English

Perangkat yang dibeli dari AliExpress biasanya menggunakan bahasa Mandarin secara default. Berikut cara mengubahnya:

1. Nyalakan X4 dan pastikan Anda di **home screen**
2. Navigasi ke ikon **齿轮/gear** (设置 / Settings) menggunakan tombol Previous/Next
3. Tekan tombol **OK** — opsi bahasa adalah **item pertama** yang sudah terpilih
4. Tekan **OK** lagi untuk mengubah bahasa ke **English**
5. Selesai — antarmuka langsung berubah ke bahasa Inggris

Alternatif: flash firmware internasional via https://xteink.dve.al/ menggunakan browser Chrome untuk mendapatkan font support yang lebih baik.

### Koneksi WiFi

Dari home screen, navigasi ke **Sync → Network Connection**. Pilih jaringan WiFi Anda (hanya mendukung **2.4 GHz** — jaringan 5 GHz tidak akan terdeteksi). Masukkan password menggunakan navigasi tombol, lalu **tekan lama tombol Back** untuk menyimpan dan keluar. Setelah terhubung, lakukan update firmware melalui **Sync → System Update**.

### Peta tombol perangkat

XTEInk X4 memiliki **7 tombol fisik** tanpa touchscreen:

| Tombol | Lokasi | Fungsi |
|--------|--------|--------|
| **Power** | Sisi atas | Tekan singkat: sleep/wake. Tekan lama: on/off |
| **Previous Page** | Rocker kanan atas | Halaman sebelumnya / navigasi menu ke atas |
| **Next Page** | Rocker kanan bawah | Halaman berikutnya / navigasi menu ke bawah |
| **Back** | Rocker kiri bawah | Kembali. Tekan lama: simpan & keluar |
| **OK/Confirm** | Rocker kiri kanan | Konfirmasi pilihan. Double-tap saat baca: buka menu reader. Tekan lama: bookmark |
| **Reset** | Sisi kiri (lubang kecil) | Hard reset dengan pin/penjepit kertas |

Saat membaca, tombol Previous/Next membalik halaman. Double-tap OK membuka menu reader yang berisi: pengaturan font, auto-flip, navigasi chapter, dark mode, rotasi layar, bookmark, dan progress bar.

---

## 2. Format buku yang didukung dan mana yang paling optimal

### Format file yang didukung

| Firmware | Format Didukung |
|----------|----------------|
| **Stock** | EPUB, TXT, JPG, BMP, PNG |
| **CrossPoint** | EPUB 2/3, TXT, FB2, HTML, MD, XTC, XTCH, JPG, BMP, PNG |
| **Papyrix** | Semua format CrossPoint + FB2 (lebih baik), HTML, Markdown |

**Penting:** X4 **tidak mendukung PDF, MOBI, AZW3, atau CBZ secara native**. Semua format tersebut harus dikonversi terlebih dahulu.

### Ranking format terbaik untuk layar 4.3 inci

**XTC/XTCH adalah format paling optimal** karena setiap halaman sudah di-render tepat di resolusi 480×800 piksel — halaman berganti instan dan formatting sempurna. XTC menggunakan 1-bit monokrom (hitam-putih murni), sedangkan XTCH menggunakan 2-bit grayscale (4 level abu-abu) untuk konten dengan gradasi warna.

EPUB menjadi pilihan terbaik kedua untuk novel, karena teks bisa mengalir ulang (reflow) menyesuaikan ukuran layar — sangat ideal untuk layar kecil. Gunakan Calibre untuk mengoptimasi EPUB: hapus CSS kompleks, hapus font embedded, resize gambar ke maksimal 480px lebar.

TXT berfungsi baik untuk dokumen sederhana tanpa formatting. PDF sebaiknya **selalu dikonversi** ke EPUB atau XTC karena layout halaman standar PDF akan terlalu kecil di layar 4.3 inci dan tidak bisa di-zoom (tidak ada touchscreen).

### Tool konversi penting

- **Calibre** (https://calibre-ebook.com/) — konversi dari MOBI, AZW, DOCX, PDF ke EPUB
- **XTC.js** (https://xtcjs.app) — konversi CBZ, PDF, gambar ke format XTC/XTCH via browser
- **EPUB2XTC** (https://epub2xtc.com) — konverter resmi Xteink dari EPUB/PDF ke XTC

---

## 3. Empat cara transfer buku ke XTEInk X4

### Metode 1: Via microSD card reader (tercepat dan paling andal)

USB-C pada X4 **hanya untuk charging — tidak mendukung transfer data USB**. Metode microSD card reader adalah cara paling cepat dan stabil.

1. **Matikan** X4 dan **keluarkan microSD card** (tekan hingga klik, kartu akan sedikit keluar)
2. **Masukkan kartu** ke USB card reader, hubungkan ke komputer
3. **Salin file** EPUB, TXT, atau XTC ke kartu — bisa langsung di root directory atau dalam subfolder terorganisir (misal: `Fiksi/`, `NonFiksi/`, `Manga/`)
4. **Safely eject** kartu dari komputer
5. **Masukkan kembali** ke X4 dan nyalakan — perangkat akan otomatis mendeteksi buku baru

**Tips:** Batasi **100–200 file per folder** untuk navigasi yang lancar. Ganti microSD bawaan dengan kartu bermerek seperti **SanDisk 128–256GB** karena kartu bawaan diketahui sering bermasalah dan panas.

### Metode 2: Via WiFi transfer

X4 membuat **hotspot WiFi sendiri** untuk transfer file:

1. Di home screen, pilih **Sync → Other Transfer Methods**
2. X4 akan membuat hotspot bernama **"E-Paper"**
3. Di HP/laptop, hubungkan ke WiFi **"E-Paper"** dengan password **`12345678`**
4. Buka browser, akses **`192.168.3.3`**
5. Pilih **File Management**, lalu upload file buku Anda

Kecepatan transfer via WiFi relatif lambat (~10MB per 30 detik). Gunakan metode ini hanya untuk transfer 1–2 file kecil. Untuk transfer batch, gunakan microSD card reader.

### Metode 3: Via aplikasi companion

Beberapa aplikasi companion tersedia untuk memudahkan transfer:

**Send to X4** (pihak ketiga, gratis, open-source) adalah yang paling populer. Tersedia di iOS (https://apps.apple.com/us/app/send-to-x4/id6758729873), Android (https://play.google.com/store/apps/details?id=com.chapiware.sendtox4), dan sebagai extension browser Firefox/Chrome. Aplikasi ini bisa mengirim EPUB, mengkonversi artikel web jadi EPUB, membuat custom wallpaper, dan mengelola file di X4 — semuanya via koneksi WiFi lokal tanpa cloud.

**Aplikasi resmi Xteink** tersedia di iOS untuk perangkat dengan firmware XT V5.0.3+. Bisa mengirim buku dan otomatis mengkonversi MOBI/PDF ke format yang didukung. Download di https://www.xteink.com/pages/xteink-apps.

**Hojo** (https://github.com/meta-boy/hojo) adalah companion Android tidak resmi yang menyediakan fitur konversi EPUB, file manager, dan wallpaper editor.

### Metode 4: Via Calibre (membutuhkan CrossPoint firmware)

Calibre bisa mengirim buku langsung ke X4 secara wireless dengan plugin CrossPoint:

1. Install **CrossPoint firmware** di X4 (lihat Bagian 6)
2. Download plugin Calibre dari https://github.com/crosspoint-reader/calibre-plugins/releases
3. Di Calibre: **Preferences → Plugins → Load plugin from file** → pilih file .zip plugin
4. Di X4: masuk ke **File Transfer → Connect to Calibre → Join a network**
5. Pastikan komputer dan X4 di **jaringan WiFi yang sama**
6. Di Calibre, klik **"Send to device"** untuk transfer buku secara wireless

Alternatif: CrossPoint juga mendukung **OPDS browser** — bisa mengakses Calibre Content Server langsung dari X4 dengan URL format `http://[IP-komputer]:8080/opds`.

---

## 4. Membaca berbagai jenis konten

### Membaca novel/ebook

Format EPUB adalah pilihan utama untuk novel. Pada **stock firmware**, opsi font terbatas pada small dan medium saja, dan formatting seperti italic/bold sering tidak tampil dengan benar. Pada **CrossPoint firmware**, pengalaman membaca jauh lebih baik: tersedia 4 ukuran font (S/M/L/XL), line spacing bisa diatur, margin layar bisa dikustomisasi, dan teks bisa di-justify.

Fitur reading yang tersedia: auto-flip (interval 0–9 detik), navigasi chapter, dark mode, bookmark (tekan lama OK), dan progress bar. Perangkat mendukung rotasi layar 4 arah dan kompatibel dengan Bluetooth page turner eksternal.

### Membaca PDF

**PDF tidak didukung secara native** dan layar 4.3 inci terlalu kecil untuk layout PDF standar. Solusinya adalah konversi:

- **PDF berbasis teks:** Konversi ke EPUB via Calibre, lalu transfer ke X4
- **PDF scan/gambar:** Konversi ke format XTC menggunakan XTC.js (https://xtcjs.app) — tool ini mengoptimasi setiap halaman ke resolusi tepat 480×800 dengan opsi dithering untuk gambar
- **Aplikasi resmi Xteink** juga bisa auto-convert PDF ke format yang didukung saat transfer

### Membaca komik dan manga

X4 tidak mendukung CBZ/CBR secara native, tapi komunitas telah membangun tool konversi yang sangat baik:

1. **Konversi CBZ/CBR/PDF ke XTC** menggunakan **XTC.js** (https://xtcjs.app) — tool browser gratis dengan fitur smart dithering, page splitting untuk spread dua halaman, dan optimasi otomatis ke resolusi 480×800
2. **cbz2xtc** (https://github.com/tazua/cbz2xtc) — tool command-line untuk batch convert manga

Untuk manga hitam-putih, gunakan format **XTC** tanpa dithering atau dengan Floyd-Steinberg dithering. Untuk komik dengan gradasi warna, gunakan **XTCH** (2-bit grayscale). Aktifkan fitur **page splitting** untuk memecah halaman landscape menjadi dua halaman portrait terpisah. Navigasi panel menggunakan tombol page-turn — tidak ada fitur zoom panel-by-panel.

---

## 5. Custom wallpaper dan sleep screen

### Cara mengganti wallpaper

**Metode paling mudah (rotating wallpaper):** Buat folder bernama **`sleep/`** di root directory microSD card, lalu masukkan semua gambar dalam format **.BMP** ke folder tersebut. Di pengaturan X4, ubah **Sleep Screen** ke **"CUSTOM"**. Setiap kali perangkat sleep, gambar dipilih secara acak dari folder ini.

**Metode single wallpaper:** Simpan file bernama **`sleep.bmp`** di root directory microSD card. Atau melalui menu: **Settings → Power-off Screen → Custom → pilih gambar → tekan lama Confirm**.

### Spesifikasi gambar optimal

| Parameter | Nilai |
|-----------|-------|
| **Resolusi** | 480 × 800 piksel |
| **Rasio aspek** | 3:5 |
| **Format** | BMP (wajib untuk sleep screen) |
| **Kedalaman warna** | 8-bit grayscale (direkomendasikan) |

### Sumber wallpaper komunitas

**basvanderploeg.nl/xteink/** (https://basvanderploeg.nl/xteink/) adalah situs komunitas oleh desainer Belanda Bas van der Ploeg yang menyediakan koleksi sleep screen kustom berkualitas tinggi, termasuk Pokédex Wallpaper Generator di https://basvanderploeg.nl/xteink/pokemon/ yang menghasilkan wallpaper BMP 480×800 bertema Pokémon.

Aplikasi **Send to X4** menyertakan **Sleep Screen Designer** dengan 1.000+ wallpaper e-ink terkurasi yang bisa langsung dikirim ke perangkat. Halaman resmi Xteink Playground (https://www.xteink.com/pages/more-fun-with-xteink) juga menyediakan wallpaper bertema seasonal. Komunitas Reddit r/xteinkereader dan r/xteink juga aktif berbagi wallpaper kustom.

---

## 6. Custom firmware: CrossPoint, CrossPet, dan Papyrix

Firmware kustom adalah **upgrade terpenting** yang bisa Anda lakukan pada XTEInk X4. Stock firmware memiliki keterbatasan serius — hanya mendukung 2 ukuran font, formatting EPUB buruk, dan tidak ada integrasi Calibre.

### CrossPoint — firmware kustom paling populer

**CrossPoint Reader** (https://github.com/crosspoint-reader/crosspoint-reader) adalah firmware open-source yang dikembangkan oleh Dave Allie dengan komunitas aktif (3.100+ stars di GitHub). Versi terbaru adalah **v1.1.1** (Februari 2026).

Keunggulan utama dibanding stock firmware: **4 ukuran font** (S/M/L/XL), rendering bold/italic yang benar, CSS support untuk EPUB, integrasi Calibre wireless, OPDS browser, custom sleep screen dengan cover buku, button remapping, KOReader sync, dan **sunlight fading fix** untuk model putih. UI tersedia dalam 8 bahasa termasuk Inggris, Spanyol, Prancis, dan Jerman.

**Cara install CrossPoint (step-by-step):**

1. Hubungkan X4 ke komputer via **USB-C** dan pastikan perangkat menyala
2. Buka **https://xteink.dve.al/** di browser **Chrome** (WebSerial diperlukan)
3. **BACKUP DULU:** Di bagian "Full flash controls", klik **"Save full flash"** — tunggu sekitar **25 menit** untuk backup lengkap. Simpan file `flash.bin` dengan aman
4. Scroll ke "OTA fast flash controls", klik **"Flash CrossPoint firmware"**
5. Tunggu proses flashing selesai
6. Tekan tombol **Reset** (lubang kecil di sisi kiri), lalu tekan lama **Power** untuk reboot

### CrossPet — virtual pet yang tumbuh seiring Anda membaca

**CrossPet** (https://github.com/trilwu/crosspet) adalah fork CrossPoint buatan developer Vietnam yang menambahkan fitur Tamagotchi berupa **ayam virtual** yang berevolusi dari telur ke dewasa seiring halaman yang Anda baca. Tersedia 3 personality: Scholar, Balanced, dan Wild berdasarkan konsistensi membaca Anda. CrossPet juga menyertakan **5 mini-game** (Chess, Gomoku, Sudoku, Tetris, 2048) dan kalender lunar Vietnam. Semua fitur reading CrossPoint tetap ada. Install via https://xteink.dve.al/ dengan cara yang sama.

### Papyrix — untuk pengguna yang butuh format lebih banyak

**Papyrix** (https://github.com/bigbag/papyrix-reader, v1.18.0) adalah fork CrossPoint oleh Pavel Liashkov yang menambahkan dukungan **FB2 (FictionBook)** yang lebih baik, custom font (konversi TTF/OTF ke format .epdfont), tema kustom, dan tool optimasi EPUB bawaan. Papyrix memerlukan **instalasi via command-line** menggunakan papyrix-flasher (https://github.com/bigbag/papyrix-flasher) — tidak ada web flasher seperti CrossPoint.

### Perbandingan singkat

- **CrossPoint:** Instalasi termudah (web flasher), komunitas terbesar, update terbanyak. Pilihan terbaik untuk sebagian besar pengguna
- **Papyrix:** Format file lebih banyak (FB2, HTML, MD), custom font support. Untuk pengguna teknis
- **CrossPet:** Gamifikasi membaca dengan virtual pet. Untuk pengguna yang ingin motivasi membaca tambahan

### Backup dan restore firmware

**Sebelum flash custom firmware, SELALU backup.** Buka https://xteink.dve.al/, klik "Save full flash" di bagian "Full flash controls", dan simpan file `flash.bin`. Proses backup memakan waktu ~25 menit.

**Untuk restore ke stock firmware:** Kembali ke https://xteink.dve.al/ dan flash firmware resmi dari menu yang tersedia. Atau kunjungi https://xteink.dve.al/debug dan klik "Swap boot partition" untuk beralih ke partisi OTA lama. Jika terjebak bootloop di CrossPoint: tekan Reset, lalu tahan tombol **Back + Power** bersamaan untuk boot paksa ke Home Screen. **ESP32-C3 hampir tidak mungkin brick permanen** karena ROM bootloader selalu bisa diakses via serial.

---

## 7. Troubleshooting masalah umum

### Device freeze/hang

Tekan tombol **Reset** (lubang kecil di sisi kiri, gunakan pin/penjepit kertas), lalu segera tekan lama **tombol Power** selama 3 detik. Jika menggunakan CrossPoint dan terjebak bootloop, tekan Reset lalu tahan **Back + Power** secara bersamaan.

### WiFi tidak connect

X4 **hanya mendukung WiFi 2.4 GHz** — pastikan router Anda tidak diset ke 5 GHz only. Password WiFi dengan spasi bisa menyebabkan masalah koneksi. Jika menggunakan hotspot HP, set nama hotspot ke "XT-EPD" dan aktifkan mode kompatibilitas (compatibility mode di iPhone, 2.4 GHz band di Android). Posisikan X4 dekat dengan router karena modul WiFi berdaya rendah.

### Buku tidak muncul setelah transfer

Penyebab paling umum: **microSD card tidak diformat exFAT**. Lakukan full format (bukan quick format) ke exFAT. Pastikan juga file dalam format yang didukung — stock firmware hanya membaca EPUB dan TXT. Jika kartu bawaan bermasalah (panas, error), ganti dengan kartu bermerek. Setelah update firmware, buka buku apapun → tekan OK → pilih **"Index"** untuk rebuild indeks.

### Ghosting di layar E-Ink

Ghosting (bayangan sisa dari gambar sebelumnya) adalah hal normal pada layar E-Ink. X4 melakukan full refresh (layar berkedip hitam sebentar) setiap ~30 halaman. Di CrossPoint firmware, Anda bisa mengatur **Refresh Frequency** ke setiap 1, 5, 10, 15, atau 30 halaman untuk mengurangi ghosting. Jika ghosting parah akibat panas, biarkan perangkat dingin di suhu ruangan — ini bukan kerusakan permanen.

### MicroSD card error

MicroSD card bawaan diketahui **berkualitas rendah** dan sering menyebabkan perangkat panas. Ganti dengan **SanDisk 128–256GB** (tersedia di Tokopedia/Shopee, ~Rp150–300 ribu). Format ulang ke **exFAT** dengan full format. Pastikan kartu terpasang dengan benar — dorong hingga terdengar bunyi klik.

### White model dan masalah UV (sunlight fading)

Model **Frost White** memiliki masalah unik: sinar UV menembus casing putih dan mengganggu chip driver IC layar E-Ink, menyebabkan **layar memudar saat terkena sinar matahari langsung**. Ini **bukan kerusakan permanen** — refresh layar mengembalikannya ke normal. Tiga solusi: install **CrossPoint firmware** dan aktifkan **"Sunlight Fading Fix"** di settings (menambah tegangan refresh untuk mengunci partikel E-Ink), tempel **selotip/stiker penutup cahaya** di area bawah belakang perangkat, atau gunakan teknik "Shadow Turn" — tutup layar dengan tangan saat membalik halaman di bawah sinar matahari.

---

## 8. Perawatan dan aksesoris untuk iklim Indonesia

### Merawat layar E-Ink

Layar E-Ink **lebih rapuh dari LCD/OLED** — hindari menekan, menjatuhkan, atau membengkokkan perangkat (X4 sangat tipis: 5.9mm). Bersihkan dengan kain microfiber. Keuntungan X4 tanpa touchscreen: layar tetap bersih karena tidak perlu disentuh saat membaca.

### Tips baterai awet

Baterai 650mAh menggunakan teknologi lithium — **jangan biarkan habis total sebelum charge**. Cabut charger setelah penuh. Matikan WiFi dan Bluetooth saat tidak digunakan. Layar E-Ink hanya mengonsumsi daya saat mengganti halaman — halaman statis tidak menggunakan daya sama sekali, sehingga baterai bisa bertahan berminggu-minggu dengan pemakaian ringan.

### Penyimpanan di iklim tropis

Indonesia memiliki suhu tinggi dan kelembaban yang bisa mempengaruhi perangkat elektronik. **Jangan tinggalkan X4 di dalam mobil yang terparkir di bawah sinar matahari** — panas bisa merusak layar E-Ink dan baterai. Pada suhu di atas 33°C, layar bisa menampilkan garis-garis pudar yang akan pulih saat suhu turun. Simpan di tempat kering dan sejuk saat tidak digunakan. Gunakan **ziplock bag atau pouch waterproof** saat musim hujan atau dekat air — X4 **tidak tahan air**. Pertimbangkan **silica gel** di tempat penyimpanan untuk menyerap kelembaban. Hindari perpindahan suhu drastis (dari ruangan AC ke luar yang panas) karena bisa menyebabkan kondensasi di dalam perangkat.

### Aksesoris yang direkomendasikan

- **Magnetic Case resmi** ($8.99/~Rp140rb) — perlindungan layar esensial dengan magnet di belakang (https://www.xteink.com/collections/accessories)
- **Protective Case PC shell** ($3.99/~Rp65rb) — casing polikarbonat ringan 14g
- **Matte Screen Protector** ($3.99/2pcs) — material PET anti-silau dengan rasa seperti kertas
- **Magnetic Reading Light** ($9.99/~Rp160rb) — LED rechargeable dengan 3 suhu warna (3000K/4500K/5500K), menempel via magnet
- **USB microSD card reader** (UGREEN, ~Rp50rb di Tokopedia) — esensial untuk transfer file cepat
- **SanDisk microSD 128–256GB** (~Rp150–300rb) — pengganti kartu bawaan yang kurang andal

Case dan screen protector pihak ketiga juga tersedia di Amazon dan Etsy, termasuk case artistik dari UOGNADGD dan case flip 3D-print dari komunitas.

---

## 9. Sumber ebook berbahasa Indonesia

### Google Play Books — opsi terbaik untuk XTEInk X4

**Google Play Books adalah satu-satunya platform komersial besar** yang memungkinkan download EPUB/PDF untuk sideload ke e-reader pihak ketiga. Buka https://play.google.com/books, beli buku, lalu di My Books klik menu tiga titik → **Export**. Buku DRM-free langsung terdownload sebagai EPUB. Untuk buku dengan Adobe DRM: download file .acsm, buka di **Adobe Digital Editions** (ADE), lalu gunakan **Calibre dengan plugin DeDRM** untuk menghapus DRM dan menghasilkan EPUB bersih yang bisa ditransfer ke X4.

### Buku Sekolah Elektronik (BSE) — gratis dan legal

Kementerian Pendidikan Indonesia menyediakan **2.000+ buku pelajaran gratis** dalam format PDF di https://bse.belajar.kemdikbud.go.id/ dan https://buku.kemdikbud.go.id/. Mencakup semua jenjang dari SD hingga SMA/SMK. Hak cipta telah dibeli pemerintah — **legal untuk disalin dan didistribusikan**. Download PDF lalu konversi ke XTC via XTC.js untuk pengalaman membaca optimal di X4.

### iPusnas — perpustakaan digital nasional (terbatas)

iPusnas (https://ipusnas.id/) memiliki **73.000+ judul** termasuk karya Tere Liye, Dee Lestari, dan Andrea Hirata. Sayangnya, **buku terkunci di dalam aplikasi iPusnas** — tidak bisa diekspor sebagai file EPUB/PDF untuk ditransfer ke e-reader eksternal. Gunakan iPusnas sebagai pelengkap untuk membaca di HP/tablet.

### Gramedia Digital — juga terbatas

Gramedia Digital (https://ebooks.gramedia.com/) dengan 100.000+ judul juga **mengunci buku di dalam aplikasinya** dengan DRM. Tidak ada cara resmi untuk mengekspor file ke e-reader pihak ketiga.

### Sumber ebook gratis lainnya

**Indonesia OneSearch** (https://onesearch.id/) — portal pencarian terpadu untuk 9,8 juta+ koleksi digital dari 2.344 institusi perpustakaan Indonesia. **Perpus.org** (https://www.perpus.org/) menyediakan buku Bahasa Indonesia gratis berbagai kategori. **Project Gutenberg** (https://www.gutenberg.org/) memiliki minimal konten Bahasa Indonesia, lebih banyak teks kolonial dalam Belanda/Inggris. **Open Library** (https://openlibrary.org/) memiliki beberapa buku Indonesia untuk dipinjam digital.

### Workflow konversi dengan Calibre

Calibre (https://calibre-ebook.com/) adalah software wajib untuk pemilik X4. Install Calibre, lalu tambahkan plugin **DeDRM** dari https://github.com/apprenticeharper/DeDRM_tools untuk menangani buku ber-DRM. Untuk konversi: tambahkan buku → klik Convert → pilih output EPUB → di Page Setup pilih profile **"Generic e-ink HD"** → klik OK. Untuk PDF, konversi ke EPUB bekerja baik untuk PDF berbasis teks; untuk PDF scan/gambar, gunakan XTC.js yang lebih efektif.

---

## 10. Spesifikasi teknis dan referensi lengkap

### Spesifikasi XTEInk X4

| Spesifikasi | Detail |
|-------------|--------|
| **Layar** | 4.3" (4.26") E-Ink, hitam-putih, tanpa lampu latar |
| **Resolusi** | 800 × 480 piksel, **220 PPI** |
| **Touchscreen** | Tidak ada |
| **Prosesor** | Espressif ESP32-C3, single-core RISC-V, 160 MHz |
| **RAM** | ~400 KB SRAM (~380 KB usable) |
| **Penyimpanan internal** | Tidak ada — semua data di microSD |
| **Slot microSD** | Mendukung hingga **512 GB** (format exFAT) |
| **Baterai** | **650 mAh**, hingga 14 hari pemakaian |
| **Konektivitas** | WiFi 2.4 GHz, Bluetooth |
| **USB** | Type-C (charging + firmware flash, BUKAN data transfer) |
| **Dimensi** | 114 × 69 × 5.9 mm |
| **Berat** | **74 gram** |
| **Warna** | Space Black, Frost White |
| **Magnet** | MagSafe-compatible magnetic ring built-in |
| **Harga** | ~$58 USD (~Rp950.000) |

### Versi firmware

| Firmware | Versi Terbaru | Tanggal |
|----------|---------------|---------|
| **Stock (resmi)** | XT V3.0.2 | November 2025 |
| **CrossPoint** | v1.1.1 | Februari 2026 |
| **Papyrix** | v1.18.0 | Maret 2026 |

### Link penting

| Sumber | URL |
|--------|-----|
| Situs resmi Xteink | https://www.xteink.com/ |
| Halaman produk X4 | https://www.xteink.com/products/xteink-x4 |
| Update firmware resmi | https://www.xteink.com/pages/xteink-x4-system-update |
| Aksesoris resmi | https://www.xteink.com/collections/accessories |
| CrossPoint GitHub | https://github.com/crosspoint-reader/crosspoint-reader |
| CrossPoint User Guide | https://github.com/crosspoint-reader/crosspoint-reader/blob/master/USER_GUIDE.md |
| Web flasher (CrossPoint) | https://xteink.dve.al/ |
| CrossPoint Calibre Plugin | https://github.com/crosspoint-reader/calibre-plugins/releases |
| CrossPet GitHub | https://github.com/trilwu/crosspet |
| Papyrix GitHub | https://github.com/bigbag/papyrix-reader |
| Send to X4 (Android) | https://play.google.com/store/apps/details?id=com.chapiware.sendtox4 |
| Send to X4 (iOS) | https://apps.apple.com/us/app/send-to-x4/id6758729873 |
| XTC.js (konverter komik) | https://xtcjs.app |
| EPUB2XTC resmi | https://epub2xtc.com |
| Calibre | https://calibre-ebook.com/ |
| Wallpaper komunitas | https://basvanderploeg.nl/xteink/ |
| Community hub | https://www.readme.club/ |
| Panduan komunitas | https://www.readme.club/guide |
| Reddit (resmi) | https://www.reddit.com/r/xteinkereader/ |
| Reddit (komunitas) | https://www.reddit.com/r/xteink/ |
| Guide lengkap (Joshua Lowcock) | https://www.joshualowcock.com/xteink/the-best-guide-tools-hacks-and-more-for-xteink-x4-owners/ |
| FAQ tidak resmi | https://www.joshualowcock.com/xteink/the-ultimate-xteink-x4-faq-unofficial/ |
| Troubleshooting guide | https://www.joshualowcock.com/xteink/xteink-x4-troubleshooting-a-guide-for-x4-owners/ |

---

## Kesimpulan

XTEInk X4 adalah perangkat baca yang penuh potensi meskipun berharga terjangkau — kuncinya ada di **tiga langkah esensial** yang harus dilakukan setiap pemilik baru: ganti microSD card bawaan dengan kartu bermerek, install CrossPoint firmware untuk pengalaman membaca yang jauh lebih baik, dan gunakan Calibre sebagai pusat pengelolaan ebook. Untuk pembaca Indonesia, Google Play Books menjadi sumber utama ebook komersial yang bisa ditransfer ke X4, sementara BSE menyediakan ribuan buku pelajaran gratis yang legal. Perangkat seberat 74 gram ini mungkin kecil, tapi dengan konfigurasi yang tepat, ia mampu menjadi perpustakaan saku yang menampung ribuan buku di ujung jari Anda.
