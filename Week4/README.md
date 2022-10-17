# Writing Week 4
## Asycnhronous
  - Fetch merupakan fungsi native yang tersedia pada Javascript dan tidak kalah praktis seperti JQuery saat menggunakannya
    ```
        fetch("https://pokeapi.co/api/v2/pokemon/pikachu/", {
        method: "GET"
        })
         .then(async (response) => {
        let convertData = await response.json();
        console.log(convertData);
        })
        .catch((error) => {
        console.log(error);
        });
    ```
  -  HTTP Request yaitu berfungsi sebagai alat komunikasi frontend dengan backend
  - HTTP Request Method
     - GET untuk mengambil data 
     - POST untuk mengirimkan data
     - PUT untuk mengirimkan atau memperbaharui data
     - DELETE untuk menghapus data  

  - Async/Await merupakan sebuah syntax khusus yang digunakan untuk menangani Promise agar penulisan code lebih efisien dan rapih.Async/Await terbagi menjadi Async dan Await
    ```
       const getAllUser = async ()=> {
         const data = await getUser()
         console.log(data)
       }
    ```
  - Pertama kita memiliki function dengan menambahkan async didepan function yang mana berfungsi untuk menjadikan function tersebut asynchronous, dan await berfungsi menunda eksekusi hingga proses asynchronous selesai, dari kode di atas berarti console.log(data) tidak akan di eksekusi sebelum proses getUser() selesai. await juga bisa digunakan berkali-kali di dalam function
  
## Responsive WEB Design
  - Responsive web design adalah suatu tampilan website yang dapat menyesuikan dengan perangkat yang digunakan. Tujuannya untuk membuat desain website dapat digunakan atau dapat diakses di device apapun
  - Setiap developer website wajib menggunakan tools bawaan yang memudahkan dalam proses development website. Chrome dev tools merupakan tools pada google chrome yang digunakan sebagai tools Responsive Web Design
  - Mengakses Chrome dev tools
    ```
    Ctrl + Shift + J
    ```
  - Pada HTML perlu ditambahkan viewport pada bagian head agar tampilan website dapat menyesuaikan dengan berbagai device
    ```
    <meta name="viewport" content="width= device-width, iitial-scale= 1.0">
    ```
  - Untuk membuat suatu gambar pada halaman website agar menjadi responsive dapat dilakukan dengan menambahkan atribut Max - width = 100% pada bagian gambar
  - Media Query salah satu cara untuk mengatur suatu website agar bisa terdiri dari beberapa jenis
  - Cara menggunakan media query:
    - Memisahkan beberapa file css sesuai dengan tampilan device yang ingin dibuat
    - Menggabungkan semua styling css device menjadi 1
  - Breakpoint yaitu istilah saat terjadi perubahan ukuran pada suatu website ketika berganti
  device. Terdapat 3 jenis breakpoint yaitu desktop, tablet, dan mobile phone
  - Penggunaan breakpoint pada media query dapat dilakukan dengan membuat range ukuran sesuai dengan tampilan device yang ingin dibuat
  - Flexbox bertujuan untuk membuat website yang lebih efisien dalam mengatur, menata dan item pada dalam sebuah wadah bahkan ketika ukurannya tidak diketahui dan/atau dinamis (dengan menggunakan kata "flex")
  - Flexbox properties:
    - Flex direction adalah menetapkan sumbu utama item, sehingga menentukan arah item fleksibel ditempatkan di wadah fleksibel
    - Flex Wrap adalah Secara default, semua item pada flexbox akan mencoba berada dalam satu baris. Maka dengan flex wrap kita dapat mengubah hal tersebut
    - Flex flow adalah cara singkat untuk properti flex-direction dan flex-wrap, yang bersama-sama menentukan sumbu utama dan sumbu silang container flex. Nilai default adalah baris nowrap
    - Align item adalah item-item pada container flex tersebut diletakkan sepanjang garis tegak lurus pada sumbu utama
    - Grid merupakan sistem tata letak berbasis dua dimensi
    - Pada Grid ada 2 jenis yaitu grid container dan grid item
## Boostrap
- Bootstrap adalah salah satu framework opensource yang berfungsi membuat suatu responsive website. Komponen utama bootstrap :
  - bootstrap.css
  - bootstrap.js
- Cara konfigurasi bootstrap :
  - Membuat tag boostrap di head. Cara memanggil css bootstrap dengan menggunakan href lalu mengganti link href css lokal dengan link boostrap online
- Contoh penggunaan content bootstrap :
  - CSS : bootstrap.min.css, bootstrap-grid.css, dll
  - JS : bootstrap.bundle.js, bootstrap.min.js, dll
- Komponen Bootstrap sebagian besar dibangun dengan base-modifier nomenclature. Contohnya mengelompokkan beberapa properti kedalam kelas dasar seperti .btn, seperti .btn-primary or .btn-success
- Layout pada boostrap menggunakan breakpoints. breakpoints merupakan suatu cara yang dilakukan untuk membuat desain responsif dengan mengontrol kapan tata letak yang disesuaikan dengan ukuran perangkat tertentu
- Container adalah blok dasar atau pembungkus boostrap yang terdiri dari contain, pad dan align yang menyelaraskan konten website dalam perangkat atau area pandang tertentu
- Grid System pada bootstrap yang terdiri dari 12 kolom default. Grid system pada bootstrap menggunakan container,baris dan kolom untuk menata dan menyelaraskan konten,yang dibangun menggunakan flexbox dan itu sudah responsive
- Grid system bootstrap :
  - .col-lg digunakan untuk mengatur grid pada ukuran monitor yang besar
  - .col-md digunakan pada monitor komputer berukuran sedang
  - .col-sm digunakan untuk mengatur monitor pada tablet
  - .col-xs digunakan untuk mengatur monitor pada handphone
