↶
↷
Block style
Paragraph
B

I

S
</>
@
-
1.
[]
Kurs - Data Historis GAU/IDR & Saham IDX Bank


Data up-to-date tiap hari - ritual 1 menit buka-tutup Google Sheet 😂


Repo ini auto-update minimal dalam 24 jam setelah Investing.com publish data baru. Kadang cuma butuh 5 detik buka-tutup Sheet, HP mati pun data udah kesync.



🚀 Data Up To Date Tiap Hari


1. GAU/IDR (Emas)
CSV historis dari 18/09/2020 sampai hari ini

GitHub Pages (rekomendasi buat HTML/Dashboard):
  http://wlmyaps.github.io/kurs/Data%20Historis%20GAU_IDR.csv

Raw GitHub (buat script/bot):
  https://raw.githubusercontent.com/wlmyaps/kurs/main/Data%20Historis%20GAU_IDR.csv



Format: Tanggal,Terakhir,Pembukaan,Tertinggi,Terendah,Vol,Perubahan%

Terakhir cek: 02/11/2026 - 2.273.194 (0,13%)



2. Saham IDX Bank - JSON
History 53 emiten + COMPOSITE dari 2025-09-25 s/d hari ini

https://wlmyaps.github.io/kurs/saham1.json



Raw:

https://raw.githubusercontent.com/wlmyaps/kurs/main/saham1.json



Struktur:

{
  "tickers": ["BBCA", "BMRI", "BBRI", ...],
  "history": [
    { "dateStr": "2026-11-02", "prices": { "BBCA": 4980, ... } }
  ]
}


3. Saham - Sheet1 CSV
https://wlmyaps.github.io/kurs/saham%20-%20Sheet1.csv



Raw:

https://raw.githubusercontent.com/wlmyaps/kurs/main/saham%20-%20Sheet1.csv



🛠️ Cara Kerja (Khususheet)


Investing.com -> Cloudflare Worker (khususheet.loveofthegod.workers.dev) 
-> Google Sheet (manual open 1 menit) -> GitHub Repo


Worker dibuat 5 tahun lalu, login via GitHub wlmyaps
Butuh interaksi manusia asli (buka Sheet) biar Cloudflare gak nge-block
Buka Sheet sebelum jam 16:30 WIB = data lama, buka setelah jam 16:30 = data baru ke-push dalam 3 menit
HP mati 5 detik setelah buka pun tetep ke-push, karena proses jalan di server


Kalau suatu hari aku meninggal, data berhenti di tanggal itu 😂


📊 Dashboard Live


https://khususheet.loveofthegod.workers.dev/



Grafik 3D Waterfall GAU/IDR 27 titik harian + tabel warna Close/Open/High/Low



📜 License


Data source: Investing.com (via proxy)

Repo by William Yap - Medan



Last update: 02/11/2026



