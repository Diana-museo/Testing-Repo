# TUTORIAL PUSH PER FEATURE

![GitHub](https://img.shields.io/badge/GitHub-Push & Commit-purple?style=for-the-badgelogo=github)

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

### 4. Tambahkan ke staged-change
- Jika sudah membuat branch, kamu akan otomatis masuk ke branch yang kamu buat.
- Jika ingin push `KursusView.java` saja, maka masukkan `KursusView.java` ke staged change, caranya:
```bash
   git add view/KursusView.java
```
- INGAT! HARUS PAKAI ROOT FOLDER YANG RINCI! SESUAIKAN DENGAN YANG INGIN KALIAN PUSH. Contoh lainnya:
```bash
   git add controller/KursusController.java
```
- Setelah itu gunakan `git status` untuk memeriksa status file yang berada di stage change, pastikan itu ada file yang mau kamu commit & push.
```bash
   $ git status
   On branch main
   Your branch is up to date with 'feature/view-kursus'.
   Changes to be committed:
   Changes to be committed:
   (use "git restore --staged <file>..." to unstage)
         new file:   view/KursusView.txt
```
- Nanti akan muncul hasil command seperti diatas.


---

## 👥 Tim Pengembang

Aplikasi Kelasync dikembangkan oleh Kelompok RancangRupa pada Praktikum Pemrograman II Kelas B Tahun 2025, dengan pembagian pengembangan berdasarkan modul dan entitas sistem.

| NIM  | Nama | GitHub Profile | 
|----------|----------|----------|
| `233040065` | Emeralda Iffatud Diana | [Diana-museo](https://github.com/Diana-museo) |
| `233040051` | Haifa Zahirah Ramdhan | [haifazahirahr](https://github.com/haifazahirahr) |
| `233040061` | Ellen Aplida Zalni | [twenteazfour](https://github.com/twenteazfour) |
| `233040086` | Iqbal Nurfikri | [MangEakLur](https://github.com/MangEakLur) |