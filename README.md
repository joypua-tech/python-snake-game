JUDUL UTAMA:
Python Snake Game

PENDAHULUAN
Aplikasi Snake Game ini dibuat sebagai hiburan dan dibuat menggunakan Python dengan modul turtle, random, dan time. Game ini mensimulasikan pergerakan ular dalam sebuah arena dengan tujuan mengumpulkan makanan dan meningkatkan skor. Setiap bagian program memiliki fungsi penting untuk menciptakan gameplay yang responsif dan interaktif

PANDUAN INSTALASI:
1. Menginstal dan Menyiapkan Python
Untuk menjalankan program Snake Game berbasis Turtle, kamu harus memiliki Python versi
3.x. Python dapat diunduh dari situs resmi Python. maka Python sudah terinstal.
2. Membuat Folder Kerja
Buat folder baru untuk menyimpan program Snake Game. Contoh nama folder:
SnakeGame. Folder ini bebas kamu buat di mana saja, misalnya di Desktop atau Documents.
3. Membuat File Program Python
Setelah folder siap, buat file .py untuk menampung kode program. Caranya:
1. Buka aplikasi editor seperti: Visual Studio Code (disarankan), IDLE Python
2. Buat file baru.
3. Salin seluruh kode Snake Game yang sudah kamu berikan sebelumnya.
4. Simpan dengan nama: snake_game.py
Pastikan file disimpan dalam folder SnakeGame
4. Mengecek Modul yang Diperlukan
Program kamu menggunakan tiga modul Python: turtle, random, time. Semua modul tersebut
sudah tersedia secara default pada Python. Jadi, kamu tidak perlu menginstal apa pun

PANDUAN MENJALANKAN PROGRAM
Ada dua cara utama untuk menjalankan file Python tersebut.

A. Menjalankan Melalui Command Prompt (CMD)
1. Buka Command Prompt.
2. Arahkan CMD ke folder SnakeGame.
Contoh perintah jika folder berada di Desktop:
cd C:\Users\NamaUser\Desktop\SnakeGame
3. Jalankan program dengan perintah: python snake_game.py
Jika Python terdeteksi, jendela game akan muncul otomatis.

B. Menjalankan Melalui Visual Studio Code
1. Jalankan VS Code.
2. Klik File → Open Folder → pilih folder SnakeGame.
3. Klik file snake_game.py.
4. Tekan tombol Run (ikon segitiga ►) di kanan atas.
Atau tekan F5 pada keyboard.
Jendela Turtle akan muncul dan game langsung berjalan.

Dokumentasi Teknis Flowchart
```mermaid
flowchart TD
   A([Start]) --> B[Inisialisasi Window & Variabel]
   B --> C[Inisialisasi Border Permainan]
   C --> D[Inisialisasi Head Snake]
   D --> E[Inisialisasi Food (random warna & bentuk)]
   E --> F[Inisialisasi Scoreboard]
   F --> G[Set Key Input (Up/Down/Left/Right)]
   G --> H{Mulai Loop Utama}

   %% LOOP UTAMA
   H --> I[Update Layar]

   %% CEK TABRAKAN DINDING
   I --> J{Snake\nmenabrak dinding?}
   J -->|Ya| K([GAME OVER]\nTampilkan skor)
   J -->|Tidak| L[Cek apakah head menyentuh food]

   %% CEK MAKAN FOOD
   L --> M{Distance < 20?}
   M -->|Ya| N[Tambah score\nUpdate high score]
   N --> O[Generate food baru (posisi & warna random)]
   O --> P[Tambah segment baru]
   P --> Q[Update scoreboard]
   Q --> R[Gerakkan ekor snake]
   M -->|Tidak| R

   %% PERGERAKAN SNAKE
   R --> S[Gerakkan head sesuai arah]

   %% CEK TABRAKAN BADAN
   S --> T{Head menabrak badan?}
   T -->|Ya| K
   T -->|Tidak| U[time.sleep(delay)]

   U --> H

   %% END
   K --> V([End])
```

Kontributor
Kontributor
| No | Nama Lengkap | NIM | Akun GitHub | Peran |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| 1 | Joy Pua  | 250211060120  | (https://github.com/p4seppp)  | Project Maintainer  |
| 2 | Junior Palilingan Jacobis  | 250211060129  | (https://github.com/juniorjac496-max/jun.git)  | Contributor  |
| 3 | Gamaliel Calvyn Hizkia Kaligis  | 250211060123  | (https://github.com/praisemandolang)  | Contributor  |


  
