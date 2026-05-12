Cara kerjanya Bro mari kita bedah **Versi 1 ** dulu sampai tuntas. Versi ini sebenarnya sangat ramah buat pengguna yang ingin hasil instan karena sifatnya yang *plug-and-play*.

Berikut adalah panduan detail cara pemakaiannya:

---

### **1. Memahami Tampilan Utama**

Begitu kamu membuka file HTML ini di browser, kamu akan langsung melihat data contoh (demo data).

* **Dashboard Atas:** Menampilkan rangkuman total modal yang kamu keluarkan, nilai pasar asetmu saat ini, serta total nominal dan persentase kerugianmu.
* **Pie Chart:** Grafik lingkaran ini menunjukkan **Alokasi Aset**. Jika satu warna mendominasi, berarti modalmu paling banyak menumpuk di saham tersebut.

### **2. Cara Input Data Baru**

Untuk memasukkan saham milikmu sendiri, gunakan panel **"Input Saham"**:

1. **Kode Saham:** Masukkan inisial saham (contoh: BBRI atau BMRI).
2. **Avg Price:** Masukkan harga rata-rata saat kamu membeli saham tersebut.
3. **Last Price:** Masukkan harga saham yang sedang berjalan di pasar saat ini.
4. **Jml Lot:** Masukkan jumlah lot yang kamu miliki (sistem otomatis mengalikan dengan 100 lembar per lot).
5. **Klik "Add":** Data akan langsung muncul di daftar bawah dan grafik akan otomatis terupdate.

### **3. Membaca Analisis "Si Biang Kerok"**

Lihat bagian **"Analisa Kontributor Penurunan"**:

* Sistem ini hanya akan menampilkan saham-saham yang posisinya sedang rugi (minus).
* **Progress Bar:** Semakin panjang bar merahnya, berarti saham itu adalah kontributor utama yang membuat portofoliomu "berdarah" secara keseluruhan.
* Ini membantu kamu menentukan saham mana yang paling mendesak untuk diperbaiki atau dijual.

### **4. Menggunakan Alat Kalkulator Tambahan**

Di bagian bawah, ada dua alat bantu praktis:

* **Average Down:** Masukkan harga lama, lot lama, lalu masukkan harga "serok" bawah dan jumlah lot baru. Klik hitung untuk tahu harga rata-rata barumu setelah beli lagi di bawah.
* **BEP (Break Even Point):** Masukkan harga belimu dan target harga jual. Kalkulator ini akan menghitung apakah kamu sudah benar-benar untung setelah dikurangi estimasi *fee* beli (0.15%) dan *fee* jual (0.25%).

---

Cara menggunakan:


> **Catatan Penting (Limitasi Versi 1):**
> Karena versi ini tidak punya fitur **LocalStorage**, semua data yang kamu masukkan akan **hilang** jika kamu me-*refresh* halaman atau menutup tab browser. Jadi, versi ini lebih cocok untuk simulasi cepat "bagaimana jika" daripada untuk memantau portofolio harian.

---

Berikut adalah panduan penggunaan detail untuk **Versi 2** :

---

### **Panduan Penggunaan Kalkulator Portofolio (Versi 2)**

Versi ini dirancang untuk penggunaan jangka panjang dengan fitur penyimpanan data otomatis dan manajemen aset yang lebih fleksibel.

#### **1. Sistem Penyimpanan Otomatis (Local Storage)**

* Setiap data yang dimasukkan akan tersimpan secara otomatis di dalam memori browser.
* Daftar saham tidak akan hilang meskipun halaman dimuat ulang (*refresh*) atau browser ditutup.

#### **2. Manajemen Daftar Saham**

* **Input Data:** Gunakan formulir input untuk memasukkan kode saham, harga rata-rata beli, harga pasar saat ini, dan jumlah lot.
* **Fitur Edit:** Setiap baris saham memiliki tombol "Edit" yang memungkinkan perubahan harga pasar atau jumlah lot tanpa harus menghapus data lama.
* **Penghapusan:** Gunakan tombol "Hapus" (X) untuk menghilangkan aset yang sudah tidak ada dalam portofolio nyata.

#### **3. Analisis Penurunan & P&L**

* **Dashboard Real-time:** Bagian atas menampilkan total modal, nilai pasar saat ini, serta total keuntungan atau kerugian (P&L) secara keseluruhan.
* **Indikator Warna:** Angri merah menunjukkan posisi kerugian (*loss*), sementara angka hijau menunjukkan posisi keuntungan (*gain*).
* **Kontributor Kerugian:** Sistem menganalisis secara mendalam saham mana yang memberikan dampak penurunan terbesar terhadap total modal, sehingga membantu prioritas pengambilan keputusan.

#### **4. Kalkulator Strategi (Tools)**

* **Average Down:** Fitur ini menghitung proyeksi harga rata-rata baru jika dilakukan pembelian tambahan di harga bawah (serok).
* **Break Even Point (BEP):** Kalkulator ini menghitung harga jual minimum agar modal kembali utuh setelah dikurangi estimasi biaya transaksi (*fee* beli dan *fee* jual).

#### **5. Alokasi Aset (Visual)**

* **Grafik Lingkaran:** Menampilkan persentase sebaran modal pada setiap kode saham untuk memantau diversifikasi aset agar tidak terlalu dominan pada satu sektor saja.

---
