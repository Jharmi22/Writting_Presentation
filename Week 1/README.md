# Writting_Presentation

## Unix Command Line
* Command Line Interface merupakan jenis shell yang berbasis teks 
* Shell merupakan program yang digunakan untuk berkomunikasi atau memerintah sistem
* Terminal Emulator merupakan aplikasi untuk mengakses Command Line Interface
* Filesytem berfungsi untuk mengatur data yang disimpan dalam sebuah system

### Command untuk navigasi
- pwd digunakan untuk melihat posisi directory saat ini
- ls digunakan untuk melihat isi file yang ada di sebuah directory
- cd digunakan untuk berpindah directory

### Command untuk membuat file dan directory
- touch digunakan untuk membuat sebuah file
- mkdir digunakan untuk membuat directory

### Command untuk melihat isi
- head digunakan untuk melihat beberapa line awal dari sebuah file text
- tail digunakan untuk melihat beberapa line akhir dari sebuah file text
- cat digunakan untuk melihat isi keseluruhan isi sebuah file

### Command untuk menyalin, memindahkan, dan menghapus file dan directory
- cp digunakan untuk menyalin file atau directory
- mv digunakan untuk memindahkan file atau directory atau mengubah file dan directory
- rm digunakan untuk menghapus file dan directory

## GIT dan GITHUB
- GIT adalah tools untuk programmer
- GIT berfungsi sebagai version control system
- Version control system memiliki tugas untuk mencatat setiap perubahan pada file pada suatu proyek baik dikerjakan secara individu maupun tim
- Dengan menggunakan GIT dan GitHub, maka dapat memudahkan dalam bekerja dalam sebuah tim
- Tujuan dari GIT dan GitHub, agar dapat berkolaborasi dalam mengerjakan proyek yang sama tanpa harus melakukan copy paste pada sebuah aplikasi

### A. Instalasi GIT
- konfigurasi GIT
```
git config global user.name "jharmi"
git config global user.email krn.pasangkin@gmail.com
```
- Melihat hasil konfigurasi 
```
git config --list
```

### B. Repository Git
- Membuat repository (didalam folder yang dibuat)
```
git init
```
- Melihat apakah terjadi perubahan atau tidak pada GIT
```
git status
```
- Menambah file baru atau file yang telah diubah pada GIT
```
git add
git add .
```
- Menyimpan perubahan pada GIT
```
git commit -m
```
### C. Riwayat atau History GIT
- Melihat riwayat atau history pada GIT
```
git log
```
### D. Command 
- Untuk menampilkan log yang lebih pendek
```
git log --oneline
```
- Untuk melihat log dari file tertentu
```
git log index.
```
- Untuk berpindah branch
```
git checkout
```
- Untuk membuat branch baru
```
git branch -b [namabranch]
```
- Untuk menyatukan vranch cabang fitur yang telah dikembangkan
```
git merge origin
```

## HTML




