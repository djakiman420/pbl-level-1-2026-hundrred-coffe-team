# **WORKBOOK: LEMBAR KERJA MAHASISWA WS05** 

## **Formulasi Kebutuhan Fungsional: User Story & Acceptance Criteria** 

Mata Kuliah: **Konsep Sistem Informasi (KSI)** Kerangka Kerja: **Project-Based Learning (PBL) Level 1** Fase Learning Spine: **Fase 3 — Define (Minggu 3)** Sub-CPMK / SFIA: **S-01.1 (Intermediate - Problem Framing) & S-03.1 (Intermediate - Pemetaan SI)** | **SFIA BUSA L1, REQM L2** Keterkaitan Deliverable: **Bahan Utama Deliverable D2 (System & Solution Design - TPL-02)** 

### **1. Identifikasi Kelompok & Rotasi Kepemimpinan** 

- **Nama Kelompok** : Hundred Team 

- **Objek UMKM Mitra** : Coffee Shop (Hundred Coffee) 

- **Phase Lead 3 (Define)** : Fatih Parulian Romadhon Hasibuan (Mahasiswa C) 

- **Anggota Tim** : 

   1. Arkyanu Aufaa Sugara 

   2. Ahmad Al Farizi 

   3. Yusril Yusuf Djakiman 

   4. Najwan Mahdy SK 

### **2. Landasan Konseptual: Analisis Sistem "What" vs "How"** 

Dalam tahap _Systems Analysis_ , fokus utama tim adalah menentukan **APA (** **_What_ )** yang dibutuhkan pengguna bisnis untuk memecahkan masalahnya, **BUKAN BAGAIMANA (** **_How_ )** sistem dibangun secara teknis (Marakas & O'Brien, 2013). 

- **User Story** merepresentasikan kebutuhan fungsional dari sudut pandang pengguna bisnis dengan pola: 

"𝑆𝑒𝑏𝑎𝑔𝑎𝑖[𝑃𝑒𝑟𝑎𝑛𝑃𝑒𝑛𝑔𝑔𝑢𝑛𝑎], 𝑆𝑎𝑦𝑎 𝑖𝑛𝑔𝑖𝑛 [𝐾𝑒𝑚𝑎𝑚𝑝𝑢𝑎𝑛/𝐹𝑖𝑡𝑢𝑟], 𝑆𝑒ℎ𝑖𝑛𝑔𝑔𝑎[𝑀𝑎𝑛𝑓𝑎𝑎𝑡𝐵𝑖𝑠𝑛𝑖𝑠𝑁𝑦𝑎𝑡𝑎]" 

- **Acceptance Criteria (Given-When-Then)** mendefinisikan batas kondisi kapan sebuah fitur dinyatakan selesai dan memenuhi syarat penerimaan pengguna (Rainer et al., 2021). 

### **3. Workspace A: Formulasi User Story Fungsional** 

Petakan minimal **3 User Story Utama** yang langsung menjawab akar masalah pada D1 / WS04: 

#### **User Story 1 (Prioritas Utama / Core Feature)** 

- **Sebagai (** **_As a_ )** : Kasir/SPV Hundred Coffee 

- **Saya ingin (** **_I want to_ )** : Pemanggilan pesanan menjadi otomatis dan kasir tidak perlu meneriakkan nama customer 

- **Sehingga (** **_So that_ )** : Waktu pelayanan atau pengantaran tidak terpotong _(misal: waktu transaksi berkurang dan tidak terjadi kesalahan hitung uang kembalian)_ 

#### **User Story 2 (Infastrukrur Jaringan)** 

- **Sebagai (** **_As a_ )** : Kasir/SPV Hundred Coffee 

- **Saya ingin (** **_I want to_ )** : Semua jaringan wifi menjadi 1 pusat jaringan 

- **Sehingga (** **_So that_ )** : Pelanggan tidak perlu login ulang wifi ketika ia ingin berpindah tempat duduk 

#### **User Story 3 (Sistem Pembayaran)** 

- **Sebagai (** **_As a_ )** : Kasir/SPV Hundred Coffee 

- **Saya ingin (** **_I want to_ )** : Pelanggan bisa melakukan payment pada jam malam 

- **Sehingga (** **_So that_ )** : Pelanggan tidak perlu menyiapkan uang cash / dan bisa memesan makanan/minuman pada jam malam 

### **4. Workspace B: Acceptance Criteria Berbasis Skenario (Given-When-Then)** 

Susun kriteria penerimaan terstruktur untuk **User Story 1** (mencakup Skenario Sukses dan Skenario Penanganan Eror): 

#### **Skenario 1A: Pemanggilan Pesanan Otomatis Berhasil (Happy Path)** 

- **Diberikan (** **_Given_ )** : Pesanan pelanggan telah selesai dibuat oleh barista dan status pesanan di sistem sudah ditandai sebagai "Siap Disajikan". 

- **Ketika (** **_When_ )** : Kasir atau SPV menekan tombol "Panggil Pesanan" untuk nomor antrean/nama tersebut di layar sistem. 

- **Maka (** **_Then_ )** : Sistem audio secara otomatis memutar suara panggilan (misal: "Nomor antrean 25, pesanan Anda silakan diambil"), layar antrean menampilkan nomor tersebut, dan kasir tidak perlu memanggil secara manual. 

**Skenario 1B: Penanganan Eror Pemanggilan / Status Tidak Valid (Exception Path)** 

- **Diberikan (** **_Given_ )** : Pesanan pelanggan dengan nomor antrean 30 masih dalam tahap pembuatan dan berstatus "Sedang Diproses". 

- **Ketika (** **_When_ )** : Kasir tidak sengaja menekan tombol "Panggil Pesanan" untuk nomor antrean 30 tersebut. 

- **Maka (** **_Then_ )** : Sistem menolak perintah pemanggilan, menampilkan pesan peringatan "Eror: Pesanan belum berstatus Siap", dan sistem audio tidak mengeluarkan suara pemanggilan apa pun. 

### **5. Workspace C: Catatan Validasi Kebutuhan dengan Mitra (Field Confirmation)** 

- **Tanggal Validasi** : 06/11/2026 

- **Narahubung Mitra** : Pak Sangap / Kasir 

- **Hasil Konfirmasi User Story** : 

   - [X] Seluruh User Story disetujui mitra 

   - [ ] Terdapat penyesuaian/revisi kebutuhan (Tuliskan revisi jika ada): 

### **6. Verifikasi Integritas AI (TPL-07) & Pengesahan** 

- **Penggunaan AI Co-pilot** : 

Apakah tim menggunakan AI untuk membantu merumuskan skenario _Given-When-Then_ ? [X] Ya 

_(Jika Ya, wajib melampirkan formulir_ **_TPL-07: AI Usage Disclosure & Verification Note_** _)_ . 

**Tanda Tangan Tim & Pengesahan Dosen** : 

- **Phase Lead 3** : Fatih Parulian Romadhon Hasibuan (Tanggal: 2 November 2026) 

- **Dosen Coach** : (Tanggal: ) [ ] Approved 

