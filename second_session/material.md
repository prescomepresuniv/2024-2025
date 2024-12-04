# 🚀 Pengantar Git dan GitHub

Selamat datang di pertemuan klub kita! 🎉

Hari ini, kita akan mempelajari dasar-dasar Git dan GitHub. Git adalah alat kontrol versi (version control) yang sangat populer untuk mengelola kode secara kolaboratif, sementara GitHub adalah platform untuk menyimpan dan berbagi repositori Git secara online.

---

## 📖 Daftar Isi
1. [Prasyarat](#-prasyarat)
2. [Dasar Git](#dasar-git)
    - [Apa itu Git?](#apa-itu-git)
    - [Apa itu GitHub?](#apa-itu-github)
3. [Perintah Dasar Git](#perintah-dasar-git)
    - [Membuat Repositori Baru](#-membuat-repositori-baru)
    - [Menarik (Pull) Perubahan](#-menarik-pull-perubahan)
    - [Melihat Status Repositori](#-melihat-status-repositori)
4. [Branch dan Merge](#branch-dan-merge)
    - [Apa itu Branch?](#-apa-itu-branch)
    - [Membuat Branch Baru](#-membuat-branch-baru)
    - [Berpindah Branch](#-berpindah-branch)
    - [Menggabungkan Branch (Merge)](#-menggabungkan-branch-merge)
5. [Kolaborasi di GitHub](#kolaborasi-di-github)
    - [Mengkloning Repositori](#-mengkloning-repositori)
6. [Cara Membuat Pull Request](#cara-membuat-pull-request)
    - [Membuat dan Mengelola Pull Request](#-membuat-dan-mengelola-pull-request)
7. [Latihan](#latihan)
8. [Referensi](#-referensi)

---

## 📋 Prasyarat
Sebelum memulai, pastikan Anda telah:

Menginstal Git di komputer Anda (bisa diunduh di git-scm.com).
Memiliki akun GitHub (daftar di github.com).
Mengerti dasar CLI (Command Line Interface) untuk menjalankan perintah Git.

---

## Dasar Git
### Apa itu Git?
Git adalah alat version control yang memungkinkan pengembang melacak perubahan pada kode mereka. Dengan Git, Anda dapat:
1. Mengelola versi kode tanpa kehilangan data.
2. Berkerja secara tim dengan alat yang mendukung kolaborasi.
3. Rollback ke versi kode sebelumnya jika terjadi kesalahan.

---

### Apa itu GitHub?
GitHub adalah platform berbasis web untuk menyimpan repositori Git secara online. Fungsinya meliputi:
- Membagikan kode.
- Kolaborasi tim melalui pull request dan issues.
- Deployment otomatis melalui integrasi.

---

## Perintah Dasar Git
### 🔹 Membuat Repositori Baru
1. Inisialisasi Git di folder proyek Anda:

```bash
git init
```
> Perintah ini membuat repositori Git lokal di folder Anda.

2. Menambahkan file ke repositori:

```bash
git add <nama_file>      # Tambahkan file tertentu
git add .                # Tambahkan semua file
```

3. Commit file:

```bash
git commit -m "Pesan commit pertama"
```

4. Membuat koneksi ke repositori GitHub (opsional):

```bash
git remote add origin https://github.com/username/nama-repo.git
```

5. Push ke repositori GitHub:

```bash
git push -u origin main
```

---

### 🔹 Menarik (Pull) Perubahan
Untuk mengambil perubahan terbaru dari repositori GitHub:

```bash
git pull origin main
```

---

### 🔹 Melihat Status Repositori
Untuk memeriksa status file (terubah, belum di-track, atau siap di-commit):

```bash
git status
```

---

## Branch dan Merge
### 🔹 Apa itu Branch?
Branch adalah cabang yang memungkinkan Anda mengerjakan fitur baru tanpa mengganggu kode utama. Branch default biasanya bernama `main`.

---

### 🔹 Membuat Branch Baru
```bash
git branch nama-branch
```

---

### 🔹 Berpindah Branch
```bash
git checkout nama-branch
```
> Tips: Gunakan perintah gabungan untuk membuat dan langsung berpindah ke branch:

```bash
git checkout -b nama-branch
```

---

### 🔹 Menggabungkan Branch (Merge)
Jika branch sudah selesai dikerjakan, gabungkan kembali ke branch utama:

1. Pindah ke branch `main`:

```bash
git checkout main
```
2. Gabungkan branch:

```bash
git merge nama-branch
```

---

## Kolaborasi di GitHub
### 🔹 Mengkloning Repositori
Jika ingin bekerja pada repositori yang sudah ada di GitHub:

```bash
git clone https://github.com/username/nama-repo.git
```

---

## Cara Membuat Pull Request
### 🔹 Membuat dan Mengelola Pull Request
Pull request digunakan untuk memberi tahu tim Anda bahwa Anda ingin menggabungkan perubahan ke branch utama.

1. Buat perubahan di branch Anda.
2. Push perubahan ke branch Anda di GitHub:
```bash
git push origin nama-branch
```
3. Buka GitHub, buka repositori, dan klik tombol "Compare & pull request".
4. Jelaskan perubahan yang Anda buat dan klik "Create pull request."

---

## Latihan
1. Buat repositori Git lokal, tambahkan file README.md, dan lakukan commit pertama.
2. Buat branch baru untuk fitur login dan tambahkan file login.js.
3. Gabungkan branch login ke branch main.
4. Push repositori lokal Anda ke GitHub.
5. Buat pull request untuk perubahan yang Anda buat.

---

## 🔗 Referensi
- [Dokumentasi Git](https://git-scm.com/doc)
- [Panduan GitHub](https://docs.github.com/en/get-started)

---

Jika ada yang belum jelas, mari diskusikan selama sesi atau tanyakan melalui grup kita. 😊