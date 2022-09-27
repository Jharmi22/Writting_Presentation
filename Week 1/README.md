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
- HTML atau *Hypertext Markup Language*, digunakan untuk menampilkan konten pada browser
- Tools yang digunakan untuk membuat HTML adalah Browser dan Code Editor
### A. Struktur HTML
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title></title>
</head>
<body>
</body>
</html>
```
- Element HTML
    - Opening tag: `<p>`
    - Closing tag: `</p>`
- Atribut pada HTML adalah properties dari sebuah HTML Element. contohnya id, class, name
- HTML Comment, digunakan digunakan untuk menjelaskan line code tertentu namun, comment ini tidak dapat di eksekusi atau tidak dapat mengubah codingan hanya sebagai catatan bagi proggrammer
`<!--  -->`
- Membuat Tabel
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <table border="1">
        <thead>
            <tr>
                <td><b>Nama</b></td>
                <td><b>Umur</b></td>
                <td><b>Universitas</b></td>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>Jharmi</td>
                <td>20</td>
                <td>Universitas Mulawarman</td>
            </tr>
        </tbody>
    </table>
</body>
</html>
```
- Semantic HTML yaitu menggunakan element HTML yang sesuai dengan kebutuhan konten. element semantik seperti `<header>`, `<aside>`, `<footer>`, `<article>`, dan sebagainya
```
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <title>Contoh Tampilan dengan Elemen Semantik</title>
</head>

<body>

  <header>
    <h1>Belajar Element Semantik di HTML</h1>
  </header>

  <nav>
    <a href="#">Home</a> |
    <a href="#">About</a> |
    <a href="#">Contact</a>
  </nav>

  <article>
    <h1>Tutorial Semantik Elemen untuk Pemula</h1>
    <p>Semantic HTML yaitu menggunakan element HTML yang sesuai dengan kebutuhan konten. element semantik seperti header, aside, footer, article, dan sebagainya
    </p>
  </article>

  <footer>
    Copyright &copy; 2022 by Jharmii
  </footer>

</body>

</html>
```
## CSS
- CSS atau *Cascanding Style Sheet* adalah bahasa yang digunakan untuk mendesain halaman website
### A. Struktur CSS
 ```
 .elementHTML{  
    property : value }
 ```






