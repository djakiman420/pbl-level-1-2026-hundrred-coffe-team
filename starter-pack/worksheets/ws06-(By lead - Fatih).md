# **WORKBOOK: LEMBAR KERJA MAHASISWA WS06** 

## **Success Metrics (BPI/DMAIC) & Pemetaan Komponen SI Awal** 

Mata Kuliah: **Konsep Sistem Informasi (KSI)** Kerangka Kerja: **Project-Based Learning (PBL) Level 1** Fase Learning Spine: **Fase 3 — Define (Minggu 4)** Sub-CPMK / SFIA: **S-01.1 (Intermediate - Problem Framing) & S-03.1 (Intermediate - Pemetaan SI)** | **SFIA BUSA L1, METR L2** 

Keterkaitan Deliverable: **Bahan Utama Deliverable D1 Final (TPL-01) & D2 Draf (TPL-02)** 

### **1. Identifikasi Kelompok & Rotasi Kepemimpinan** 

- **Nama Kelompok** : Hundred Team 

- **Objek UMKM Mitra** : Coffee Shop 

- **Phase Lead 3 (Define)** : Fatih Parulian Romadhon Hasibuan (Mahasiswa C) 

- **Anggota Tim** : 1. Najwan Mahdy SK 2. Arkyanu Aufaa Sugara 3. Ahmad Al Farizi 4. Yusril djakiman 

### **2. Landasan Konseptual: Metrik BPI & Pemetaan 5 Pilar SI** 

- **Business Process Improvement (BPI)** mengukur keberhasilan perbaikan proses bisnis melalui dua dimensi utama (Rainer et al., 2014): 

   - **Efisiensi (** **_Efficiency_ )** : Mengukur penghematan sumber daya ( _doing things well_ ), seperti efisiensi waktu siklus transaksi atau reduksi biaya operasional. 

   - **Efektivitas (** **_Effectiveness_ )** : Mengukur pencapaian kualitas/tujuan ( _doing the right things_ ), seperti akurasi data stok, penurunan angka selisih kasir, dan kepuasan pelanggan. 

- **Model 5 Pilar SI O'Brien** : Solusi sistem informasi dipetakan ke dalam pilar _People, Hardware, Software, Data,_ dan _Network_ (Marakas & O'Brien, 2013). 

### **3. Workspace A: Matrik Metrik Keberhasilan Bisnis (DMAIC Six Sigma)** 

|**Dimensi Metrik**|**Parameter**<br>**Kinerja**|**Kondisi**<br>**Baseline**<br>**(As-Is)**|**Target Solusi**<br>**(To-Be)**|**Metode**<br>**Pengukuran**|
|---|---|---|---|---|
|**Efisiensi**<br>**(Waktu)**|Durasi<br>pelayanan<br>transaksi per<br>pelanggan|180 detik|90 detik|Stopwatch<br>transaksi|
|**Efisiensi**<br>**(Waktu)**|Durasi<br>rekapitulasi<br>harian pemilik|300 - 600 detik<br>/ malam|600 detik /<br>malam|Wawancara|
|**Efektivitas**<br>**(Akurasi)**|Tingkat selisih<br>pencatatan stok<br>barang|Selisih 1-2% /<br>bulan|Selisih 0,5% /<br>bulan|Stock opname<br>bulanan|
|**Efektivitas**<br>**(Kualitas)**|Frekuensi<br>kesalahan<br>hitung nota|3 - 4 kali /<br>minggu|1 - 2 kali /<br>minggu|Audit sampel<br>lembar nota dan<br>pengecekan di<br>grup laporan|



### **4. Workspace B: Pemetaan Arsitektur 5 Pilar SI Solusi Awal** 

┌────────────────────────────────────────────┐ │ PETA 5 PILAR SISTEM INFORMASI │ ├────────────────────────────────────────────┤ │ 1. PEOPLE RESOURCES (Pengguna & Spesialis) │ │  • Pengguna Akhir: Kasir (Kak Eca)│ │  • Pengelola Data: SPV (Pak Sangap) atau Kasir (Kak Eca) │ ├────────────────────────────────────────────┤ │ 2. HARDWARE RESOURCES (Perangkat Mesin & Media) │ 

- │  • Perangkat Fisik Input: Monitror TouchScreen/Tablet, Mouse dan Keyboard (Opsional), QR Code (Opsional) │  • Perangkat Fisik Output: Speaker, Layar Antrean (TV), Printer Struk │ ├────────────────────────────────────────────┤ │ 3. SOFTWARE RESOURCES (Aplikasi & Prosedur Operational) │ │  • Aplikasi Program: SIstem Antrean Kasir (fitur pemanggilan pesanan), Modul Text-To-Speech(TTS) │ │  • Prosedur Pengguna: 1. Tahap Persiapan - Barista membuat pesanan sesuai kemauan pelanggan. 

- - Pembaruan Status : Setelah pesanan dibuat, pegawai mengubah status pesanan dari “Dalam Proses” menjadi “Siap Disajikan”. 

   2. Tahap Pemanggilan 

- Pegawai menekan tombol “Panggil Pesanan” untuk memanggil nomor antrean/nama pelanggan yang bersangkutan. 

- - Sistem audio memutar suara panggilan otomatis. 

- 3. Tahap Penyelesaian - Verifikasi Pelanggan: Pelanggan mendatangi counter setelah mendengar panggilan. 

- - Kasir menyerahkan pesanan kepada pelanggan. │ 

- ├────────────────────────────────────────────┤ │ 4. DATA RESOURCES (Struktur Data & Basis Data) │ 

│  • Data Transaksi: Data Nomor Antrean Pelanggan & Nama Pelanggan, Log Aktifitas Pemanggilan │ 

- │  • Data Produk/Stok: FIle Audio Suara Panggilan. │ 

├────────────────────────────────────────────┤ 

- │ 5. NETWORK RESOURCES (Jaringan Communication & Media) 

│ 

- │  • Konektivitas: Jaringan Lokal, Koneksi Audio Output. │ 

└────────────────────────────────────────────┘ 

### **5. Workspace C: Lembar Persetujuan Formal Mitra (Sign-Off)** 

Dengan ini, pemilik / manajer UMKM mitra menyatakan setuju atas rumusan kebutuhan fungsional, target metrik keberhasilan, dan batas cakupan sistem yang dirancang oleh tim mahasiswa. 

- **Nama UMKM Mitra** : Hundred Coffee 

- **Nama Pemilik / Pengelola** : Pak Sangap 

- **Tanggal Persetujuan** : 06/11/2026 

#### **Tanda Tangan Persetujuan Mitra** : 

_(Cap / Tanda Tangan Pemilik UMKM Mitra)_ 

### **6. Verifikasi Integritas AI (TPL-07) & Pengesahan** 

- **Penggunaan AI Co-pilot** : 

Apakah tim menggunakan AI untuk membantu merumuskan metrik BPI / diagram 5 pilar SI? [X] Ya 

_(Jika Ya, wajib melampirkan formulir_ **_TPL-07: AI Usage Disclosure & Verification Note_** _)_ . 

**Tanda Tangan Tim & Pengesahan Dosen** : 

- **Phase Lead 3** : Fatih Parulian Romadhon Hasibuan (Tanggal: 11/11/2026) 

- **Dosen Coach** : (Tanggal: ) [ ] Approved 

