# Sesi 2: Latihan Git dan GitHub (1.2)

## Konfigurasi Kelompok

**Nama Kelompok:** Beda Tuhan, Satu Tujuan

**Anggota Kelompok:**
1. Brian Zakariya
2. Benaya Yoyada

---

## Latihan 2.1: Instalasi dan Identitas Git (15 Menit)

Setelah proses instalasi Git selesai, kami melakukan pengecekan versi Git melalui terminal menggunakan perintah berikut:

```bash
git --version
```

**Hasil:**
```bash
git version 2.56.0.windows.4
```

Selanjutnya, kami melakukan konfigurasi identitas Git secara global dengan mengatur nama pengguna (*username*) dan alamat email. Identitas ini akan digunakan sebagai informasi pembuat setiap commit.

**Konfigurasi nama dan email:**

```bash
git config --global user.name "Brian Zakariya"
git config --global user.email "brianzakariya@gmail.com"
```

Untuk memastikan konfigurasi berhasil diterapkan, kami memeriksa hasilnya menggunakan perintah:

```bash
git config --list
```

**Hasil konfigurasi:**
```bash
user.name=Brian Zakariya
user.email=brianzakariya@gmail.com
```

Dengan demikian, konfigurasi identitas Git telah berhasil dilakukan.

---

## Latihan 2.2: Repository Pertama, Hello World (30 Menit)

Pada latihan ini, kami membuat repository pertama bernama `hello-world` melalui GitHub. Repository dibuat dalam keadaan kosong tanpa menambahkan file `README.md` secara otomatis dari GitHub.

Setelah itu, kami membuat folder proyek secara lokal dan menginisialisasi Git repository menggunakan perintah:

```bash
git init
```

**Hasil:**
```bash
Initialized empty Git repository in C:/Users/benay/OneDrive/Desktop/hello-world/.git/
```

### 1. Membuat File Proyek

Setelah repository berhasil diinisialisasi, kami membuat dua file di dalam folder proyek, yaitu:

- `index.html` sebagai file utama proyek.
- `README.md` sebagai dokumentasi proyek.

### 2. Menambahkan dan Melakukan Commit

Selanjutnya, kami menambahkan seluruh file ke staging area menggunakan perintah:

```bash
git add .
```

Kemudian, kami menyimpan perubahan tersebut ke dalam Git menggunakan perintah commit:

```bash
git commit -m "ini commit pertama ku dari benaya"
```

**Hasil commit:**
```bash
[master (root-commit) 5724852] ini commit pertama ku dari benaya
 2 files changed, 12 insertions(+)
 create mode 100644 README.md
 create mode 100644 index.html
```

### 3. Menghubungkan Repository Lokal dengan GitHub

Setelah commit berhasil dibuat, kami menghubungkan repository lokal dengan repository GitHub menggunakan perintah:

```bash
git remote add origin https://github.com/mausukses/hello-world.git
```

Perintah tersebut digunakan untuk menambahkan repository GitHub sebagai remote dengan nama `origin`.

### 4. Mengunggah Proyek ke GitHub

Langkah terakhir adalah mengunggah file dan riwayat commit dari repository lokal ke GitHub menggunakan perintah:

```bash
git push -u origin master
```

**Hasil push:**
```bash
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 490 bytes | 163.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/mausukses/hello-world.git
 * [new branch]      master -> master
branch 'master' set up to track 'origin/master'.
```

Berdasarkan hasil tersebut, proses push berhasil dilakukan. Branch `master` pada repository lokal juga telah terhubung dengan branch `master` pada repository GitHub.

**Repository GitHub:** https://github.com/mausukses/hello-world

---