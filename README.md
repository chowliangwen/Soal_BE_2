# Bookstore App

Repo ini berisi test assignment untuk calon Back-End Engineer

## Struktur Repo dan Dokumen Tambahan

| path                                                                                                                     | content             | description                                 |
| ------------------------------------------------------------------------------------------------------------------------ | ------------------- | ------------------------------------------- |
| ./bookstore_web                                                                                                          | compiled angular FE | Web tampilan sebagai sarana validasi test   |
| [API Requirement Docs](https://docs.google.com/document/d/1QqWf7nDTHwEueuxcDGuaiMP09JADxrFczlEdmtHj_0k/edit?usp=sharing) | Google Docs Link    | Docs berisi Kriteria API yang harus di buat |

## Tentang Assignment

1. Buat aplikasi Back-End sesuai kriteria [API Requirement Docs](https://docs.google.com/document/d/1QqWf7nDTHwEueuxcDGuaiMP09JADxrFczlEdmtHj_0k/edit?usp=sharing) dengan Framework sesuai preferensi masing-masing.
2. Test Jalan API yang sudah di buat di local dengan menggunakan Web yang ada di repo ini. ( cara installasi dan running ada di bawah )
3. Batas waktu pengerjaan 5 hari, setelah itu kirim Email ke: steven@econolab.co.id berisi :

   Subject :

   ```
   NAMA - POSISI - HASIL TEST
   ```

   Isi :

   ```
   Nama : Anon
   Posisi : Back-End 2
   Repo : https://github.com
   Keterangan : ( Penjelasan singkat tentang Framework yang di pakai, db yang dipakai, atau teknologi lain yang di pakai, dll )

   ```

   Attachment

   ```
   - Diagram struktur DB
   - dll
   ```

## Running Web Tampilan di Local

Note : Web memerlukan API sesuai ketentuan untuk bisa berjalan.

Step instalasi :

1. Pertama kalian perlu set-up `Node.JS` di local machine. Silahkan buka [Link Download Node.JS](https://nodejs.org/en/download/) dan Install ke Local machine jika belum ada.
2. Lalu install [lite-server](https://github.com/johnpapa/lite-server) globally dengan `npm` sebagai web server lewat command :

```
# run on command prompt/terminal

npm install --global lite-server
```

3. Lalu buka file `"/bookstore_web/assets/project_config.json"` dan ganti value "Main_Url" sesuai url root API kalian

```
{
    "Main_URL": YOUR API URL HERE
}
```

4. Set up `port` untuk web nya

- Buka file `"/bookstore_web/bs-config.json"`
- Edit `port` sesuai kebutuhan (biasa 3000)

5. Setelah selesai, buka command prompt, set lokasi command prompt di root folder repository dan jalankan command :

```
lite-server -c bs-config.json

# Perlu berada di dalam folder /bookstore_web untuk menjalankan command
```

6. Ketika selesai eksekusi web akan terbuka otomatis di browser default dan dapat diakses di `http://localhost:YourAssignedPort` (port sesuai settingan). Kalian bisa jalankan API yang sudah di buat dan mulai test final dengan web ini
