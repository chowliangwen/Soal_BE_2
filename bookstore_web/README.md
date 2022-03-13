# Web View Bookstore

Merupakan web view simple sebagai sarana test dan validasi API Bookstore.

## Running Web Tampilan di Local

Note : Web memerlukan API sesuai ketentuan untuk bisa berjalan.

Step instalasi :

1. Pertama kalian perlu set-up `Node.JS` di local machine. Silahkan buka [Link Download Node.JS](https://nodejs.org/en/download/) dan Install ke Local machine jika belum ada.
2. Lalu install [lite-server](https://github.com/johnpapa/lite-server) globally dengan `npm` sebagai web server lewat command :

```
# run on command prompt/terminal

npm install --global lite-server
```

3. Lalu buka file `"/assets/project_config.json"` dan ganti value "Main_Url" sesuai url root API kalian

```
{
    "Main_URL": YOUR API URL HERE
}
```

4. Set up `port` untuk web nya

- Buka file `"/bs-config.json"`
- Edit `port` sesuai kebutuhan (biasa 3000)

5. Setelah selesai, buka command prompt, set lokasi command prompt di root folder repository dan jalankan command :

```
lite-server -c bs-config.json

# Perlu berada di dalam folder /bookstore_web untuk menjalankan command
```

6. Ketika selesai eksekusi web akan terbuka otomatis di browser default dan dapat diakses di `http://localhost:YourAssignedPort` (port sesuai settingan). Kalian bisa jalankan API yang sudah di buat dan mulai test final dengan web ini
