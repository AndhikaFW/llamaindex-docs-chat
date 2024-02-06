# Aplikasi MultiDocs Chat

Aplikasi MultiDocs Chat adalah sebuah aplikasi Python yang memungkinkan anda untuk chat dengan banyak dokumen. Anda bisa bertanya tentang dokumen-dokumen yang anda berikan menggunakan bahasa yang natural, dan aplikasi ini akan memberikan respon yang relevan berdasarkan koren dari dokumen-dokumen yang anda berikan. Aplikasi ini menggunakan sebuah _language model_ untuk menghasilkan jawaban yang akurat terhadap permintaan anda.
Perlu diketahui bahwa aplikasi ini hanya merespon pertanyaan yang berhubungan dengan dokumen-dokumen yang anda berikan.

## Dependency-Dependency & Instalasi
----------------------------
Untuk menginstall aplikasi ini, ikuti langkah-langkah berikut:

1. Clone repository:
   ```
   git clone https://github.com/AndhikaFW/llamaindex-docs-chat.git
   ```
2. Masuk ke folder:
   ```
   cd llamaindex-docs-chat
   ```

4. Buat _python virtual environment_:
   ```
   python3 -m venv .venv
   ```
5. Jalankan _python virtual environment_:
   ```
   source .venv/bin/activate  
   ```

3. Install dependency-dependency yang dibutuhkan:
   ```
   pip install -r requirements.txt
   ```

4. Dapatkan API key dari OpenAI dan tambahkan API key serta tanda anda ke file `.env` di direktori projek.
   ```commandline
   OPENAI_API_KEY=api_key_rahasia_anda
   mark="tanda_anda"
   ```

## Penggunaan
-----
Untuk menggunakan aplikasi ini, ikuti langkah-langkah berikut:

1. Pastikan dependency-dependency sudah diinstall dan pastikan sudah menambahkan OpenAI API key serta tanda anda ke file `.env`.

2. Jalankan _python virtual environment_:
   ```
   source .venv/bin/activate  
   ```

3. Jalankan file `main.py` dengan CLI. `Jalankan perintah berikut`:
   ```
   #Untuk Lokal
   uvicorn main:docs_chat --reload

   #Untuk Server #.#.#.# diisi dengan ip tujuan dan #### diisi dengan port yang kosong
   uvicorn main:docs_chat --host #.#.#.# --port ####
   ```

4. Aplikasi akan muncul di browser default anda, menampilkan GUI.

5. Masukkan dokumen ke aplikasi dengan instruksi yang diberikan.

6. Masukkan pertanyaan secara natural mengenai PDFs dengan chat interface.



## License
-------
 Aplikasi MultiDocs Chat dirilis dibawah [Lisensi MIT](https://opensource.org/licenses/MIT).

