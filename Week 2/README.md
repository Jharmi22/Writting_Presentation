# Writing Week 2
## Js-Scope and Function
### Scope
- Scope adalah konsep dalam flow data variabel. Menentukan suatu variabel bisa diakses pada scope tertentu atau tidak
- Blocks adalah code yang berada didalam curly braces `{}`. Conditional, function, dan  looping menggunakan blocks.
Scope ada dua macam:
  - Global scpoe, variabel yang dibuat dapat diakses dimanapun dalam suatu file. Agar menjadi Global Scope, suatu variabel harus dideklarasikan diluar Blocks.
    ```
    let namaSaya = 'Jharmi';

    function greeting() {
        return namaSaya;
    }
    console.log(namaSaya);
    ```
  - Local Scope, mendeklarasikan variabel didalam blocks seperti function, conditional, dan looping. Maka variabel hanya bisa diakses didalam blocks saja. Tidak bisa diakses diluar blocks.
    ```
    function greeting() {
      let namaSaya = 'Jharmi';
      return namaSaya;
    }
    console.log(greeting())
    console.log(namaSaya);
    ```
### Function    
- Function adalah sebuah blok kode dalam sebuah grup untuk menyelesaikan 1 task/1 fitur
- Membuat function
  ```
    function greeting () {
    return 'Hello word';
    };
  ```
- Cara memanggil function
  ```
  greeting()
  consosle.log(greeting());
  ```
- Parameter, function dapat menerima sebuah inputan data dan menggunakannya untuk melakukan task/tugas
    ```
    function penambahan(a, b){
      return a + b;
    }
    ```
- Argumen adalah nilai yang digunakan saat memanggil function, jumlah argumen harus sama dengan jumlah parameternya
    ```
    function penambahan(a, b){
      return a + b;
    }
    console.log(6, 7)
    ```
- Function, dapat menggunakan function yang sudah dibuat pada function lain
- Arrow function adalah cara lain menuliskan function. Ini adalah fitur terbaru yang ada pada ES6 (Javascript Version)

## Data Type Built in Prototype & Method
- Data Type adalah jenis-jenis data yang bisa kita simpan di dalam variabel. Terdapat dua macam type yaitu primitive value and object
  - Primitive values, nilai yang sudah ditentukan sebelumnya
    - Boolean type
    - Null type
    - Undefined type
    - Number type
    - String type
  - Object, wadah untuk nilai yang diberi nama atau biasa disebut properti atau method.
- Math, objek bawaan yang memiliki properti dan metode untuk konstanta dan fungsi matematika, math ini bukan merupakan objek fungsi
- Non-primitive,  tipe data yang didefinisikan sendiri oleh programmer dan biasanya berisi lebih dari satu nilai
  - Object
  - Array
  - Function
- DOM  merupakan cara memanipulasi html agar website lebih dinamis dan interaktif
- Cara memanggil DOM:
  - berdasarkan ID `console.log(document.getElementByID("header))`
  - berdasarkan class name `console.log(document.getElementByClassName("text-color-blue"))`
  - berdasarkan query selector `console.log(document.querySelector("#header "))` `console.log(document.querySelector(".text-color-blue"))`
  
- Cara memanipulasi konten
  - Deklarasi varible header sebagai wadah untuk menyimpan tag HTML `let header = document.getElementById("header");`
  - Memanipulasi Content pada Header Content dari pemilik element dengan ID Header dengan text.Content `document.getElementById("header").textContent = "Teks Heading"`
- Membuat element HTML
  ```
  <div id ="header"></div>

  //untuk membuat sebuah elemnt heading
  const heading = dosument.createElement("h1)
  heading.textContent = "Ini Heading"

  document.getElemntByID("header").appendChild(heading)
  ```
- DOM Event merupakan object model yang bertugas untuk membantu interaksi user dengan document HTML. Contoh HTML DOM event
  - Click
  - Scroll
  - Change
  - Focus
  - Hover
  - Submit
  - Blur
- Menangkap interaksi user
  - `Element.addEventListener(“event”)`
  - `Element.onevent`
- EventListener <br>
Dengan menggunakan cara `Element.addEventListener(“event”)` maka akan
  - Bisa dihilangkan
  - Bisa ada beberapa event 
  - Memiliki argument tambahan { options }
- EventListener - Blur : event dimana sebuah element kehilangan fokus dari user
- EventListener - Form Submission
- Contoh EvenListener - Form Submission <br>
Misalkan terdapat beberapa input dalam sebuah form `<input name="email"/>` dan `<input type="password" name="password"/>` <br>
Untuk mendapatkan isi dari kedua inputan tersebut terdapat 2 cara :
  - Memasang event listener di kedua input dan tombol submit, lalu saat tombol diklik, baca value dari kedua input tersebut
  - Memasang event listener di form, lalu gunakan FormData untuk menggambil data dari masing-masing input
  ``` const form = document.getElementById("form")

  form.addEventListener("submit", function(event)){
  event.preventDefault()

  const formData = new FormData(form)
  const values = Object.fromEntries(formData) {
    email: ....
  }
  }) 
  ```

 







