# TUTORIAL PUSH PER FEATURE

![GitHub](https://img.shields.io/badge/GitHub-Push&Commit-purple?style=for-the-badge&logo=github)

Tutorial Commit dan Push untuk Tugas Besar Praktikum Pemrograman II

---

## 🗃️ Conventional Commit Message

Ini adalah aturan baku untuk commit message:
- `feat:` -> feature baru ke codebase, validasi baru
- `fix:`  -> memperbaiki (fix) bug di codebase,
             memperbaiki validasi yang sudah ada
- `style:` -> styling halaman
- dll
Masih banyak lagi, tapi yang akan kita gunakan hanya `feat` dan `fix` saja di tugas besar ini.

---

## 🗝️ Panduan Commit dan Push

Ikuti langkah-langkah berikut untuk commit dan push yang ditentukan:

### 1. Pastikan selalu mulai dari branch `dev`
```bash
   git checkout dev
```

### 2. Selalu periksa push terbaru di branch `dev`
```bash
   git pull origin dev
```

### 3. Kerjakan tugasmu, tidak apa-apa untuk memulai di branch `dev`
- Karena untuk commit dan push nantinya kita akan membuat branch baru!

### 4. Jika tugas selesai, saatnya commit & push!

### 5. Di terminal mari buat branch baru terlebih dahulu
- Gunakan nama branch yang konsisten.
- Dalam kasus ini, kita ingin commit & push `KursusView.java` saja
```bash
   git checkout -b feature/view-kursus
```
Jika ingin `KursusController.java`, maka:
```bash
   git checkout -b feature/controller-kursus
```
Jika ingin `Kursus.java`, maka:
```bash
   git checkout -b feature/model-kursus
```
Mengikuti nama entity-nya.

### 6. Tambahkan ke staged-change
- Jika sudah membuat branch, kamu akan otomatis masuk ke branch yang kamu buat.
- Jika ingin push `KursusView.java` saja, maka masukkan `KursusView.java` ke staged change, caranya:
```bash
   git add view/KursusView.java
```
- INGAT! HARUS PAKAI ROOT FOLDER YANG RINCI! SESUAIKAN DENGAN YANG INGIN KALIAN PUSH. Contoh lainnya:
```bash
   git add controller/KursusController.java
```
- Jangan pakai `git add .` secara mentah-mentah!
- Setelah itu gunakan `git status` untuk memeriksa status file yang berada di stage change, pastikan itu ada file yang mau kamu commit & push.
```bash
   $ git status
   On branch main
   Your branch is up to date with 'feature/view-kursus'.
   Changes to be committed:
   Changes to be committed:
   (use "git restore --staged <file>..." to unstage)
         new file:   view/KursusView.java
```
- Nanti akan muncul hasil command seperti diatas.

### 7. Masukkan Pesan Commit!
- Masukkan pesan commit, contohnya:
```bash
   git commit -m "feat: add KursusView Interface"
```
- Jika ingin menambah validasi (sebelumnya belum dibuat)
- Isi pesannya sesuaikan, tapi prefix-nya tetap `feat:`
```bash
   git commit -m "feat: add input validation for KursusController"
```
- Jika ingin mengubah/memperbaiki validasi (sebelumnya sudah dibuat tapi ada kesalahan)
```bash
   git commit -m "fix: prevent empty Nama Kursus field in Data Kursus form"

   Artinya : "Mencegah field Nama Kursus kosong di form Data Kursus"
```

### 8. Push ke GitHub
- Terakhir kita push ke GitHub!
```bash
   git push origin feature/view-kursus
```

### 9. Pull Request
- Sekarang kamu pergi ke Repo GitHub tubes `RancangRupa-pp2-B-2025` dan lakukan pull request
- Nanti akan muncul seperti ini di halaman utamanya:
```bash
 ----------------------------------------------------------------------------------------------------
|                                                                        ------------------------    |
|   feature/view-kursus had recent pushes 40 seconds ago                | Compare & pull request |   |
|                                                                        ------------------------    |
 ----------------------------------------------------------------------------------------------------
```
- Di klik tombol hijau `Compare & pull request`, nanti akan diarahkan ke halaman yang di bagian atasnya ada seperti ini:
```bash
OPEN A PULL REQUEST
Create a new pull request by comparing changes across two branches. If you need to, you can also . Learn more about diff comparisons here.
 ---------------------------------------------------------------------------------------------------------------------
|    ------------      ------------------------------                                                                 |              
|   | base: main | <- | compare: feature/view-kursus |  ✓ Able to merge. These branches can be automatically merged.  |
|    ------------      ------------------------------                                                                 |               
 ---------------------------------------------------------------------------------------------------------------------
```
- Ganti base nya menjadi `base: dev`, lalu klik tombol hijau `Create pull request`
- Lalu laporkan ke grup, biar nanti aku Merge pull request!
- SELESAI!
---


## 👥 Tim Pengembang

Aplikasi Kelasync dikembangkan oleh Kelompok RancangRupa pada Praktikum Pemrograman II Kelas B Tahun 2025, dengan pembagian pengembangan berdasarkan modul dan entitas sistem.

| NIM  | Nama | GitHub Profile | 
|----------|----------|----------|
| `233040065` | Emeralda Iffatud Diana | [Diana-museo](https://github.com/Diana-museo) |
| `233040051` | Haifa Zahirah Ramdhan | [haifazahirahr](https://github.com/haifazahirahr) |
| `233040061` | Ellen Aplida Zalni | [twenteazfour](https://github.com/twenteazfour) |
| `233040086` | Iqbal Nurfikri | [MangEakLur](https://github.com/MangEakLur) |