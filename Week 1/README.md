# Writting_Presentation Week 1

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
 - Ada 3 cara menggunakan CSS
    - Inline tag, menggunakan CSS pada attribute element HTML
     ```
    <p style = "color : blue"> Ini adalah paragraph.</p>
     ```
    - Internal tag, menggunakan CSS dibagian head
     ```
    <!DOCTYPE html>
    <html>
    <head>
    <style>
    body {background-color: powderblue;}
    h1 {color: blue;}
    p {color: red;}
    </style>
    </head>
    <body>

    <h1>This is a heading</h1>
    <p>This is a paragraph.</p>

    </body>
    </html>

     ```
    - External tag, menggunakan file CSS terpisah dengan HTML
    ```
    <!DOCTYPE html>
    <html>
    <head>
    <link rel="stylesheet" href="mystyle.css">
    </head>
    <body>

    <h1>This is a heading</h1>
    <p>This is a paragraph.</p>

    </body>
    </html>
     ```
 - Mengakses file .CSS di HTML
 ```
 <link href="styles.css" type="text/css" rel="stylesheet"/>
 ```
 - Tag name, jika menggunakan tag element HTML secara langusng pada CSS maka akan bersifat global atau dapat mempengaruhi seluruh tag element HTML yang ada pada file tersebut
 - Tag Id dan Tag Class bisa digunakan di CSS namun Tag Class lebih bersifat fleksibel karena dapat diberikan lebih dari 1 nilai sedangkan Tag Id bersifat kaku karena hanya memiliki 1 nilai. Contohnya dapat digunakan pada navigation dan footer.
 - Nested Element yaitu setiap element yang terdiri atas parent dan child
 - !important CSS berada di level paling atas dari ID dan Class, artinya jika pada styling CSS  di gunakan !important, maka styling sebelumnya baik itu ID Name atau Class Name akan di override.
## Flexbox
- Flexbox adalah cara untuk mengatur layout/tata letak
- Flexbox memiliki 1 parent/container dan bisa beberapa child/item
- Flex-directon digunakan untuk mengatur tata letak itemchild
- Flex-wrap membuat atau mengatur tata letak item child dalam 1 line
- Flex-flow digunakan sebagai shortcut untuk set up flex-direction dan flex-wrap bersamaan
- Order pada flex berfungsi untuk ordering item mana yang ingin kita atur posisinya berdasarkan urutan order
- justify-content digunakan untuk mengatur tata letak dan space antar item child secara horizontal atau main axis
- align-items digunakan untuk mengatur align dari item child secara vertikal atau cross axis
- align-self digunakan untuk mengatur align item pada masing-masing item
- align-content digunakan untuk mengatur tata letak dan space antar item child secara vertikal atau cross axis
- flex-grow dapat mengatur size suatu item child pada flexbox
- flex-shrink adalah properti yang membuat size suatu item child mengecil secara relatif terhadap item child yang lainnya
- flex-basis mengatur width dari setiap item child

## Algoritma & Pseudocode
### Algoritma
- Algoritma adalah deskripsi berupa step-step yang dibutuhkan untuk menyelesaikan suatu masalah
- Kualitas Algorima
    - Input dan output harus didefinisikan terlebih dahulu dengan tepat
    - Setiap step harus benar-benar clear dan tidak ambigu
    - Algoritma seharusnya tidak mengandung suatu code pada bahasa pemograman tertentu. 
    - Algoritma harus dibuat agar dapat digunakan dalam bahasa pemograman apapun.
- Alasan mempelajari algoritma
    - Programming itu adalah algoritma dan struktur data
    - Data struktur digunakan untuk mengelola/manajemen sebuah data
    - Dan Algoritma yang akan menyelesaikan suatu permasalahan menggunakan data tersebut.
- Contoh Algoritma 
```
Kalkulator sederhana 

- Inisialisaikan bil, oprs, hasil
- Input nilai X
- Pilih salah satu operasi dari (+),(-),(x),(:)

- Input nilai X
- Jika anda memilih operasi (+), maka hasil = X + X
- Jika anda memilih operasi (-), maka hasil = X - X
- Jika anda memilih operasi (x), maka hasil = X * X
- Jika anda memilih operasi (:), maka hasil = X : X
- Cetak hasil
```

### Pseudocode
- Pseudocode adalah menuliskan algoritma dengan umumnya bahasa inggris sebelum kita implementasikan ke bahasa pemograman tertentu
- Panduan menulis pseudocode
```
1. Menggunakan huruf besar pada kata kunci 
2. 1 statement hanya 1 baris
3. Menggunakan identitas
4. Harus spesifik
5. Simpel
```
- Contoh Pseudocode
```
Program Menghitung Persegi Panjang

Deklarasi
var panjang, lebar, luas : integer;
Implementasi 
Read(panjang);
Read(lebar);
luas ← panjang*lebar;
Write (luas);
```
- Jenis pseudocode
    - Procedural adalah cara berpikir secara runtun. Artinya serangkaian perintah yang berurutan
    - Conditional digunakan saat dibutuhkan percabangan kasus. Komputer akan melakukan suatu tindakan jika suatu kondisi terpenuhi
    - Looping, sebuah proses yang sama berulang-ulang
    - Recursive adalah pola pikir dalam algoritma yang memanggil method/function didalam sebuah function

## JavaScript Dasar
- Javascript adalah bahasa pemograman yang sangat powerful yang digunakan untuk logic pada sebuah website selain itu Javascript juga dapat membuat website menjadi interaktif dan dinamis
- Javascript dijalankan melalui browser pada device setiap user, browser yang paling umum digunakan adalah mozilia dan google chrome
- Syntax adalah sesuatu yang dapat diibaratkan sebagai kamus dan berperan dalam mengatur tata cara dalam bahasa pemrograman. Syntax digunakan untuk membuat statement program, instruksi untuk dijalankan atau dieksekusi oleh web browser dan compiler
- Contoh syntax JavaScript
    - alert()
    - prompt()
    - confirm()
- Console log adalah tempat untuk memeriksa logic pemograman web yang kita kembangkan, juga tempat untuk melakukan debugging (mengetahui error pada code) pada pemograman web
- Comments adalah sintaks yang digunakan untuk memberi keterangan tentang suatu statement. Menggunakan bahasa inggris atau bahasa indonesia
    - Single Comment `//`
    - Multiline `/*  */`
- Tipe data adalah klasifikasi yang kita berikan untuk berbagai macam data yang digunakan dalam programming
- Ada 6 tipe data fundamental pada Javascript
    ```
    1. Number
    2. String
    3. Boolean
    4. Null
    5. Undefined
    6. Object
    ```
- Variabel merupakan wadah atau tempat untuk menyimpan sebuah nilai 3 hal yang dapat dilakukan pada variabel:
    - Membuat variabel dengan nama yang jelas dan menggambarkan tentang data tersebut
    - Menyimpan dan mengupdate informasi/data yang disimpan
    - Mendapatkan/menampilan data yang tersimpan
- Ada 3 cara mendefinisikan sebuah variabel
    - var
    - let
    - const
- Aturan Penamaan Variabel
    - Harus mendeskripsikan tentang data yang disimpan
    - Tidak bisa menggunakan number pada awal nama variabel
    - Gunakan camelcase untuk penamaan yang lebih dari 1 kata. 
- Operator
- Assignment Operator (=) digunakan untuk menyimpan sebuah nilai pada variabel contohnya : `let name = 'Jharmi'`
- Mathematical Assignment Operator
```
  Contoh
      let x = 5 ; 
      x *= 2 ; 
      console.log(x) // Output: 10
```
- Increment dan Decrement digunakan untuk menambah atau mengurangi sebesar 1 nilai
```
  Contoh
      let a = 10;
      a++
      console.log(a) // output: 11
```
- Arithmetic operator adalah operator yang melibatkan operasi matematika.
    Tambah (+)
    Kuramg (-)
    Perkalian (*)
    Pembagian (/)
    Modulus (%)
- Comparism Operator digunakan untuk membandingkan suatu nilai
    - Lebih kecil dari : <
    - Lebih besar dari: >
    - Lebih kecil atau sama dengan: <=
    - Lebih besar atau sama dengan: >=
    - Sama dengan: ===
    - Tidak sama dengan: !==
- Logical Operator digunakan untuk sebuah kondisi
    - AND operator (&&)
    - OR operator (||)
    - NOT operator (!)
- Conditional merupakan statement percabangan yang menggambarkan suatu kondisi. Conditional statement akan mengecek kondisi spesifik dan menjalankan perintah berdasarkan kondisi tersebut
- Contoh Conditional IF Statement
    ```
    - ika cuaca cerah hari ini, maka kita akan pergi keluar
    - Jika alarm berbunyi, maka kita akan bangun dari tidur
    - Jika lelah, maka kita akan istirahat
    - Jika lapar, kita akan makan
    ```
- IF ... ELSE Statement, Else akan mengeksekusi sebuah statement/code jika suatu kondisi bernilai FALSE
    ```
    var siswa = "andi";
    if( siswa == "budi" ) {
    document.write("<b>Budi</b>");
    } else if( siswa == "joni" ) {
    document.write("<b>Joni</b>");
    } else if( siswa == "andi" ) {
    document.write("<b>Andi</b>");
    } else {
    document.write("<b>Siswa tidak terdaftar</b>");
    }
    ```
- IF ... ELSE IF Statement, Else … If statement dapat kita gunakan jika kita mempunyai berbagai kondisi.
    ```
    let num1 = 10
    let num2 = 20

    if (num1 = num2){
    console.log(num1)
    } else if (num1 > num2){
    console.log(num1)
    } else {
    console.log(num2)
    }
    ```
- Switch Case Conditional, digunakan jika kondisi dan percabangan terlalu banyak
    ```
    let warna = "kuning";
        switch (warna){
            case "hitam":
                    console.log ("warna hitam");
                    break;
            case "merah":
                    console.log ("warna merah");
                    break;
            case "hijau":
                    console.log ("warna hijau");
                    break;
            default:
                    console.log ("warna tidak terdeteksi");
  	}
    ```
- Ternary Operator merupakan short-syntax dari statement if ... else
    ```
    let isNowSale = true; isNowSale ? console.log('Let's shopping now) : console.log('Shopping later);
    ```
- Looping adalah statement yang mengulang sebuah instruksi hingga kondisi terpenuhi atau jika kondisi stop/berhenti tercapai
- Macam-macam looping
    - FOR LOOP merupakan instruksi pengulangan yang dapat kita berikan pada program yang kita kembangkan.
    - WHILE LOOP digunakan untuk menjalankan instruksi pengulangan kondisi bernilai TRUE.
    - Do While digunakan untuk mengeksekusi kode setidaknya satu kali bahkan jika kondisi mengembalikan false.
    - Nested loop adalah loop di dalam loop, yaitu kita sebut saja loop luar dan loop dalam. Jadi, konsepnya, iterasi pertama loop luar dijalankan terlebih dahulu, kemudian menunggu sampai loop dalam selesai, baru melanjutkan ke iterasi kedua loop luar yang juga menunggu sampai loop dalam selesai dijalankan lagi, dan diulangi terus sampai semua iterasi dijalankan.






    






