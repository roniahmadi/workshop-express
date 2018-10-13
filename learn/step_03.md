# Langkah 3 - Membangun server

Hal pertama yang perlu kita lakukan adalah membangun server. Anda harus membangun server saat menulis kode **back-end**. Sebuah server dapat dibangun di Node.js murni, tetapi Express memberi kita sintaks yang lebih sederhana untuk digunakan.

## Apa itu server?

Server adalah program komputer yang menerima permintaan dari program lain, *klien* dan mengirim balasan, misalnya, berbagi data, informasi, perangkat keras, dan resource software.

Mari kita ambil situs web misalnya. Situs web hanyalah kumpulan file HTML dan CSS, gambar, mungkin beberapa file javascript. Saat Anda mengetik alamat situs web di url browser Anda, Browser (klien) mengirim **permintaan** ke server yang sesuai dengan alamat itu. Browser meminta server untuk memberikannya file yang diperlukan untuk ditampilkan sesuai situs web dengan benar.


![Server flow](https://files.gitter.im/heron2014/FiiK/server.png)

## 1. Membuat file `app.js`

Sebelum kita melakukan apa pun, mari kita buat file baru bernama `app.js`. Di sinilah semua kode server akan dijalankan.

## 2. `require express` dari librari

Kita telah menginstal Express pada Langkah 2, tetapi kita harus memastikannya disertakan dalam file ini sehingga dapat menggunakan apapun metode-metode yang disediakan oleh Express. Di Node.js, ketika Anda ingin mengakses fungsionalitas librari atau modul dari file lain, Anda harus `require`.

Untuk mengimpor Express, tulis di dalam `app.js` berikut:

```js
const express = require('express')
```

## 3. Inisialisasi server

Untuk menginisialisasi server, Anda hanya perlu memanggil fungsi `express()`. Ini akan membuat Express berfungsi pada aplikasi yang Anda bangun.

Tambahkan baris kode kedua ke file `app.js` Anda:

```js
const express = require('express')
const app = express()
```

## 4. Lakukan 'listening' untuk menjalankan server

Tinggal satu langkah lagi, kita perlu mengatur **port** untuk dilisten oleh server. Pikirkan port sebagai nomor masuk server; setiap permintaan yang datang ke server akan datang melalui port itu. Mengatur port akan menjadikan server Anda berjalan.

Kita menggunakan metode ** `app.listen` ** untuk melakukan ini. Metode ini membutuhkan dua argumen: **port** dan **callback function** yang memberitahukan apa yang harus dilakukan setelah server berjalan. Butuh kelarifikasi? Baca method `app.listen` pada [Dokumentasi Express](http://expressjs.com/en/4x/api.html#app.listen).

Kami akan menjalankan server kami di port `3000`, dan menjalankan` console.log` sederhana sebagai fungsi panggilan balik kami. Perbarui file `server.js` Anda, panggil metode` app.listen`:

```js
const express = require('express')
const app = express()

app.listen(3000, function () {
  console.log('Server telah berjalan di port 3000')
})
```

## 5. Aktifkan server!

Anda telah membangun server, tetapi belum berjalan. Kita perlu menjalankan perintah di terminal untuk mengaktifkannya. Kita akan menggunakan kata kunci `node` untuk menjalankan file server.

Ketik perintah berikut pada terminal:
```
$ node app.js
```

Jika melihat seperti gambar berikut maka saya ucapkan **SELAMAT**!

![Berhasil Jalan](https://github.com/talkasrul/workshop-express/blob/master/img/serverRunning.png?raw=true)


### [Langkah 4 >>>>](https://github.com/talkasrul/workshop-express/blob/master/learn/step_04.md)

## Kata kunci
?
dalam pengembangan