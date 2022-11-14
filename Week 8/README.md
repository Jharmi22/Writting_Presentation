# Writting week 8

## React Context
- Context adalah salah satu State Management yg di khususkan buat React Js serta mengelola state secara global, dapat di gunakan bersama useState Hook untuk berbagai state.
- React Context dirancang untuk berbagi data yang dapat dianggap "global" untuk pohon komponen React, seperti pengguna yang diautentikasi saat ini, tema, atau bahasa pilihan
- Penggunaan React Context
  - Untuk membuat new context, gunakan fungsi createContext baru React
  - Fungsi createContext mengembalikan a Provider dan a Consumer component
- Cara menggunakan React Context
  - Buat Sebuah Folder context di dalam folder src dan di dalam folder tersebut terdapat file dengan nama `<AppContext.js>`
    ```
      // 1. Import React Library
    import React from "react"

    // 2. Definisikan variable dengan assign value React.createContext()
    export const AppContext = React.createContext()
    ```
- Lalu beralih ke `<App.js>` dan jangan lupa ,mengimport Home dan file-file yg kita butuhkan.
- Buat sebuah folder components dan di dalamnya ada folder navbar lalu di dalam folder navbar ada file `<Navbar.jsx>`

## React Testing
- Testing berarti memeriksa bahwa kode kami memenuhi beberapa harapan
- Testing dibagi menjadi 2 main kategori yaitu:
  - Manual Testing:
    - Aplikasi bebas dari error dan bug
    - Aplikasi berjalan sesuai dengan ekspektasi
    - Meningkatkan kualitas dari sebuah software dan kepuasan pengguna
  - Automated Testing:
    - Lebih reliable karena Manual Testing tetap berpotensi adanya kesalahan dan kekeliruan
    - Lebih cepat dan efisien
    - Mudah untuk dimaintain (Review, Edit, dan Add Collection of Tests)
- Alur Testing:
  - import fungsi untuk menguji
  - Memberikan masukan ke fungsi
  - Menentukan apa yang diharapkan sebagai output
  - Memeriksa apakah fungsi menghasilkan output yang diharapkan
- Perlunya dilakukan testing:
  - Tujuan pertama dari testing adalah untuk mencegah regresi. Regresi adalah kemunculan kembali   - bug yang sebelumnya telah diperbaiki. Itu membuat fitur berhenti berfungsi sebagaimana     dimaksud setelah peristiwa tertentu terjadi
  - Testing digunakan memastikan fungsionalitas komponen kompleks dan aplikasi modular.
  -Testing diperlukan untuk kinerja yang efektif dari aplikasi perangkat lunak atau produk.
- React Testing Library dibangun di atas DOM Testing Library dengan menambahkan API untuk bekerja dengan komponen React.
- Menginstall library testing `npm install --save-dev @testing-library/react`
  
  
