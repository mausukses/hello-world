# Sesi 2: Latihan Git dan GitHub (1.2)

## Konfigurasi Kelompok
Kelompok: Beda Tuhan, satu tujuan

Anggota:

Brian Zakariya

Benaya Yoyada

## Latihan 2.1: Instalasi dan identitas (15 menit)
setelah kami menginstall Git, kami menjalankan `git --version` pada terminal.
```bash
git --version
git version 2.56.0.windows.4
```

setelah itu, kami melakukan atau membuat konfigurasi untuk Nama dan juga Email dengan perintah seperti `config --global user.name "Nama Anda"` untuk konfigurasi nama, dan  `git config --global user.email "email@contoh.com"` untuk konfigurasi email.
```bash
git config --global user.name "Brian Zakariya"   
git config --global user.email "brianzakariya@gmail.com"
```
dan tidak lupa kita cek hasil konfigurasi tersebut dengan menggunakan `git config --list`
```bash
user.name=Brian Zakariya
user.email=brianzakariya@gmail.com
```

## Latihan 2.2: Repository pertama, hello-world (30 menit)
kami telah mmbuat sebuah repository kosong bernama hello-world di github tanpa File README.md dari github. setlah itu tidak lupa kami membuat folder "hello-world", dan melakukan `git init`
```bash
git init                            
Initialized empty Git repository in C:/Users/benay/OneDrive/Desktop/hello-world/.git/
```

setelah kita membuat file index.php, beserta README.md beserta isianya. kita melakukan perintah `git add .`, `git commit -m "first commit".`
```
 git add .
PS C:\Users\benay\OneDrive\Desktop\latihan-git> git commit -m "ini commit pertama ku dari benaya"
[master (root-commit) 5724852] ini commit pertama ku dari benaya
 2 files changed, 12 insertions(+)
 create mode 100644 README.md
 create mode 100644 index.html
PS C:\Users\benay\OneDrive\Desktop\latihan-git> git remote add origin https://github.com/mausukses/hello-world.git
PS C:\Users\benay\OneDrive\Desktop\latihan-git> git push -u  origin master
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 490 bytes | 163.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/mausukses/hello-world.git
 * [new branch]      master -> master
branch 'master' set up to track 'origin/master'. brian gantenga

aku updat readmenya