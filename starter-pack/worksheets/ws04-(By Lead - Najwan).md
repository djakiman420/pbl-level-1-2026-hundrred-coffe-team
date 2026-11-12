## WS04: Problem Identification & Scope

**Mata Kuliah**: Konsep Sistem Informasi (KSI)

**Kerangka Kerja**: Project-Based Learning (PBL) Level 1

**Fase Learning Spine**: **Fase 2 — Frame (Problem Discovery & Scope) Minggu / Alokasi Waktu**: Minggu 2 / 14 Jam Belajar

**Sub-CPMK / SFIA**: S-01.1 (Introduce - Problem Framing) | SFIA BUSA L1 (_Business Analysis_), IRMG L1

#### Penanggung Jawab Fase: Phase Lead 2 (Frame — Mahasiswa B)

**Keterkaitan Deliverable**: Sumber Utama Penyusunan **Deliverable D1 (Problem Brief - TPL-01)**

# 1. Identifikasi Tim & Objek Proyek

| **Elemen Informasi**          | **Rincian Identitas Kelompok & Mitra** |
| ----------------------------- | -------------------------------------- |
| **Nama Kelompok / Kelas**     | \[Hundred Team / A \]                  |
| **Phase Lead 2 (Frame - M2)** | \[Arkyanu Aufaa Sugara — 2600016025\]  |
| **Nama UMKM Mitra Lapangan**  | \[Coffee Shop Hundred\]                |
| **Pemilik / Kontak Mitra**    | \[Pak Sangap / 0822-8114-5011\]        |

2. **Matriks Problem Framing & Analisis Akar Masalah (Root Cause Analysis)**

Gunakan temuan kuantitatif dari WS03 untuk memisahkan antara **Gejala Permukaan (_Symptoms_)** dan **Akar Masalah Utama (_Root Cause_)** operasional bisnis mitra:

| **No** | **Kategori Observasi**     | **Gejala Permukaan (_Symptoms_)**    | **Akar Masalah Operasional (_Root Cause_)**                                           | **Bukti Kuantitatif (_Baseline Data_)**                              |
| ------ | -------------------------- | ------------------------------------ | ------------------------------------------------------------------------------------- | -------------------------------------------------------------------- |
| **1**  | **Proses Transaksi Kasir** | Antrean memanjang saat kondisi padat | Masih menggunakan pemanggilan pesanan yang manual secara lisan sehingga pelayan harus | Rata-rata pelayan harus berkeliling rata rata = **60 detik/pesanan** |

|       |                             |                                                                                                  | berkeliling terlebih dahulu                                                                                                                                                                                                                                                     |                                                                                                                                                                                          |
| ----- | --------------------------- | ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **2** | **Pengelolaan Stok Barang** | Pencatatan stok bahan baku berisiko tidak akurat atau terlambat terdeteksi                       | Metode pencatatan stok sebelumnya dilakukan secara mingguan (_weekly_) dan penginputan bahan baku masih mengandalkan kedisiplinan mandiri (_self-reporting_) staf.                                                                                                              | Sistem direkap harian (_daily_) via **Google Spreadsheet** manual oleh staf bar untuk bahan baku utama (biji kopi, susu,<br><br>sirup).                                                  |
| **3** | **Rekapitulasi Keuangan**   | Laporan omset dan sisa bahan baku rawan selisih atau lambat direkap.                             | Catatan penjualan dan stok belum terhubung otomatis. Kasir pakai aplikasi Nuta POS, tapi stok bahan masih diisi manual sama barista di Google Spreadsheet.                                                                                                                      | Memakai 1 aplikasi POS dan 1 file Spreadsheet terpisah. Rekap stok baru diubah dari mingguan (1x seminggu) jadi harian (1x sehari) oleh 1 barista per shift.                             |
| **4** | **Infastruktur Jaringan**   | Koneksi internet (WI-FI) terputus dan harus login ulang ketika pelanggan berpindah tempat duduk. | Pemasangan 3 unit modem/router di area kedai dilakukan secara<br><br>terpisah-pisah tanpa menggunakan sistem jaringan terpusat yang mendukung fitur _seamless roaming_, sehingga setiap perangkat berdiri sendiri dan membaca perpindahan jaringan sebagai<br><br>koneksi baru. | **100%**<br><br>**pelanggan** yang berpindah posisi duduk dari area kasir ke area meja lain mengalami pemutusan koneksi (_disconnect_) dan wajib _login_ ulang ke jaringan<br><br>Wi-Fi. |
| **5** | **Sistem Pembayaran**       | Transaksi menggunakan QRIS gagal diproses saat jam sibuk di                                      | Terjadinya pemeliharaan sistem rutin (_maintenance_) berkala dari pihak penyedia layanan perbankan/QRIS                                                                                                                                                                         | **100% transaksi** yang gagal saat jam _maintenance_ dialihkan secara manual ke                                                                                                          |

|     |     | malam hari, sehingga kasir terpaksa mengalihkan pembayaran ke metode tunai secara mendadak dan memicu antrean panjang. | pada jam malam, sementara kedai belum memiliki SOP penanganan cepat atau opsi _backup_ pembayaran digital alternatif yang siap pakai di kasir. | pembayaran tunai, yang memperlambat waktu layanan kasir dan menyebabkan penumpukan antrean. |
| --- | --- | ---------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- |

# 3. Perumusan Problem Statement Kontekstual

Berdasarkan analisis di atas, rumuskan **Problem Statement** utama dalam 1–2 paragraf terstruktur.

_Petunjuk_: Hindari mendefinisikan masalah sebagai _"Mitra belum memiliki aplikasi Python/komputer"_. Definisikan dari hambatan bisnis nyata mitra!

#### Rumusan Problem Statement Kelompok

"Saat pengunjung ramai di malam hari, antrean sering menumpuk dan pesanan jadi lambat karena kasir dan barista dipegang oleh 1 orang per _shift_ tanpa bantuan alat pager antrean. Di sisi lain, rekap stok bahan baku seperti kopi, susu, dan sirup masih dilakukan secara terpisah melalui Google Spreadsheet manual. Hal ini berisiko memicu selisih data antara omzet penjualan di aplikasi kasir (Nuta POS) dengan sisa bahan baku di lapangan, serta menurunkan kenyamanan pengunjung yang berdampak pada rendahnya jumlah pelanggan yang datang kembali (_repeat customer_)."

# 4. Menetapkan Batasan Sistem (System Boundary / Scope Alignment)

Untuk mencegah terjadinya pembengkakan fitur (_Scope Creep_) yang membahayakan penyelesaian proyek dalam 1 semester, tentukan secara tegas apa yang **Masuk Cakupan (_In-Scope_)** dan apa yang **Di Luar Cakupan (_Out-of-Scope_)**:

None

```
┌───────────────────────────────────────────┐
```

│ SYSTEM BOUNDARY (BATASAN SISTEM) │

```
│ │
```

│ \[ IN-SCOPE: Fitur yang Akan Dibangun \] │

│ 1. Menerapkan fitur panggil otomatis agar pelanggan tidak perlu menunggu pesanan di buat │

│ 2. Mengintegrasikan modem yang terpisah ke dalam satu Router │

│ 3. Menyediakan metode QRIS cadangan (alternartif) │

```
│ │
│─────────────────────────────────────────── │
│ │
```

│ \[ OUT-OF-SCOPE: Di Luar Cakupan Proyek \] │

│ 1. Tidak merekrut staf khusus runner, karena pertimbangan efisiensi biaya operasional kedai.

│ 2. Pengembangan Aplikasi Self-Service Kiosk / Pager Hardware (Pemanggilan)

│ 3. Perbaikan Core Server / Backend Utama QRIS <sub>│</sub>

```
└────────────────────────────────────────────┘
```

**Tabel Penegasan Cakupan Proyek (_Scope Alignment Table_)**

| **No** | **Modul / Fitur Sistem**          | **Status Cakupan (_In-Scope /_**<br><br>**_Out-of-Scope_)** | **Alasan Pertimbangan Kelayakan**<br><br>**(O'Brien)**                         |
| ------ | --------------------------------- | ----------------------------------------------------------- | ------------------------------------------------------------------------------ |
| **1**  | Input Transaksi & Kalkulasi Total | **IN-SCOPE**                                                | Kelayakan Operasional: Sangat dibutuhkan kasir untuk mempercepat transaksi.    |
| **2**  | Update Stok Otomatis              | **IN-SCOPE**                                                | Kelayakan Teknis: Dapat diimplementasikan dengan logika struktur data Python.  |
| **3**  | Laporan Rekap Harian (Laba/Rugi)  | **IN-SCOPE**                                                | Kelayakan Ekonomi: Memberikan nilai _Value of Information_ bagi pemilik usaha. |

| **No** | **Modul / Fitur Sistem**            | **Status Cakupan (_In-Scope /_**<br><br>**_Out-of-Scope_)** | **Alasan Pertimbangan Kelayakan**<br><br>**(O'Brien)**                       |
| ------ | ----------------------------------- | ----------------------------------------------------------- | ---------------------------------------------------------------------------- |
| **4**  | Pembayaran Online / Payment Gateway | **OUT-OF-SCOPE**                                            | Keterbatasan waktu 1 semester & kompleksitas API luar di PBL Level<br><br>1. |
| **5**  | Multi-Branch / Banyak Cabang        | **OUT-OF-SCOPE**                                            | Mitra saat ini hanya memiliki 1 lokasi usaha operasional.                    |

# 5. Target Metrik Keberhasilan Solusi (To-Be Targets)

Tentukan target kuantitatif perbaikan yang ingin dicapai melalui solusi sistem informasi To-Be:

| **Indikator Kinerja**               | **Kondisi As-Is (Baseline)** | **Target To-Be (Expected)** | **Estimasi Persentase Peningkatan**             |
| ----------------------------------- | ---------------------------- | --------------------------- | ----------------------------------------------- |
| **Waktu Pelayanan Transaksi Kasir** | 180 Detik / pelanggan        | **90 detik / pelanggan**    | Peningkatan efisiensi<br><br>**50%**            |
| **Durasi Rekapitulasi Harian**      | 300 - 600 Detik / malam      | **600 detik / malam**       | Penghematan waktu<br><br>**83,3%**              |
| **Akurasi Pencatatan Stok**         | Terdapat 3-5 Miss / bulan    | **Akurasi > 98%**           | Penurunan tingkat kesalahan selisih<br><br>stok |

# 6. Refleksi & Lembar Pengesahan Phase Lead

### A. Pertanyaan Refleksi Tim

1. _Bagaimana tim memastikan bahwa batasan proyek yang ditetapkan realistis untuk diselesaikan dalam 16 minggu?_
   - **Jawab**: \[ Fokus ke Solusi Masalah Utama, Membuat _Timeline_, Sesuaikan dengan Kemampuan dan Kapasitas Tim, Evaluasi Rutin Rutin Tiap Minggu \]
2. _Apakah pemilik usaha mitra telah menyetujui batasan sistem yang diusulkan oleh kelompok?_
   - **Jawab**: \[ Iya, Sangat di approve \]

### B. Tanda Tangan Pengesahan Phase Lead 2

None

Disusun oleh Phase Lead 2 (Frame): \[ Arkyanu Aufaa Sugara — 2600016025 \] Tanggal Penyusunan: \[ 6 November 2026 \]

Tanda Tangan Phase Lead 2:

Diverifikasi oleh Dosen Pengampu / Coach:

Tanggal: \[ Tanggal \] | Status Checkpoint: \[ APPROVED / REVISION NEEDED \] Catatan Dosen: