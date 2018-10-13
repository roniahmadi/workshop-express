# Step 4 - Berkominikasi dengan Server

Sekarang Anda telah membangun server, Anda perlu berkomunikasi dengannya. Anda akan mengontrol server dengan **handler function**.

### Apa itu handler function?

Ketika request sampai ke server, Anda membutuhkan cara untuk menanggapinya. Handler function hanyalah sebuah fungsi yang menerima permintaan atau *request* dan menanganinya sesuai namanya.

Handler function selalu mengambil objek `request` dan` response`, dan mengirim respon kembali ke klien bersamaan dengan beberapa informasi. Anda dapat memutuskan apa yang harus dikirim kembali dalam respons Anda.

### Apasaja handler function Express?

Metode `get()` digunakan untuk mendefinisikan handler function dalam Express. Diperlukan dua parameter: **endpoint** untuk memicu suatu aksi (saya akan menjelaskan lebih lanjut tentang ini di langkah berikutnya), dan handler function yang memberi tahu dengan tepat apa yang harus dilakukan. contoh sederhana:

```js
app.get('/', function (req, res) {
    res.send('Halo, Asrul')
});
```

Di sini, kita memberi tahu server untuk merespons dengan "Halo, Asrul" ketika seseorang mencoba mengakses halaman web.

## 1. Membuat handler function.

Anda sekarang membuat fungsi dengan pesan khusus dalam tanggapan server. Anda dapat menulis pesan apa pun yang Anda inginkan.

Perbarui file `app.js` Anda dengan fungsi `app.get()` kosong:

```js
var express = require('express')
var app = express()

app.get('/', function (req, res) {

})

app.listen(3000, function () {
  console.log('Server telah berjalan di port 3000')
})
```

Cobalah `console.log` objek `req` di dalam handler function. Restart server Anda, refresh browser, lalu pergi ke terminal Anda untuk melihat seperti apa tampilannya. Anda akan melihat informasi muncul.

## 2. Ubah handler function sesuai keinginan

Ketika Anda ingin memberikan response ke client beberapa informasi, Anda dapat melakukan itu dengan menggunakan metode Express `send()`. Ini akan memperbarui objek respons dengan informasi tersebut.

Ubah handler function Anda:

```js
var express = require('express')
var app = express()

app.get('/', function (req, res) {
  res.send('Selamat belajar bos!')
})

app.listen(3000, function () {
  console.log('Server telah berjalan di port 3000')
})
```

## 3. Cek pada browser

Keluar dari server Anda di terminal dengan `ctrl + c`. Kemudian restart untuk menjalankan perubahan baru Anda.

```
$ node app.js
```

Sekarang, buka browser favorit Anda (seperti Chrome), dan arahkan ke `http://localhost:3000`. Jika Anda melihat pesan Anda di browser, selamat! Anda baru saja mengirim respons pertama Anda dari server.

### [Langkah 5 >>>>](https://github.com/talkasrul/workshop-express/blob/master/learn/step_05.md)
