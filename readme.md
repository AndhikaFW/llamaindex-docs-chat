# Multiple Docs Chat App

Otomasi pengerjaan tugas-tugas emas2 & MultiPDF Chat app.

## Dependency-Dependency & Instalasi
----------------------------
Untuk menginstall aplikasi emas2-bot, ikuti langkah-langkah berikut:

1. Clone repository.

2. Install dependency-dependency yang dibutuhkan dengan menjalankan perintah berikut:
   ```
   pip install -r requirements.txt
   ```

3. Dapatkan API key dari OpenAI dan tambahkan API key serta username dan password sso ke file `.env` di direktori projek.
```commandline
OPENAI_API_KEY=api_key_rahasia_anda
username=username_anda
password=password_anda
question=pertanyaan_dari_bot_setiap_kali_mendapatkan_soal
```

## Penggunaan
-----
Untuk menggunakan aplikasi otomasi emas2-bot, ikuti langkah-langkah berikut:

1. Pastikan dependency-dependency sudah diinstall dan pastikan sudah menambahkan OpenAI API key serta username dan password sso ke file `.env`.

2. Jalankan file `bot-emas2.py` dengan CLI. `Jalankan perintah berikut`:
   ```
   python bot-emas2.py
   ```

3. Aplikasi akan berjalan di CLI.

Untuk menggunakan MultiPDF Chat App, ikuti langkah-langkah berikut:

1. Pastikan dependency-dependency sudah diinstall dan pastikan sudah menambahkan OpenAI API key serta username dan password sso ke file `.env`.

2. Jalankan file `index.py` dengan CLI. `Jalankan perintah berikut`:
   ```
   python index.py
   ```

3. Aplikasi akan muncul di browser default anda, menampilkan GUI.

4. Masukkan dokumen PDF ke aplikasi dengan instruksi yang diberikan.

5. Masukkan pertanyaan secara natural mengenai PDFs dengan chat interface.



## License
-------
The MultiPDF Chat App is released under the [MIT License](https://opensource.org/licenses/MIT).

