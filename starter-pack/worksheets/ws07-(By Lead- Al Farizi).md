# **WORKBOOK: LEMBAR KERJA MAHASISWA (WS07)** 

## **Simple Solution Design — IPO, Flowchart & Pseudocode** 

### **INFORMASI UTAMA** 

- **Mata Kuliah** : Konsep Sistem Informasi (KSI) 

- **Kerangka Kerja** : Project-Based Learning (PBL) Level 1 

- **Learning Moment** : _Fase 4: Design (Minggu 5–6)_ 

- **Sub-CPMK / SFIA** : S-03.1 (Intermediate) | SFIA ARCH L2, DESN L2 

- **Keterkaitan Deliverable** : Sumber utama pembuatan **Deliverable D2 (System** 

   - **& Solution Design - TPL-02)** 

- **Phase Lead** : **Mahasiswa D** ( _Phase Lead 4 — Design_ ) 

### **RUANG KERJA TIM (WORKSPACE)** 

#### **1. IDENTIFIKASI KELOMPOK & SOLUSI** 

- **Nama Tim** : Hundred Team 

- **Nama UMKM Mitra** : Coffee Shop Hundred 

- **Judul Solusi SI** : **OrderFlow** 

- **Phase Lead 4 (Design)** : Ahmad Al farizi 

#### **2. PEMETAAN ARSITEKTUR 4 LAPISAN SI (M05)** 

Petakan solusi Anda ke dalam 4 lapisan arsitektur terintegrasi: 

|**Lapisan**<br>**Arsitektur**|**Komponen Solusi Tim**|**Keterangan &**<br>**Batasan**|
|---|---|---|
|**1. Process**<br>**Layer**_(Alur_<br>_Kerja To-Be)_|Pelanggan memesan sebuah kopi atau makanan<br>setelah itu pesanan langsung masuk ke dalam system<br>antrean.|Alur transaksi<br>kasir yang<br>mengintegrasik<br>an metode<br>pemanggilan<br>otomatis<br>**OrderFlow**|
|||(nama & nomor<br>meja<br>pelanggan)<br>untuk|



|||mengatasi<br>_bottleneck_<br>(penumpukan<br>antrean dan<br>kebingungan<br>pelanggan saat<br>pengambilan<br>pesanan).|
|---|---|---|
|**2. Data**<br>**Layer**_(Struktur_<br>_Data Logis)_|Tabel Menu/Produk, Tabel Transaksi, Tabel Stok,<br>& Tabel OrderFlow|Entitas data:<br>Tabel<br>Menu/Produk,<br>Tabel<br>Transaksi, &<br>Tabel Stok,<br>ditambah Tabel<br>OrderFlow<br>untuk<br>menyimpan<br>status antrean,<br>nama<br>pelanggan, dan<br>nomor meja.|
|**3. Application**<br>**Layer**_(Modul_<br>_Program)_|Modul Login, Input Transaksi, Hitung Total/Diskon,<br>Rekap, & Modul OrderFlow Engine|Modul Utama:<br>Login, Input<br>Transaksi,<br>Hitung<br>Total/Diskon, &<br>Rekap, serta<br>Engine<br>OrderFlow<br>khusus untuk<br>memicu<br>notifikasi<br>pemanggilan<br>pelanggan.|
|**4.**<br>**Infrastructure**<br>**Layer**_(Perang_<br>_kat Fisik)_|menggunakan POS/EDC & Tablet Monitor<br>Display|Hardware: POS<br>/ EDC & Tablet<br>Display;<br>Network:<br>Wi-Fi/4G; OS:<br>Windows/Andro<br>id.|



#### **3. SPESIFIKASI IPO (INPUT - PROCESSING - OUTPUT - STORAGE - CONTROL)** 

**Fitur Fungsional Utama 1: [Tuliskan Nama Fitur, misal: Pencatatan Transaksi Penjualan]** 

- **Input** : Pelanggan mendatangi meja kasir dan membaca daftar menu di papan display. Kasir menyapa dan memberikan rekomendasi jika pelanggan bingung memilih varian. Kasir menginput item pilihan ke aplikasi POS berbasis tablet. 

- **Processing** :Sistem POS\ADC secara otomatis menghitung total harga tagihan. Pelanggan melakukan pembayaran di awal via scan QRIS statis atau Tunai. Mesin kasir mencetak 1 rangkap struk nota thermal. 

- **Output** : Sistem audio (speaker) memutar suara panggilan secara otomatis agar customer bisa mengetahui pesanan nya sudah di buat. 

- **Storage** : Sistem menyimpan log riwayat. 

- **Control (Error Handling)** : Jika koneksi ke speaker atau layar antrean terputus,sistem akan menampilkan notifikasi error. 

#### **4. DIAGRAM ALIR (FLOWCHART) LOGIKA PROGRAM** 

_Petunjuk: Gambarkan diagram alir terstruktur menggunakan simbol standar (Persegi Panjang = Proses, Belah Ketupat = Keputusan IF-ELSE, Jajar Genjang = Input/Output, Oval = Start/End). Lampirkan hasil gambaran digital/foto kertas A3 di bawah ini._ 

- `[ TEMPELKAN GAMBAR DIAGRAM FLOWCHART DIGITAL / FOTO DRAF A3 DI SINI ]` 



#### **5. PSEUDOCODE TERSTRUKTUR (INDEPENDEN TEKNOLOGI)** 

Tuliskan kode semu terstruktur ( _pseudocode_ ) untuk modul logika utama solusi Anda: 

```
ALGORITMA Sistem_Coffee_Shop_OrderFlow
```

```
KAMUS DATA:
```

```
menu_pesanan, metode_pembayaran, lokasi_tunggu : STRING
nomor_antrean : INTEGER
status_pesanan : STRING
```

```
ALUR LOGIKA:
```

```
START
```

```
// 1. Fase Pemesanan
```

```
PRINT "Pelanggan datang dan memesan menu"
INPUT menu_pesanan
```

```
// 2. Pemrosesan Sistem & Kasir
nomor_antrean = Generate_Nomor_Antrean()
CALL Simpan_Data_Pesanan(menu_pesanan, nomor_antrean)
PRINT "Kasir mencetak struk"
// 3. Fase Pembayaran
INPUT metode_pembayaran
IF metode_pembayaran == "CASH" THEN
PRINT "Kasir menerima Cash"
CALL Konfirmasi_Pembayaran()
ELSE IF metode_pembayaran == "QRIS" THEN
PRINT "Sistem menampilkan QRIS"
CALL Konfirmasi_Pembayaran()
ENDIF
// 4. Pilihan Tempat Menunggu oleh Pelanggan
INPUT lokasi_tunggu
IF lokasi_tunggu == "Menunggu di depan kasir" THEN
PRINT "Pelanggan menunggu di depan kasir"
ELSE IF lokasi_tunggu == "Menunggu di meja" THEN
PRINT "Pelanggan memantau sambil menunggu antrean (tanpa antre di depan
kasir)"
ENDIF
// 5. Proses Barista & Pemanggilan Otomatis via Speaker
PRINT "Barista/staff menyelesaikan pesanan dan mengubah status menjadi 'pesanan
siap'"
status_pesanan = "Pesanan Siap"
IF status_pesanan == "Pesanan Siap" THEN
// Sistem memicu pengeras suara secara otomatis
CALL Sistem_Menjalankan_Pemanggilan_Otomatis_Melalui_Speaker()
PRINT "Pelanggan mendengar dan menuju counter kasir"
ENDIF
// 6. Penyelesaian
PRINT "Mengambil pesanan"
END
```

### **CHECKLIST REFLEKSI & PENGESAHAN WS07** 

Arsitektur 4 lapisan SI telah terdefinisi konsisten. 

Tabel IPO mencakup kriteria _Storage_ dan _Control_ (penanganan eror). Flowchart menggambarkan logika percabangan ( _IF-ELSE_ ) dan perulangan ( _Loops_ ) tanpa _infinite loop_ . 

Pseudocode terstruktur dengan rapi dan independen terhadap bahasa pemrograman. 

Form **TPL-07 (AI Usage Disclosure & Verification Note)** telah dilampirkan. 

**Tanggal Pengesahan** : 11 november 2026 **Tanda Tangan Phase Lead 4 (Design)** : **Tanda Tangan Dosen Pembimbing / Coach** : 

