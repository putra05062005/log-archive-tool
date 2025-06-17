# Log Archive Tool

Ini adalah alat baris perintah (CLI) sederhana yang ditulis dalam Bash untuk mengarsipkan direktori log secara rutin. Skrip ini akan mengompres direktori target ke dalam sebuah file `.tar.gz` dengan nama yang unik berdasarkan tanggal dan waktu.

## Fitur

- Mengarsipkan direktori apa pun yang diberikan sebagai argumen.
- Membuat file arsip `.tar.gz` yang terkompresi untuk menghemat ruang.
- Memberi nama file arsip dengan stempel waktu (timestamp) yang unik untuk menghindari penimpaan file.
- Melakukan validasi input untuk memastikan direktori yang diberikan ada.
- Mudah diinstal dan digunakan di berbagai sistem Linux.

## Instalasi

Untuk menggunakan alat ini di sistem Anda, ikuti langkah-langkah berikut:

1.  **Clone repository ini:**
    ```bash
    git clone [https://github.com/putra05062005/log-archive-tool.git](https://github.com/putra05062005/log-archive-tool.git)
    ```

2.  **Masuk ke direktori proyek:**
    ```bash
    cd log-archive-tool
    ```

3.  **Buat skrip agar bisa dieksekusi:**
    ```bash
    chmod +x log-archive
    ```

4.  **Buat symbolic link** agar perintah bisa dijalankan dari mana saja (disarankan):
    ```bash
    # $(pwd) akan otomatis mengambil path direktori saat ini
    sudo ln -s "$(pwd)/log-archive" /usr/local/bin/log-archive
    ```

## Cara Penggunaan

Jalankan skrip dengan memberikan path ke direktori yang ingin Anda arsipkan.

**Sintaks Dasar:**
```bash
log-archive <path_ke_direktori>
