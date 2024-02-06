# EMAS2-BOT

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


## How It Works
------------

![MultiPDF Chat App Diagram](./docs/PDF-LangChain.jpg)

The application follows these steps to provide responses to your questions:

1. PDF Loading: The app reads multiple PDF documents and extracts their text content.

2. Text Chunking: The extracted text is divided into smaller chunks that can be processed effectively.

3. Language Model: The application utilizes a language model to generate vector representations (embeddings) of the text chunks.

4. Similarity Matching: When you ask a question, the app compares it with the text chunks and identifies the most semantically similar ones.

5. Response Generation: The selected chunks are passed to the language model, which generates a response based on the relevant content of the PDFs.


## License
-------
The MultiPDF Chat App is released under the [MIT License](https://opensource.org/licenses/MIT).

