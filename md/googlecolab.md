Ah, paham! Kalau di **Google Colab**, situasinya jadi jauh lebih mudah karena Anda tidak perlu pusing memikirkan *environment variable* atau sistem operasi Windows. Google Colab berjalan di cloud berbasis Linux.

Berikut adalah perintah-perintah penting yang biasa digunakan saat bekerja dengan `google-genai` **khusus di Google Colab**:

### 1. Perintah Instalasi

Di Google Colab, Anda harus menambahkan tanda seru (`!`) di depan perintah `pip` agar Colab tahu bahwa Anda sedang menjalankan perintah terminal, bukan kode Python.

* **Instal library utama:**
```bash
!pip install google-genai

```


* **Instal sekaligus dengan library pendukung (opsional):**
Di Colab, library gambar (`pillow`) sudah otomatis terinstal. Namun jika Anda butuh library visualisasi data atau manipulasi file yang sering mendampingi AI, Anda bisa pakai:

```bash
    !pip install google-genai pandas matplotlib
    ```

### 2. Cara Aman Memasukkan API Key di Colab (Tanpa Perintah `export`)
Di Google Colab, Anda **tidak perlu** mengetik perintah `set` atau `export` untuk API Key. Colab punya fitur bawaan yang jauh lebih aman bernama **Secrets** (ikon kunci di menu sebelah kiri).

1. Klik ikon **Kunci (Secrets)** di sidebar kiri Colab.
2. Tambahkan secret baru dengan Name: `GEMINI_API_KEY`.
3. Masukkan API Key Anda di kolom Value.
4. Aktifkan tombol centang **Notebook access**.

Setelah itu, jalankan perintah Python ini di dalam *cell* Colab Anda untuk memanggilnya:

```python
from google.colab import userdata
from google import genai

# Colab akan otomatis mengambil API Key yang Anda simpan di fitur Secrets tadi
api_key = userdata.get('GEMINI_API_KEY')
client = genai.Client(api_key=api_key)

response = client.models.generate_content(
    model='gemini-2.5-flash',
    contents='Halo Gemini, saya sedang mencoba di Google Colab!',
)
print(response.text)

```

### 3. Perintah Tambahan Colab yang Berguna

* **Melihat File yang Ada di Colab:**
Jika Anda ingin Gemini menganalisis gambar atau dokumen, Anda bisa mengunggah file tersebut ke Colab (klik ikon folder di kiri), lalu cek nama file Anda dengan perintah:
```bash
!ls

```


* **Mengecek Spesifikasi Sistem Colab:**
Jika Anda penasaran Google memberikan Anda spesifikasi komputer seperti apa di cloud (terutama jika Anda mengaktifkan T4 GPU):
```bash
!nvidia-smi

```



Jadi, di Colab Anda cukup fokus jalankan `!pip install google-genai` di *cell* paling atas, lalu sisanya tinggal mainkan kode Python-nya! Mau langsung dicoba untuk membuat sesuatu?

```

```
