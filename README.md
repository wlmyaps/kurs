Kurs - Data Historis GAU/IDR & Saham IDX Bank

Data up-to-date tiap hari - ritual 1 menit buka-tutup Google Sheet 😂

Repo ini auto-update minimal dalam 24 jam. Kadang cuma butuh 5 detik buka-tutup Sheet, HP mati pun data udah kesync.

🚀 Data Up To Date Tiap Hari

1. GAU/IDR (Emas)
CSV historis dari 18/09/2020 sampai hari ini

GitHub Pages (rekomendasi buat HTML/Dashboard):
http://wlmyaps.github.io/kurs/Data%20Historis%20GAU_IDR.csv

Raw GitHub (buat script/bot):
https://raw.githubusercontent.com/wlmyaps/kurs/main/Data%20Historis%20GAU_IDR.csv

Format: Tanggal,Terakhir,Pembukaan,Tertinggi,Terendah,Vol,Perubahan%
Last check: 02/11/2026 - 2.273.194 (0,13%)

2. Saham IDX Bank - JSON
History 53 emiten + COMPOSITE
https://wlmyaps.github.io/kurs/saham1.json

Raw:
https://raw.githubusercontent.com/wlmyaps/kurs/main/saham1.json

3. Saham - Sheet1 CSV
https://wlmyaps.github.io/kurs/saham%20-%20Sheet1.csv

Raw:
https://raw.githubusercontent.com/wlmyaps/kurs/main/saham%20-%20Sheet1.csv

🛠️ Cara Kerja (Khususheet)

Cloudflare Worker (khususheet.loveofthegod.workers.dev) 
-> Google Sheet (manual open 1 menit) -> GitHub Repo

Worker dibuat 5 tahun lalu
Butuh interaksi manusia asli (buka Sheet) - 1 menit ritual
Buka Sheet sebelum jam 16:30 WIB = data lama, buka setelah jam 16:30 = data baru ke-push dalam 3 menit

Kalau suatu hari aku meninggal, data berhenti di tanggal itu 😂

📊 Dashboard Live

https://khususheet.loveofthegod.workers.dev/

Grafik 3D Waterfall GAU/IDR 27 titik harian + tabel warna Close/Open/High/Low

📜 Catatan

Data dikumpulkan dari data pasar publik untuk keperluan edukasi & riset pribadi
Bukan saran finansial
Repo by William Yap - Medan

Last update: Senin s/d Jumat (hari bursa)
