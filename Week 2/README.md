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











